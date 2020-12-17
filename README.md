# -_empty-project
Folder/Directory structure and files for starting a new website project.

Some notes on index.html
------------------------
This is a basic structure for a standard web page.  It has a header at the top, a footer at the bottom, and a main element as a starting place for content. While the main element must be unique on the page, you can have multiple header and footer elements (e.g. in addition to these two, and article element could have its own header). To account for this, I use classes on the header and footer elements so that I can target them with CSS rules.

**What's with the "Skip to content" link?**
This is a link that allows users to jump directly to the content area.  It is typically hidden with CSS and is primarily for users of assistive technologies (e.g. screen readers). But even if you are seeing an HTML only version of the file if your header/navigation is long enough having a skip to content link at the top of the page is nice.

Read about it:
* https://webaim.org/techniques/skipnav/
* https://css-tricks.com/how-to-create-a-skip-to-content-link/
* http://web-accessibility.carnegiemuseums.org/code/skip-link/

**Why the page-frame and content-frame divs?**
I use these two container divs to allow CSS layout styling over the whole page or just the content area (separate from the header and footer).  By having the div.page-frame element I can, for example, set a background-color and max-width on the page which I can then center in the body element so as to center the page in the browser.  By having a div.content I can have the page-header and page-footer elements be full width if I so choose, will setting a max-width on the div.content for readability.
