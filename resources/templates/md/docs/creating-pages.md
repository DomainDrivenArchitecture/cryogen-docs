{:title "Creating Pages"
 :layout :page
 :page-index 5
 :section "Your Content"}
 
Creating pages is not much different from writing posts. You're still required to include the map representing the metadata and the page must be written in valid Markdown. 

## The Pages Folder

Similar to your posts, all of your pages should reside under the `page-root` folder specified in your configuration file. Again, as long as the file contains the proper metadata followed by valid Markdown content, they will be converted into an HTML page. 

## Creating Pages

To create a new page, just make a new Markdown file under your `page-root`. You don't need to include a date in the file name like you need to with a post but words should still be dash-separated and the file must have a `.md` extension. For example:

```
about.md
my-projects.md
```

### Page Contents

The following information is mandatory in your page metadata.

  * `:title` - A string representation of your page title.
  * `:layout` - A keyword representing the name of the HTML file that you want to use as your page layout.
  * `:page-index` - Because pages can be linked up with previous/next links, this is how they get sorted.
  * `:navbar?` - Set this to true if you want the link to this page to appear in the navbar. Set it to false if you want it in the sidebar.

For example:

```
{:title "Check out this page!"
 :layout :post
 :page-index 0
 :navbar? false}
```

### Images in Your Pages

You can include images in your pages in the same way you include images in your blog posts. Please refer to the "Including Images in Posts" and "Images in Markdown" sections of the [Writing Posts](/docs/writing-posts.html) page.

### Highlighting Code Snippets

Want to show off your code in a page? It works the same way as it does in posts. Just wrap your code block in triple backticks and highlight.js will take care of the rest.