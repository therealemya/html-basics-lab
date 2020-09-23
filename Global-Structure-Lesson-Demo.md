<img  src="code-diff-logo.png" alt="Code Differently Logo" style="height:100px; width:300px;">

# Demo - Getting Started with HTML and Structuring Your Content


## Getting Started with HTML


### What is HTML?
* HTML is a programming language used to create and display webpages

* HTML stands for Hypertext Markup Language

    * Hypertext = word or words that contain a link to a website

    * Markup Language = computer language that uses tags to define elements in an HTML document.

### Global Structure of an HTML Document

There are 1000s of webpages on the internet and each one is different. They do have one thing in common, the global document structure. 

#### DOCTYPE
* `<!DOCTYPE HTML>` is a declaration on the first line of code on an HTML document. It defines the document type. This is not a tag or an element.

* The declaration is not case-sensitive

#### HTML
* `<html>` element tell the web browser that this is an HTML document. 

#### HEAD
* `<head>` element follows the `<html>` element. This contains the `<title>` element and metadata. Content wrapped by the `<head>` tag does not appear on the webpage. The `<link>` element, which is used to link the HTML document to an outside resource, is nested in the `<head>` element as well.

#### TITLE 
* `<title>` element names the HTML document. The title of the HTML document will appear on the tab of the current page.

#### BODY
* `<body>` element is where all content appears. All that is visible on a webpage is nested inside of the `<body>` element.

--

## HTML Headings
* Most HTML documents begin with a heading. With HTML you can use different elements to display various sizes. 

* HTML has six levels of headings beginning with `h1` indicating the highest level of priority. 

* All headings are block-level elements


```html
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
<h4>This is heading 4</h4>
<h5>This is heading 5</h5>
<h6>This is heading 6</h6>

```


## HTML Semantic Markup & The `<p>` Element


### Semantic Markup

- Semantics is the meaning behind words, phrases, or any text.

- In relation to HTML, markup should describe the meaning of content rather than how it looks.

- With semantic markup, websites are more understandable to search engines and also helps users with screen reading software navigate on a website.


### `<p>` Element

* Allows developers to structure their HTML document into paragraphs.

* `<p>` elements have opening and closing tags

    * `<p></p>`

* Paragraph elements are block-level elements


### Structuring Content

* A common webpage will be divided into three sections:

    - <strong> `<header>` </strong>: contains the introductory content

        - site logo, navigation, menu, etc.

    - <strong>`<main>`</strong>: holds the most important content

        - blogs, articles, image galleries, etc.

    - <strong>`<footer>`</strong>: contains information about the site

        - address, copyright date, etc. 

### Sectioning Content

* We can go even further with adding sectioning to our content using `<article>`, `<nav>`, and `<aside>` elements.

    - `<article>` is used to represent a self-contained piece of content on the webpage such as a blog entry.

        - This could be used to wrap and article's heading, entry, and article information, making it a single component on the webpage.

    - `<nav>` is used to nest the list of links to other pages or sections within the page.

        - This element communicates that its content is an important section containing navigation links which assist with screen readers. 

    - `<aside>` element allows developers to section content that is sort of related to the main topic but could be removed. Think of a Twitter feed on a page or a list of related articles or resources.

### Grouping Content 

-  The `<main>` element is used to nest the main content of the web page. Sections like the about, articles, and contact information are placed inside of the `<main>` element. 

    - This element also assists with screen readers and other technologies that assist those surfing the internet.

    - `<header>` and `<footer>` elements would not be included in the `<main>` element.

    - There should only be one `<main>` element per page

- The `<div>` element is another element used for grouping content. It has little semantic meaning but is widely used for grouping.

    - Developers use this element as a wrapper for an entire page to aid in controlling the width of the layout. Also makes it easier to center the webpage with CSS later.

    - Wrapping an inline element with a `<div>` elements will make it block-level.

### Adding Quotes

* `<q>`: this element is used for marking up short inline quotes. 

* `<blockquote>`: this element is used for marking up long, multi-line quotations. If you have a webpage with a blog, you may want to quote an excerpt from another source. 

    * To credit the author of the source a `cite` attribute can be used within the `<blockquote>` element. Its value is the location of that source. 


