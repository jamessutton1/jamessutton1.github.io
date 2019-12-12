# Minimal Mistakes remote theme starter

Contains basic configuration to get you a site with:

- Sample posts.
- Sample top navigation.
- Sample author sidebar with social links.
- Sample footer links.
- Paginated home page.
- Archive pages for posts grouped by year, category, and tag.
- Sample about page.
- Sample 404 page.
- Site wide search.

## Basic Setup

- Install [Git](https://git-scm.com/download/win). you dont need the GUI or Bash window, but the bash does make branch management easier with pretty colors.
- Create a folder to store your sites files. For example, `~/Desktop/GitWebsite/`
- Open the command prompt
- Navigate to your site folder: `cd /Desktop/GitWebsite/`
- Clone this repository: `git clone https://github.com/jamessutton1/jamessutton1.github.io.git`
- Customize files with markdown as needed!
- Update website with following git commands (Run these from the `~/Desktop/GitWebsite/jamessutton1.github.io` folder __the root directory of the repository__)
- `git add --all`
- `git commit -m "some comment"`
- `git push -u origin master`
- Your domain, [**jamessutton1.github.io**](https://jamessutton1.github.io/) should be ready in a minute!

You could also edit files directly in the github.com editor like a fucking noob, which requires no setup.

[**Markdown refrence**](https://kramdown.gettalong.org/quickref.html)

[**Documentation**](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)

[**Example Files**](https://github.com/mmistakes/minimal-mistakes/tree/master/docs)

## Programming Guide

All of text is markdown. Use [**Markdown refrence**](https://kramdown.gettalong.org/quickref.html).
`.html` and `.md` files don't use tabs, just two spaces. It will break everything. All of the photos I downloaded off your Blogspot have to be addressed with an all caps `.JPG`. idk
- make a post take up the full screen width by adding `classes: wide` to the front matter of the page. (in the top --- portion)
- If you want to remove the teaser photos from the Posts page, open the file `_includes/head/custom.html`. On line 15, change `or` to `and`. Example for no teaser image: `{% if include.type == "grid" and teaser %}`

- `_config.yml` sets global site variables
- `index.html` is homepage settings
- `_pages/about.md` is about page settings
- `_posts` contains all posts. The date in file name sets the post's "post date." You can add subfolders to this folder for organization.
- All images go in `/assets/images/`. Try to keep image size under 2 MB for quick loading. You can also link images. See [post examples](https://github.com/mmistakes/minimal-mistakes/tree/master/docs/_posts). When viewing `.md` files in GitHub, click the __Raw__ button to view it as plaintext code. 
- If you can't figure out how to format a type of post, visit [**Here**](https://mmistakes.github.io/minimal-mistakes/year-archive/) for examples (this site is the domain of the documentation being refrenced). Note the final portion of the URL of the post of intrest. Find this name in [this section](https://github.com/mmistakes/minimal-mistakes/tree/master/docs/_posts) of the documentation.

- I added a site icon that appears in the tab on mobile and desktop. If you want to change these, delete all of the image files in the root folder. Create a new image set [Here](https://favicon.io/). Extract the download and copy the photos to the root website directory.
- Delete everything and paste the html code snippet given by the Favicon generator into this file `/_includes/custom.html`. Mine was

~~~ html
<!-- start custom head snippets -->
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="manifest" href="/site.webmanifest">
<!-- end custom head snippets -->
~~~

---

## Troubleshooting

If you have a question about using Jekyll, start a discussion on the [Jekyll Forum](https://talk.jekyllrb.com/) or [StackOverflow](https://stackoverflow.com/questions/tagged/jekyll). Other resources:

- [Ruby 101](https://jekyllrb.com/docs/ruby-101/)
- [Setting up a Jekyll site with GitHub Pages](https://jekyllrb.com/docs/github-pages/)
- [Configuring GitHub Metadata](https://github.com/jekyll/github-metadata/blob/master/docs/configuration.md#configuration) to work properly when developing locally and avoid `No GitHub API authentication could be found. Some fields may be missing or have incorrect data.` warnings.
