** !-- Document Header Starts -->**

An unordered list starts with the <ul> tag. Each list item starts with the <li> tag

The anchor element is used to create hyperlinks between a source anchor and a destination anchor. 

Read more: https://html.com/anchors-links/#ixzz5zF85ieap


The HTML <p> element represents a paragraph. Paragraphs are usually represented in visual media as blocks of text separated from adjacent blocks by blank lines and/or first-line indentation, but HTML paragraphs can be any structural grouping of related content, such as images or form fields.


HTML defines six levels of headings. A heading element implies all the font changes, paragraph breaks before and after, and any white space necessary to render the heading. The heading elements are H1, H2, H3, H4, H5, and H6 with H1 being the highest (or most important) level and H6 the least. For example:


#### LAB 2 

The DOCTYPE is intended to tell browsers which specific set of rules should be used in interpreting the markup. Why you may ask? it is so that no sloppy or invalid code passes by. 

In practice, its use in HTML and web development is slightly different, and has to do with browsers being forgiving of sloppy or invalid code.

Basically, because code quality was (and is) very low in lots of web pages, browsers' rendering engines are very fault tolerant, and dealt with certain aspects of layout according to an emerging set of expectations.

Many, or even most, of these sloppy pages lacked doctypes. At some point the major browsers started using the presence of a doctype as a signal from the developer saying "I know what I'm doing," and this caused the browser to use rendering behaviors that adhere (more) strictly to the established HTML and CSS standards, but which might look different than the more forgiving, "quirky" rendering modes.

You should use this simple doctype (the HTML5 doctype), to trigger "standards mode" rendering in browsers:

<!doctype html>

...unless you are serving XHTML pages with an application/xhtml+xml MIME type. If you don't know what that means, you should definitely use the simple one. It works in every major browser, right back through IE6.


LAB 4


Forms allow unscripted client-server interaction: given a form, a user can provide data, submit it to the server, and have the server act on it accordingly (e.g. returning the results of a search or calculation). 

<form Attributes >
button 
fieldset
input
keygen
label
object
output
select
textarea

The <fieldset> tag is used to group related elements in a form.

The <fieldset> tag draws a box around the related elements.

 The <legend> tag defines a caption for the <fieldset> element.

fieldset {
  display: block;
  margin-left: 2px;
  margin-right: 2px;
  padding-top: 0.35em;
  padding-bottom: 0.625em;
  padding-left: 0.75em;
  padding-right: 0.75em;
  border: 2px groove (internal value);
}