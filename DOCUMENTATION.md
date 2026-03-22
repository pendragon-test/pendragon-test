# Documentation

The site is written using [Jekyll](https://jekyllrb.com/). Jekyll is a site generator that works from templates and layouts. For the most part, you shouldn’t need to worry about how Jekyll works.

You can either make changes locally (using a local editor and git) or through siteleaf.

Page can either be normal HTML (.html) or Markdown (.md) files, and include metadata about the page, such as title, date, and layout. In siteleaf, metadata can be edited on the right hand side when editing a page. When editing files locally, the metadata is at the top of the file between the `---` lines.

## Local development
You can run a local development server by running the script `run-local-dev-server.bat`. Then it should be available at http://localhost:4000

You can then edit the files through whatever editor you like . Changes to the site should appear in the browser in real-time.

When you have made changes, [commit](https://docs.github.com/en/desktop/making-changes-in-a-branch/committing-and-reviewing-changes-to-your-project-in-github-desktop) (select the files you want to commit on the left of github desktop, enter a commit message in the bottom left, and then hit “commit”) and [push](https://docs.github.com/en/desktop/making-changes-in-a-branch/pushing-changes-to-github-from-github-desktop) the changes (Hit the “Push origin” button on the top of github desktop)

In order to get the changes to the live site, you still have to, for now, log in to siteleaf and then hit “Publish” in the top left.

## How to create a new collection of stories (siteleaf)
* In Siteleaf, click on “New Collection” to create the collection.
* You need to create the links for the pages in order to make the collection visible however. You can ask me for help with this if you need. (I will also try to simplify this, so you don’t have to all this)
  * Create a page for the collection as follows:
    * Go to “Pages” on the right hand-side, and add a new page
    * Title the page the collection’s title
    * Click the pencil next to the URL/path below the title and title it `stories/[collection-name].html` or something like that
    * At the bottom of the page, click “New metadata field” and then give it the Field name of `collection` and then the value of the name of your collection, all lower case with hyphens for spaces (for example, `santa-claire` for the collection “Santa Claire”)
  * Add that link to the “Stories” page (also)
    * Go to “Pages” then click on “Stories”
    * Copy and paste line starting with `<li>`, change the href to the path you set above, and the collection title as above
  * If you also just wanted all your posts on one page instead of organized into subpages like this, lmk and I can make that change

## How to upload a new story to a collection (siteleaf)
* Click the circle/plus button to the right of the collection to add a new entry
* On the right hand side, click the “Advanced options” and change the layout to “post” (otherwise there will be no styling applied to the page)
* It defaults to markdown, you can change to html by setting an explicit path (pencil icon below title) to something ending in html
* You can [export libreoffice documents to markdown](https://help.libreoffice.org/latest/en-US/text/swriter/guide/markdown.html?DbPAR=WRITER) (although your libreoffice version I think has to be 25 or 26) and then copy the text in.

## How to upload new images (siteleaf)
* Click on “Site” on the right hand side
* Go to the “images” folder, then either the “rasters” or “vectors” folder
* Hit “Upload files” to add new images
* Images will be displayed on the site in alphabetical order. I can change this if you like, or you can add dates or something as prefixes to make sure things are sorted in the order you like

## How to upload new images (local)
* In the folder where you cloned the site, go into “images” then “rasters” or “vectors”, and copy your files there
* Commit those images in github desktop and push the commit

## Making the site “live”
When you want the site to be live, I’ll set up the contact form so it hits your email, and we can change the domain name to whatever you would like.
