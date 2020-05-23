<h4 id="C0">Top</h4>

# Getting Started
<p><a href="#C1">Basic HTML tags</a></p>
<p><a href="#C2">HTML Formatting</a></p>  
<p><a href="#C3">HTML Links</a></p>
<p><a href="#C4">HTML Lists</a></p>
<p><a href="#C5">HTML Tables</a></p>
<p><a href="#C6">Div and Span</a></p>
<p><a href="#C7">Class and Id</a></p>
<p><a href="#C8">Forms</a></p>


## What's HTML?
* Is a **Markup Language** 
* Stands as __Hypertext Markup Language__
* Used to describe Web documents or Web pages
* HTML elements tell the browser how to display the content
* HTML elements are represented by tags
* Browsers do not display the HTML tags, but use them to render the content of the page
## A Simple HTML Document

 ``` javascript
 <!DOCTYPE HTML>
 <html>
     <head>
         <title>Getting Started with HTML</title>
    </head>
    <body>
    <h1>Getting Started</h1>
    <h2>Our first Web Page</h2>
    </body>
</html>
```
* The `<!DOCTYPE html>` declaration defines this document to be HTML5
* The `<html>` element is the root element of an HTML page
* The `<head>` element contains meta information about the document
* The `<title>` element specifies a title for the document
* The `<body>` element contains the visible page content
* The `<h1>` element defines a large heading

<h2 id="C1">Basic HTML Tags</h2>
* HTML tags are element names surrounded by angle brackets:

        `<tagname>`content goes here...`</tagname>`

* HTML tags normally come in pairs like `<p>` and `</p>`
* The first tag in a pair is the start(opening) tag, the second tag is the end(close) tag

 ``` javascript
<!DOCTYPE html>
<html>
    <head>
        <title>Getting Started with HTML</title>
    </head>
    <body>
    <h1>Header 1</h1>
    <h2>Header 2</h2>
    <h3>Header 3</h3>
    <h4>Header 4</h4>
    <h5>Header 5</h5>
    <h6>Header 6</h6>
    
    <p>This is an example of a paragraph.</p>
    <p>This is my second paragraph.</p>
    
    <a href="http://www.google.com">Go to Google</a>
    <img src="https://www.google.com/images/srpr/logo11w.png">

    </body>
</html>
```
## Image Attributes and Links
```
    <a href="http://www.google.com">
        <img src="https://www.google.com/images/srpr/logo11w.png" alt="Google Logo" height="50px" width="150px">
    </a>
```
<a href="#C0">Top</a>

<h2 id="C2">HTML Formatting</h2>

* Paragraph `<p> </p>` starts with newline
```dotnetcli
<!DOCTYPE html>
<html>
    <head>
        <title>HTML FORMATTING</title>
    </head>
    <body>
    <h1>HTML Formatting</h1>
        
    This is just text.
        
    <p>This is a paragraph.</p>
        
    <b>This is bold text.</b>
    <br>    
    <strong>This is strong text.</strong>
 
    <i>This is italic text</i>
    <br>
    <em>This is emphasized text</em>
    <br>
    <h1>This is an example of a <small>small</small> text formatting</h1>
    <br>
    <h1>This is an example of a <mark>marked</mark> text formatting</h1>       
    </body>
</html>
```
## Citations and Quotations
* The HTML `<q>` element defines a short quotation. Browsers usually insert quotation marks around the `<q>` element.
* The HTML `<cite>` element defines the title of a work. Browsers usually display `<cite>` elements in italic.
* The HTML `<blockquote>` element defines a section that is quoted from another source. Browsers usually indent `<blockquote>` elements.
* The HTML `<address>` element defines contact information (author/owner) of a document or an article. The `<address>` element is usually displayed in italic.
* The HTML `<abbr>` element defines an abbreviation or an acronym.
* The HTML `<bdo>` element defines bi-directional override. The `<bdo>` element is used to override the current text direction.

```
<!DOCTYPE html>
<html>
    <head>
        <title>HTML Elements Cont..</title>
    </head>
    <body>
    <h1>More Elements</h1>
     
    <p>Here is a quote: <q>Inspirational quote would go right here.</q></p>
        
    <p><cite>This Course</cite> by Andrew Eddy. Taugh in 2015.</p>
        
    <p>Here is a quote by Andrew Eddy:</p>
    
    <blockquote cite="http://www.udemy.com">
    Every time i type words. I hope that I wont have
    to type to many  more. A quote is but a persons 
    imagination laid out in words and feelings.
    </blockquote>
        
<address>
Written by Andrew Eddy.<br> 
Visit us at:<br>
udemy.com<br>
3766, Ausland<br>
USA
</address>
        
    <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
        
    <bdo dir="rtl">This text will be written from right to left</bdo>

    </body>
</html>
```
## HTML Comment
*  Add comments to the HTML source by using the following syntax:

    `<!-- Write your comments here -->`

* Comments are not displayed in the browser, but they can help document our HTML source code.
<a href="#C0">Top</a>
<h2 id="C3">HTML Links</h2>

* HTML links are hyperlinks.
* You can click on a link and jump to another document.
### link.html
```
<!DOCTYPE html>
<html>
<head>
<title>This is a title</title>    
</head>
<body>
<h1>Lets Play with Links</h1>   
<a href="link1.html" target="_blank">Go to Link Page</a>
</body>
</html>
```
### link1.html
```
<!DOCTYPE html>
<html>
<head>
<title>This is a title</title>    
</head>
<body>
<h1>Lets Play with Links</h1>   
<a href="http://www.google.com" title="goto Google Page" target="_blank">Google</a>
</body>
</html>
```
* title attribute is a tooltip text when the mouse moves over the element.
### The target Attribute
* The target attribute specifies where to open the linked document.

* The target attribute can have one of the following values:

    * _blank - Opens the linked document in a new window or tab
    * _self - Opens the linked document in the same window/tab as it was clicked (this is default)
    * _parent - Opens the linked document in the parent frame
    * _top - Opens the linked document in the full body of the window

### HTML Links - Create a Bookmark
* HTML bookmarks are used to allow readers to jump to specific parts of a Web page.

* Bookmarks can be useful if a webpage is very long.
    * create a bookmark with the id attribute:
        * `<h2 id="C1">Chapter 1</h2>`
    * Add a link to the bookmark ("Jump to Chapter 1"), from within the same page:
        * `<a href="#C1">Jump to Chapter 1</a>`

<a href="#C0">Top</a>   
<h2 id="C4">HTML Lists </h2>

* Unordered List
* Ordered List
* Description List
### Unordered List
```
<ul>
    <li>Laddu</li>
    <li>Mysore Pak</li>
    <li>Burfi</li>
</ul>
```
* CSS `list-style-type` property is used to define the style of the list item marker:
    * disc - Sets the list item marker to a bullet (default)
    * circle - Sets the list item marker to a circle
    * square - Sets the list item marker to a square
    * none - 
    The list items will not be marked

```
<ul style="list-style-type:disc;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
### Ordered List
* type="1"	The list items will be numbered with numbers (default)
* type="A"	The list items will be numbered with uppercase letters
* type="a"	The list items will be numbered with lowercase letters
* type="I"	The list items will be numbered with uppercase roman numbers
* type="i"	The list items will be numbered with lowercase roman numbers
```
<ol type="a" start =5>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
### Description List
```
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
<h2 id="C5">HTML Tables</h2>

```html
<table border="1">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th> 
    <th>Age</th>
  </tr>
  <tr>
    <td>Swetha</td>
    <td>Barath</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Nalini</td>
    <td>Sampath</td>
    <td>94</td>
  </tr>
  <tr>
    <td>Shivani</td>
    <td>Rai</td>
    <td>80</td>
  </tr>
</table>
```
<a href="#C0">Top</a>
<h2 id="C6">Div and Span</h2> 

### Div(Block Element)
* The `<div>` tag defines a division or a section in an HTML document.
* By default, browsers always place a line break before and after the `<div>`
### Span(Inline Element)
 * Don't start with new line
 * Manipulate style of text
 ```
 <div style="background-color: azure; color: black">This is my first div</div>
<div style="background-color: blue; color: white">This is my second div</div>
<h2>This is <span style="color: blue">blue</span> header</h2>

 ```
 <a href="#C0">Top</a>
<h2 id="C7">Class and Id</h2> 

* HTML element can only have one unique id that belongs to that single element
* Class can be used by multiple elements
```html
<!DOCTYPE html>
<html>
<head>
<title>ID and Class Page</title>

<style>
    #main-navigation {
        color: brown;   
    }
    h1 {
     color: aqua;   
    }
    .headerone {
        color: blueviolet;
        text-decoration:line-through;
    }
    .headergreen {
        color: green;
        text-decoration: underline;
    }
</style>
</head>
<body>

<div id="main-navigation"><ul>
    <li>Home</li>
    <li>About</li>
    <li>Contact</li>
    
    </ul></div>

<h1 class="headerone">Header One</h1>
<h2 class="headerone">Header One</h2>
<h3 class="headerone">Header One</h3>
<h4 class="headerone">Header One</h4>

<h3 class="headergreen">Header Green</h3>
<h2 class="headergreen">Header Green</h2>
<h1 class="headergreen">Header Green</h1>

</body>
</html>
```

<a href="#C0">Top</a>
<h2 id="C8">Forms</h2>

* HTML `<form>` element defines a form that is used to collect user input
* Form elements are different types of input elements, like: text fields, checkboxes, radio buttons, submit buttons, and more.
```html
<!DOCTYPE html>
<html>
<head>
<title>HTML Form</title>
</head>
<body>

<form>
<label for="firstname">First Name:</label>
<input type="text" name="firstname" placeholder="First Name"> <br><br>
<label for="lastname">Last Name:</label>
<input type="text" name="lastname" placeholder="Last Name"><br><br>
<textarea name="content"></textarea> <br>
<p>Select your favorite fruit.</p>
<select name="fruit">
    <option value="apple">Apple</option>
    <option value="apple">Strawberry</option>
    <option value="apple">Kiwi</option>
    <option value="apple">Watermelon</option>
</select>
<br><br>
<input type="submit"> 
</form>

</body>
</html>
```
<a href="#C0">Top</a>

