# HTML Interview Questions with Answers

<img src="./images/html5.jpg" width="800">

## Table of Contents

|No.| Questions            |
|----|------------------------------------|
| 1.|[What is the DOM? How does the DOM work?](#what-is-the-dom-how-does-the-dom-work)|
| 2.|[How does the browser rendering engine work?](#how-does-the-browser-rendering-engine-work)|
| 3.|[What does a `<DOCTYPE html>` do?](#what-does-a-doctype-html-do)|
| 4.|[What happens when DOCTYPE is not given?](#what-happens-when-doctype-is-not-given)|
| 5.|[What is the difference between standards mode and quirks mode?](#what-is-the-difference-between-standards-mode-and-quirks-mode)|
| 6.|[What are the building blocks of HTML5?](#what-are-the-building-blocks-of-html5)|
| 7.|[Describe the difference between a `cookie`, `sessionStorage` and `localStorage`?](#describe-the-difference-between-a-cookie-sessionstorage-and-localstorage)|
| 8.|[What is Critical Rendering Path?](#what-is-critical-rendering-path)|
| 9.|[What are the Benefits of Server Side Rendering (SSR) Over Client Side Rendering (CSR)?](#what-are-the-benefits-of-server-side-rendering-ssr-over-client-side-rendering-csr)|
| 10.|[What is the difference between a `<span>` and a `<div>`?](#what-is-the-difference-between-a-span-and-a-div)|
| 11.|[Name 5 common block-level and inline HTML elements?](#name-5-common-block-level-and-inline-html-elements)|
| 12.|[What are semantic and non-semantic elements?](#what-are-semantic-and-non-semantic-elements)|
| 13.|[What is the purpose of `main` element?](#what-is-the-purpose-of-main-element)|
| 14.|[Define semantic markup. What are the semantic meanings for `<section>, <article>, <aside>, <nav>, <header>, <footer>` and when/how should each be used in structuring html markup?](#define-semantic-markup-what-are-the-semantic-meanings-for-section-article-aside-nav-header-footer-and-when-how-should-each-be-used-in-structuring-html-markup)|
| 15.|[When should you use `section`, `div` or `article`?](#when-should-you-use-section-div-or-article)|
| 16.|[What is the purpose of meta tags?](#what-is-the-purpose-of-meta-tags)|
| 17.|[What does async and defer refer in script tag? Describe the difference between `<script>`, `<script async>` and `<script defer>`](#what-does-async-and-defer-refer-in-script-tag-describe-the-difference-between-script-script-async-and-script-defer)|
| 18.|[Can you describe the difference between progressive enhancement and graceful degradation?](#can-you-describe-the-difference-between-progressive-enhancement-and-graceful-degradation)|
| 19.|[What is the purpose of cache busting and how can you achieve it?](#what-is-the-purpose-of-cache-busting-and-how-can-you-achieve-it)|
| 20.|[Name 3 ways to decrease page load?](#name-3-ways-to-decrease-page-load)|
| 21.|[What ARIA and screenreaders are, and how to make a website accessible?](#what-aria-and-screenreaders-are-and-how-to-make-a-website-accessible)|
| 22.|[What is the purpose of the `alt` attribute on images?](#what-is-the-purpose-of-the-alt-attribute-on-images)|
| 23.|[Explain some of the pros and cons for CSS animations versus JavaScript animations?](#explain-some-of-the-pros-and-cons-for-css-animations-versus-javascript-animations)|
| 24.|[What does CORS stand for and what issue does it address?](#what-does-cors-stand-for-and-what-issue-does-it-address)|
| 25.|[Ways to improve website performance](#ways-to-improve-website-performance)|
| 26.|[Comparison of browsers engines like Chrome, Firefox, Internet explorer, Safari?](#comparison-of-browsers-engines-like-chrome-firefox-internet-explorer-safari)|
| 27.|[What does the lang attribute in html do?](#what-does-the-lang-attribute-in-html-do)|
| 28.|[What is desktop first and mobile first design approach?](#what-is-desktop-first-and-mobile-first-design-approach)|
| 29.|[What are `data-` attributes good for?](#what-are-data-attributes-good-for)|
| 30.|[Explain the difference between layout, painting and compositing?](#explain-the-difference-between-layout-painting-and-compositing)|
| 31.|[Explain about HTML Canvas?](#explain-about-html-canvas)|
| 32.|[Explain about HTML Layout Engines used by browsers?](#explain-about-html-layout-engines-used-by-browsers)|
| 33.|[What are the semantic tags available in html5?](#what-are-the-semantic-tags-available-in-html5)|
| 34.|[Why you would like to use semantic tag?](#why-you-would-like-to-use-semantic-tag)|
| 35.|[How to make page responsive?](#how-to-make-page-responsive)|
| 36.|[What are optional closing tag?](#what-are-optional-closing-tag)|
| 37.|[What is a self closing tag?](#what-is-a-self-closing-tag)|
| 38.|[Does the following trigger http request at the time of page load?](#does-the-following-trigger-http-request-at-the-time-of-page-load)|
| 39.|[How Geo-location API works in html5?](#how-geo-location-api-works-in-html5)|
| 40.|[What is difference between SVG and Canvas?](#what-is-difference-between-svg-and-canvas)|
| 41.|[Explain Drag and Drop in HTML5?](#explain-drag-and-drop-in-html5)|
| 42.|[Explain Application Cache in HTML5. OR What is a manifest file in HTML?](#explain-application-cache-in-html5-or-what-is-a-manifest-file-in-html)|
| 43.|[Explain Microdata in HTML5?](#explain-microdata-in-html5)|
| 44.|[List the API available in HTML5?](#list-the-api-available-in-html5)|
| 45.|[What are different new form element types provided by HTML5?](#what-are-different-new-form-element-types-provided-by-html5)|
| 46.|[How you can Use Modernizr in HTML5?](#how-you-can-use-modernizr-in-html5)|
| 47.|[What is the use of WebSocket API?](#what-is-the-use-of-websocket-api)|

## What is the DOM? How does the DOM work?

The DOM (Document Object Model) is a cross-platform API that treats HTML documents as a tree structure consisting of nodes. These nodes (such as elements and text nodes) are objects that can be programmatically manipulated and any visible changes made to them are reflected live in the document. In a browser, this API is available to JavaScript where DOM nodes can be manipulated to change their styles, contents, placement in the document, or interacted with through event listeners.

* The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API.

* document.getElementById() and document.querySelector() are common functions for selecting DOM nodes.

* Setting the innerHTML property to a new value runs the string through the HTML parser, offering an easy way to append dynamic HTML content to a node.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## How does the browser rendering engine work?

In order to render content the browser has to go through a series of steps:

* Document Object Model(DOM)
* CSS object model(CSSOM)
* Render Tree
* Layout
* Paint

<img src="./images/layers.png" alt="Browser Rendering Engine" />

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What does a `<DOCTYPE html>` do? 

A DOCTYPE is always associated to a `DTD` ( **Document Type Definition** ). A DTD defines how documents of a certain type should be structured (i.e. a `button` can contain a `span` but not a `div`), whereas a DOCTYPE declares what DTD a document supposedly respects (i.e. this document respects the HTML DTD). For webpages, the DOCTYPE declaration is required. It is used to tell user agents what version of the HTML specifications your document respects. 

Once a user agent has recognized a correct DOCTYPE, it will trigger the `no-quirks mode` matching this DOCTYPE forreading the document. If a user agent doesn't recognize a correct DOCTYPE, it will trigger the `quirks mode`.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What happens when DOCTYPE is not given? 

The web page is rendered in quirks mode. The web browsers engines use quirks mode to support older browsers which does not follow the **W3C specifications**. In quirks mode CSS class and id names are case insensitive. In standards mode they are case sensitive.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is the difference between standards mode and quirks mode? 

In **Quirks mode**, layout emulates nonstandard behavior in Navigator 4 and Internet Explorer 5. This is essential in order to support websites that were built before the widespread adoption of web standards. In **Standards mode**, the behavior is described by the HTML and CSS specifications. 

For HTML documents, browsers use a `<!DOCTYPE html>` in the beginning of the document to decide whether to handle it in quirks mode or standards mode. 
```html
<!DOCTYPE html>
<html lang="en">
 <head>
  <meta charset=UTF-8>
  <title>Hello World!</title>
 </head>
 <body>
 </body>
</html>
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What are the building blocks of HTML5? 

* **Semantics**: allowing you to describe more precisely what your content is.
* **Connectivity**: allowing you to communicate with the server in new and innovative ways.
* **Offline and storage**: allowing webpages to store data on the client-side locally and operate offline more efficiently.
* **Multimedia**: making video and audio first-class citizens in the Open Web.
* **2D/3D graphics and effects**: allowing a much more diverse range of presentation options.
* **Performance and integration**: providing greater speed optimization and better usage of computer hardware.
* **Device access**: allowing for the usage of various input and output devices.
* **Styling**: letting authors write more sophisticated themes.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Describe the difference between a `cookie`, `sessionStorage` and `localStorage`? 

* ```cookie```: A text file saved on the users computer to store and retrieve data

* ```sessionStorage```: Is memory space in a browser to save temporary data until the window or tab is closed.

* ```localStorage```: Like cookie, where data can be saved and retrieved after browser sessions, but stored in memory like sessionStorage. Data is stored as plain key value pairs and can be stored as Json objects.

|                    | `cookie`                         | `localStorage` | `sessionStorage` |
| -------------------------------------- | -------------------------------------------------------- | -------------- | ---------------- |
| Initiator               | Client or server. Server can use `Set-Cookie` header   | Client     | Client      |
| Expiry                 | Manually set                       | Forever    | On tab close   |
| Persistent across browser sessions   | Depends on whether expiration is set           | Yes      | No        |
| Sent to server with every HTTP request | Cookies are automatically being sent via `Cookie` header | No       | No        |
| Capacity (per domain)         | 4kb                           | 5MB      | 5MB       |
| Accessibility             | Any window                        | Any window   | Same tab     |


*Note: If the user decides to clear browsing data via whatever mechanism provided by the browser, this will clear out any `cookie`, `localStorage`, or `sessionStorage` stored. It's important to keep this in mind when designing for local persistance, especially when comparing to alternatives such as server side storing in a database or similar (which of course will persist despite user actions).*

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is Critical Rendering Path? 

* Constructing the DOM Tree
* Constructing the CSSOM Tree
* Running JavaScript - parser blocking resource
* Creating the Render Tree
* Generating the Layout
* Painting

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What are the Benefits of Server Side Rendering (SSR) Over Client Side Rendering (CSR)? 

* We are using server side rendering for two reasons:
  * performance benefit for our customers
  * Consistent SEO performance

* The main difference is that for SSR your server???s response to the browser is the HTML of your page that is ready to be rendered, while for CSR the browser gets a pretty empty document with links to your javascript. That means for SSR your browser will start rendering the HTML from your server without having to wait for all the JavaScript to be downloaded and executed.
  
* for SSR, the user can start viewing the page while all of that is happening. For the CSR world, you need to wait for all of the above to happen and then have the virtual dom moved to the browser dom for the page to be viewable.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is the difference between a `<span>` and a `<div>`? 

* `<div>` is a block level element which means it will render it on it's own line with a width of a 100% of the parent element.
* `<span>` is an inline element which means it will render on the same line as the previous element, if it is also an inline element, and it's width will be determined by it's content.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Name 5 common block-level and inline HTML elements? 

* block elements `<h1>, <p>, <ul>, <ol>, <li>`,
* inline elements `<span>, <a>, <strong>, <i>, <img>`

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What are semantic and non-semantic elements? 

* **Semantic elements**: clearly describes its meaning to both the browser and the developer. For example: `<form>`, `<table>`, `<article>`, `<aside>`, `<details>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<section>`, `<summary>`, `<time>` clearly defines its content.
 
* **Non-semantic elements**: `<div>` and `<span>` tells nothing about its content. 

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is the purpose of `main` element? 

The HTML `<main>` element represents the dominant content of the `<body>` of a document. The main content area consists of content that is directly related to or expands upon the central topic of a document, or the central functionality of an application.

```html
<main role="main">
  <p>Geckos are a group of usually small, usually nocturnal lizards. 
    They are found on every continent except Australia.</p>
  <p>Many species of gecko have adhesive toe pads which enable them to climb walls and even windows.</p>
</main>
```

*Note: A document mustn\'t have more than one `<main>` element that doesn't have the hidden attribute specified.*

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Define semantic markup. What are the semantic meanings for `<section>, <article>, <aside>, <nav>, <header>, <footer>` and when/how should each be used in structuring html markup? 

* `<header>` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author???s name, time and date of publication, table of contents, or other navigational information.

* `<article>` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing it???s meaining. Individual blog posts or news stories are good examples.

* `<section>` is a flexible container for holding content that shares a common informational theme or purpose.

* `<footer>` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author???s name, copyright information, and related links are typical examples of such content.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## When should you use `section`, `div` or `article`? 

* `<section>`, group of content inside is related to a single theme, and should appear as an entry in an outline of the page. It???s a chunk of related content, like a subsection of a long article, a major part of the page (eg the news section on the homepage), or a page in a webapp???s tabbed interface. A section normally has a heading (title) and maybe a footer too.

* `<article>`, represents a complete, or self-contained, composition in a document, page, application, or site and that is, in principle, independently distributable or reusable, e.g. in syndication. This could be a forum post, a magazine or newspaper article, a blog entry, a user-submitted comment, an interactive widget or gadget, or any other independent item of content.

* `<div>`, on the other hand, does not convey any meaning, aside from any found in its class, lang and title attributes.

```html
<meta charset="utf-8"/>
```

* **UTF-8**: A Unicode Translation Format that comes in 8-bit units that is, it comes in bytes. A character in UTF8 can be from 1 to 4 bytes long, making UTF8 variable width.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is the purpose of meta tags? 

The META elements can be used to include name/value pairs describing properties of the HTML document, such as author, expiry date, a list of keywords, document author etc.

```html
<!DOCTYPE html>
<html>
 <head>
    <!--Recommended Meta Tags-->
    <meta charset="utf-8">
    <meta name="language" content="english"> 
    <meta http-equiv="content-type" content="text/html">
    <meta name="author" content="Author Name">
    <meta name="designer" content="Designer Name">
    <meta name="publisher" content="Publisher Name">
    <meta name="no-email-collection" content="name@email.com">
    <meta http-equiv="X-UA-Compatible" content="IE=edge"/>

    <!--Search Engine Optimization Meta Tags-->
    <meta name="description" content="Project Description">
    <meta name="keywords" content="Software Engineer,Product Manager,Project Manager,Data Scientist">
    <meta name="robots" content="index,follow">
    <meta name="revisit-after" content="7 days">
    <meta name="distribution" content="web">
    <meta name="robots" content="noodp">
    
    <!--Optional Meta Tags-->
    <meta name="distribution" content="web">
    <meta name="web_author" content="">
    <meta name="rating" content="">
    <meta name="subject" content="Personal">
    <meta name="title" content=" - Official Website.">
    <meta name="copyright" content="Copyright 2020">
    <meta name="reply-to" content="">
    <meta name="abstract" content="">
    <meta name="city" content="Bangalore">
    <meta name="country" content="INDIA">
    <meta name="distribution" content="">
    <meta name="classification" content="">
  
    <!--Meta Tags for HTML pages on Mobile-->
    <meta name="format-detection" content="telephone=yes"/>
    <meta name="HandheldFriendly" content="true"/> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/> 
    <meta name="apple-mobile-web-app-capable" content="yes" />
    
    <!--http-equiv Tags-->
    <meta http-equiv="Content-Style-Type" content="text/css">
    <meta http-equiv="Content-Script-Type" content="text/javascript">
   
  <title>HTML5 Meta Tags</title>
 </head>
 <body>
    ...
 </body>
</html>
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What does async and defer refer in script tag? Describe the difference between `<script>`, `<script async>` and `<script defer>` 

* **Async**: Downloads the script file during HTML parsing and will pause the HTML parser to execute it when it has finished downloading.

* **Defer**: Defer downloads the script file during HTML parsing and will only execute it after the HTML parser has completed. Not all browsers support this.
  
The async attribute is used to indicate to the browser that the script file can be executed asynchronously. The HTML parser does not need to pause at the point it reaches the script tag to fetch and execute, the execution can happen whenever the script becomes ready after being fetched in parallel with the document parsing.

The defer attribute tells the browser to only execute the script file once the HTML document has been fully parsed.   

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Can you describe the difference between progressive enhancement and graceful degradation? 

* Graceful degradation is when you initially serve the best possible user experience, with all modern functionality, but use feature detection to ???gracefully degrade??? parts of your application with a fallback or polyfill.

* Progressive enhancement ensures a page works at the lowest expected abilities of browsers. So if you have a JavaScript web application that enhances a persons ability to send information to a database with features like ajax ??? at the very least you need to provide the ability for a person to send that same information without JavaScript enabled. In this case a simple form with full-page refresh will do what you need.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is the purpose of cache busting and how can you achieve it? 

Browsers have a cache to temporarily store files on websites so they don't need to be re-downloaded again when switching between pages or reloading the same page. The server is set up to send headers that tell the browser to store the file for a given amount of time. This greatly increases website speed and preserves bandwidth.

However, it can cause problems when the website has been changed by developers because the user's cache still references old files. This can either leave them with old functionality or break a website if the cached CSS and JavaScript files are referencing elements that no longer exist, have moved or have been renamed.

**Cache busting** is the process of forcing the browser to download the new files. This is done by naming the file something different to the old file.

A common technique to force the browser to re-download the file is to append a query string to the end of the file.

```html
<!-- src="js/script.js" => src="js/script.js?v=2" -->
<script src="js/script.js?v=2"></script>
```

The browser considers it a different file but prevents the need to change the file name.  

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Name 3 ways to decrease page load? 

1. LocalStorage 
1. Caching resources 
1. DNS-prefetch (sample below) 
1. Keep resources on a CDN

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What ARIA and screenreaders are, and how to make a website accessible? 

Screen readers are software programs that provide assistive technologies that allow people with disabilities (such as no sight, sound or mouse-ing ability) to use web applications. You can make your sites more accessible by following ARIA standards such as semantic HTML, alt attributes and using [role=button] in the expected ways

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is the purpose of the `alt` attribute on images? 

The `alt` attribute provides alternative information for an image if a user cannot view it. The `alt` attribute should be used to describe any images except those which only serve a decorative purposes, in which case it should be left empty.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Explain some of the pros and cons for CSS animations versus JavaScript animations? 

Regarding optimization and responsiveness the debate bounces back and forth but, the concept is:

* CSS animations allows the browser to choose where the animation processing is done, CPU or the GPU. (Central or Graphics Processing Unit)

* That said, adding many layers to a document will eventually have a performance hit.

* JS animation means more code for the user to download and for the developer to maintain.

* Applying multiple animation types on an element is harder with CSS since all transforming power is in one property transform

* CSS animations being declarative are not programmable therefore limited in capability.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What does CORS stand for and what issue does it address? 

Cross-Origin Resource Sharing (CORS) is a W3C spec that allows cross-domain communication from the browser. By building on top of the XMLHttpRequest object, CORS allows developers to work with the same idioms as same-domain requests. CORS gives web servers cross-domain access controls, which enable secure cross-domain data transfers.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Ways to improve website performance 

* Minimize HTTP Requests
  * Sites are mainly slow because of too many (or too large) HTTP requests. We can eliminate unnecessary request;
    * combined files: js to a file, css to a file
    * CSS sprites: CSS Sprites are the preferred method for reducing the number of image requests. Combine your background images into a single image and use the CSS background-image and background-position properties to display the desired image segment.

* Use a Content Delivery Network CDN

  * A CDN is essentially many optimized servers around the world that deliver web content to users based on their geographic location. This means big performance improvements for site users. Because, say, if a person accessing your site in India, they will be retrieving web content from a server nearby

* Optimize Images:

  * image sizes make a huge difference to site speed. The larger content/images, the slower the site. we could:
    * Changing the resolution: reducing the ???quality??? of the image (and thereby the file size)
    * Compressing the picture: increasing the efficiency of image data storage
    * Cropping the picture: when cropping, you are cutting out unneeded areas and thus making the image smaller in size

* Put Scripts at the Bottom:

  * Javascript files can load after the rest of your page. The simplest solution is to place your external Javascript files at the bottom of your page, just before the close of your body tag. Now more of your site can load before your scripts. Another method that allows even more control is to use the defer or async attributes when placing external .js files on your site.
    
    * Async tags load the scripts while the rest of the page loads, but this means scripts can be loaded out of order. Basically, lighter files load first. This might be fine for some scripts, but can be disastrous for others.
    
    * The defer attribute loads your scripts after your content has finished loading. It also runs the scripts in order. Just make sure your scripts run so late without breaking your site.

* Add an Expires or a Cache-Control Header

  * Web page designs are getting richer and richer, which means more scripts, stylesheets, images, and Flash in the page. A first-time visitor to your page may have to make several HTTP requests, but by using the Expires header you make those components cacheable. This avoids unnecessary HTTP requests on subsequent page views. Expires headers are most often used with images, but they should be used on all components including scripts, stylesheets, and Flash components.

* Gzip Components

  * Compression reduces response times by reducing the size of the HTTP response. Gzipping generally reduces the response size by about 70%.

* Put Stylesheets at the Top:

  * This is because putting stylesheets in the HEAD allows the page to render progressively.

* Avoid CSS Expressions

* Use GET for AJAX Requests:

  * Ajax is that it provides instantaneous feedback to the user because it requests information asynchronously from the backend web server

* Make JavaScript and CSS External:

  * Using external files in the real world generally produces faster pages because the JavaScript and CSS files are cached by the browser. JavaScript and CSS that are inlined in HTML documents get downloaded every time the HTML document is requested. This reduces the number of HTTP requests that are needed, but increases the size of the HTML document. On the other hand, if the JavaScript and CSS are in external files cached by the browser, the size of the HTML document is reduced without increasing the number of HTTP requests.

* Use get to ajax request:

  * POST is implemented in the browsers as a two-step process: sending the headers first, then sending data. So it's best to use GET, which only takes one TCP packet to send (unless you have a lot of cookies).

* No 404s:

  * HTTP requests are expensive so making an HTTP request and getting a useless response (i.e. 404 Not Found) is totally unnecessary and will slow down the user experience without any benefit.

* Reduce Cookie Size:

  * HTTP cookies are used for a variety of reasons such as authentication and personalization. Information about cookies is exchanged in the HTTP headers between web servers and browsers. It's important to keep the size of cookies as low as possible to minimize the impact on the user's response time.

* Reduce DNS Lookups
* Minify JavaScript and CSS
* Avoid Redirects
* Remove Duplicate Scripts
* Configure Etags
* Make Ajax Cacheable
* Post-load Components
* Preload Components
* Reduce the Number of DOM Elements
* Minimize the Number of iframes
* Minimize DOM Access
* Optimize CSS Sprites
* Don't Scale Images in HTML
* Make favicon.ico Small and Cacheable
* Avoid Empty Image src

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Comparison of browsers engines like Chrome, Firefox, Internet explorer, Safari? 

* Chrome: 
  * Layout rendering engine **Webkit**. 
  * JavaScript engine **V8**

* Firefox: 
  * Layout rendering engine **Gecko**. 
  * JavaScript engine **Spider monkey**
    
* Internet explorer: 
  * Layout rendering engine **Trident**. 
  * JavaScript engine **Chakra**
    
* Safari:
  * Layout rendering engine **Webkit**. 
  * JavaScript engine JavascriptCore i.e **Nitro**

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What does the lang attribute in html do? 

* Helps in styling pages by using them in css :lang() pseudo class Spelling and grammar checkers Languade detection by search engines

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is desktop first and mobile first design approach? 

* Desktop first : 
    General selectors and styles designed to make the site look good on DESKTOP screens defined globally. But they affect all devices, and must be overridden by max-width media queries targeting minimum screen size

* Mobile First : 
    General selectors and styles designed to make the site look good on small MOBILE screens go here. But they affect all devices, and must be overridden by min-width media queries targeting maximum scrren size
  
  In desktop first approach the media queries will be written with respect to max-width whereas in mobile first approach media queries will be written with respect to min-width

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What are `data-` attributes good for? 

* The HTML5 data attribute lets you assign custom data to an element. When we want to store more information/data about the element when no suitable HTML5 element or attribute exists

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Explain the difference between layout, painting and compositing? 

<img src="lib/img/frame-full.jpg" alt="Browser Engine" />

* **JavaScript**: Typically JavaScript is used to handle work that will result in visual changes, whether it???s jQuery???s animate function, sorting a data set, or adding DOM elements to the page. It doesn???t have to be JavaScript that triggers a visual change, though: CSS Animations, Transitions, and the Web Animations API are also commonly used.
* **Style calculations**: This is the process of figuring out which CSS rules apply to which elements based on matching selectors, for example, .headline or .nav > .nav__item. From there, once rules are known, they are applied and the final styles for each element are calculated.
* **Layout**: Once the browser knows which rules apply to an element it can begin to calculate how much space it takes up and where it is on screen. The web???s layout model means that one element can affect others, for example the width of the <body> element typically affects its children???s widths and so on all the way up and down the tree, so the process can be quite involved for the browser.
* **Paint**: Painting is the process of filling in pixels. It involves drawing out text, colors, images, borders, and shadows, essentially every visual part of the elements. The drawing is typically done onto multiple surfaces, often called layers.
* **Compositing**: Since the parts of the page were drawn into potentially multiple layers they need to be drawn to the screen in the correct order so that the page renders correctly. This is especially important for elements that overlap another, since a mistake could result in one element appearing over the top of another incorrectly.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Explain about HTML Canvas?  

**canvas** is an HTML element which can be used to draw graphics via JavaScript. This can, for instance, be used to draw graphs, combine photos, or create animations.

**Colors, Styles, and Shadows**

| Property  |	Description                                 |
|--------------|--------------------------------------------------------------------------------|
|fillStyle	  | Sets or returns the color, gradient, or pattern used to fill the drawing    |
|strokeStyle  | Sets or returns the color, gradient, or pattern used for strokes        |
|shadowColor  | Sets or returns the color to use for shadows                  |
|shadowBlur	  | Sets or returns the blur level for shadows                   |
|shadowOffsetX | Sets or returns the horizontal distance of the shadow from the shape      |
|shadowOffsetY | Sets or returns the vertical distance of the shadow from the shape       |


**Line Styles**

|Property	 | Description                          |
|------------|----------------------------------------------------------------|
|lineCap	 |Sets or returns the style of the end caps for a line      |
|lineJoin	 |Sets or returns the type of corner created, when two lines meet |
|lineWidth	 |Sets or returns the current line width             |
|miterLimit	 |Sets or returns the maximum miter length            |


**Rectangles**
 
|Method	    |Description                     |
|---------------|-----------------------------------------------------|
|rect()	    |Creates a rectangle                 |
|fillRect()	  |Draws a "filled" rectangle              |
|strokeRect()	|Draws a rectangle (no fill)             |
|clearRect()	|Clears the specified pixels within a given rectangle |


**Paths**
  
| Method	   |  Description                                         |
|-----------------|---------------------------------------------------------------------------------------------- |
|fill()	     |Fills the current drawing (path)                                |
|stroke()	   |Actually draws the path you have defined                            |
|beginPath()	 |Begins a path, or resets the current path                           |
|moveTo()	   |Moves the path to the specified point in the canvas, without creating a line          |
|closePath()	 |Creates a path from the current point back to the starting point                |
|lineTo()	   |Adds a new point and creates a line to that point from the last specified point in the canvas |
|clip()	     |Clips a region of any shape and size from the original canvas                 |
|arc()	     |Creates an arc/curve (used to create circles, or parts of circles)               |
|arcTo()	   |Creates an arc/curve between two tangents                           |
 

**Transformations**
  
|Method	    |Description                                |
|---------------|-------------------------------------------------------------------------- |
|scale()	  |Scales the current drawing bigger or smaller                |
|rotate()	  |Rotates the current drawing                        |
|translate()	|Remaps the (0,0) position on the canvas                  |
|transform()	|Replaces the current transformation matrix for the drawing         |
|setTransform()	|Resets the current transform to the identity matrix. Then runs transform() |
 

**Text**
  
|Property	  |Description                            |
|---------------|----------------------------------------------------------------- |
|font	    |Sets or returns the current font properties for text content   |
|textAlign	  |Sets or returns the current alignment for text content      |
|textBaseline	|Sets or returns the current text baseline used when drawing text |
|fillText()	  |Draws "filled" text on the canvas                 |
|strokeText()	|Draws text on the canvas (no fill)                |
|measureText()	|Returns an object that contains the width of the specified text  |

[Live Example](canvas.html) 

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Explain about HTML Layout Engines used by browsers? 

|Engine	   |Status	    |Embedded in                                      |
|-------------|-----------------|--------------------------------------------------------------------------------------|
|WebKit	   |Active	    |Safari browser, plus all browsers hosted on the iOS App Store             |
|Blink	   |Active	    |Google Chrome and all other Chromium-based browsers like Opera and Microsoft Edge   |
|Gecko	   |Active	    |Firefox browser and Thunderbird email client, plus forks like SeaMonkey and Waterfox |
|KHTML	   |Discontinued	 |Konqueror browser                                   |
|Presto	   |Discontinued	 |formerly in the Opera browser                             |
|EdgeHTML	 |Discontinued	 |formerly in the Microsoft Edge browser                        |
|Trident	 |Discontinued	 |Internet Explorer browser and Microsoft Outlook email client             |

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What are the semantic tags available in html5? 

HTML5 semantic tags define the function and the category of your text, simplifying the work for browsers and search engines, as well as developers.

HTML5 offers new semantic elements to define different parts of a web page:

* `<article>`
* `<aside>`
* `<details>`
* `<figcaption>`
* `<figure>`
* `<footer>`
* `<header>`
* `<main>`
* `<mark>`
* `<nav>`
* `<section>`
* `<summary>`
* `<time>`

Syntax:
```html
<header></header>
<section>
	<article>
		<figure>
			<img>
			<figcaption></figcaption>
		</figure>
	</article>
</section>
<footer></footer>
```
*Example:* [HTML5 Semantic Tags](semantic-tags.html)

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Why you would like to use semantic tag? 

* Search Engine Optimization, accessibility, repurposing, light code. 
* Many visually impaired person rely on browser speech and semantic tag helps to interpret page content clearly.
* Search engine needs to understand page content to rank and semantic tag helps.
* Semantic code aids accessibility. Specially, many people whose eyes are not good rely on speech browsers to read pages to them. These programs cannot interpret pages very well unless they are clearly explained.
* Help Search engines to better understand pages. Search engine need to understand what your content is about when rank you properly on search engines. Semantic code tends to improve your placement on search engines, as it is easier for the "search engine spiders" to understand.
* It???s easier to read and edit, which saves time and money during maintenance.

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## How to make page responsive? 

Responsive Web Design is about using HTML and CSS to automatically resize, hide, shrink, or enlarge, a website, to make it look good on all devices (desktops, tablets, and phones).

**1) Setting the viewport** 
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
**2) Responsive Images** 
If the CSS width property is set to 100%, the image will be responsive and scale up and down
```html
<img src="img.png" style="width:100%;">
```
**3) Show different Images depending on Browser Width** 
The HTML `<picture>` element allows you to define different images for different browser window sizes.
```html
<picture>
 <source srcset="img_small.jpg" media="(max-width: 600px)">
 <source srcset="img_large.jpg" media="(max-width: 1500px)">
 <source srcset="img.jpg">
 <img src="img_small.jpg" alt="Image">
</picture>
```
**4) Responsive Text Size** 
The text size can be set with a "vw" unit, which means the "viewport width". That way the text size will follow the size of the browser window.
```html
<h1 style="font-size:10vw">Hello World</h1>
```
**5) Media Queries** 
Using media queries you can define completely different styles for different browser sizes.
```css
/* Use a media query to add a breakpoint at 800px: */
@media screen and (max-width: 800px) {
 .left, .main, .right {
  width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
 }
}
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What are optional closing tag? 

`<p>, <li>, <td>, <tr>, <th>, <html>, <body>`, etc. don't have to provide end tag. Whenever browser hits a new tag it automatically ends the previous tag. 

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is a self closing tag? 

In HTML5 it is not strictly necessary to close certain HTML tags. The tags that aren???t required to have specific closing tags are called ???self closing??? tags.

An example of a self closing tag is something like a line break (`<br />`) or the meta tag (`<meta>`). This means that the following are both acceptable:

```html
<meta charset="UTF-8">
...
<meta charset="UTF-8" />
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Does the following trigger http request at the time of page load? 

```html
<img src="mypic.jpg" style="visibility: hidden" alt="My photo">

<div style="display: none;">
  <img src="mypic.jpg" alt="My photo">
</div>
```
* Yes

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## How Geo-location API works in html5? 

The Geolocation API allows the user to provide their location to web applications if they so desire. For privacy reasons, the user is asked for permission to report location information.

The Geolocation API is published through the `navigator.geolocation` object.
```javascript
if ("geolocation" in navigator) {
 /* geolocation is available */
} else {
 /* geolocation IS NOT available */
}
```

*Example:* [HTML5 Geolocation API](geolocation.html)

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is difference between SVG and Canvas? 

**1.) SVG**: The Scalable Vector Graphics (SVG) is an XML-based image format that is used to define two-dimensional vector based graphics for the web. Unlike raster image (e.g. .jpg, .gif, .png, etc.), a vector image can be scaled up or down to any extent without losing the image quality.

There are following advantages of using SVG over other image formats like JPEG, GIF, PNG, etc.

* SVG images can be searched, indexed, scripted, and compressed.
* SVG images can be created and modified using JavaScript in real time.
* SVG images can be printed with high quality at any resolution.
* SVG content can be animated using the built-in animation elements.
* SVG images can contain hyperlinks to other documents.

*Example:* 
```html
<!DOCTYPE html>
<html>
  <head>
   <style>
     #svgelem {
      position: relative;
      left: 50%;
      -webkit-transform: translateX(-20%);
      -ms-transform: translateX(-20%);
      transform: translateX(-20%);
     }
   </style>
   <title>HTML5 SVG</title>
  </head>
  <body>
   <h2 align="center">HTML5 SVG Circle</h2>
   <svg id="svgelem" height="200" xmlns="http://www.w3.org/2000/svg">
     <circle id="bluecircle" cx="60" cy="60" r="50" fill="blue" />
   </svg>
  </body>
</html>
```
[Live Example](a.svg.html)

**2.) Canvas**: Canvas is a HTML element is used to draw graphics on a web page. It is a bitmap with an ???immediate mode??? graphics application programming interface (API) for drawing on it. The `<canvas>` element is only a container for graphics. In order to draw the graphics, you are supposed to use a script. Canvas has several strategies when it comes to drawing paths, boxes, circles, text & adding images.

*Example:*
```html
<!DOCTYPE html>
<html>
  <head>
   <title>HTML5 Canvas Tag</title>
  </head>
  <body>
   <canvas id="newCanvas" width="200" height="100" style="border:1px solid #000000;"></canvas>
   <script>
     var c = document.getElementById('newCanvas');
     var ctx = c.getContext('2d');
     ctx.fillStyle = '#7cce2b';
     ctx.fillRect(0,0,300,100);
   </script>
  </body>
</html>
```
[Live Example](canvas.html) 

**Differences between SVG and Canvas**  

|SVG	        |Canvas                     |
|-----------------------|-----------------------------------------------|
|Vector based (composed of shapes)	|Raster based (composed of pixel)
|Multiple graphical elements, which become the part of the page's DOM tree|	Single element similar to <img> in behavior. Canvas diagram can be saved to PNG or JPG format|
|Modified through script and CSS	|Modified through script only
|Good text rendering capabilities	|Poor text rendering capabilities
|Give better performance with smaller number of objects or larger surface, or both	|Give better performance with larger number of objects or smaller surface, or both|
|Better scalability. Can be printed with high quality at any resolution. Pixelation does not occur	|Poor scalability. Not suitable for printing on higher resolution. Pixelation may occur |

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Explain Drag and Drop in HTML5? 

HTML5 drag-and-drop uses the `DOM event model` and `drag events` inherited from `mouse events`. A typical drag operation begins when a user selects a draggable element, drags the element to a droppable element, and then releases the dragged element.

|Event	    |Description                              |
|---------------|-----------------------------------------------------------------------|
|Drag	    |It fires every time when the mouse is moved while the object is being dragged.|
|Dragstart	  |It is a very initial stage. It fires when the user starts dragging object.|
|Dragenter	  |It fires when the user moves his/her mouse cursur over the target element.|
|Dragover	  |This event is fired when the mouse moves over an element.|
|Dragleave	  |This event is fired when the mouse leaves an element.|
|Drop	    |Drop It fires at the end of the drag operation.|
|Dragend	  |It fires when user releases the mouse button to complete the drag operation.|

Example
```html
<!DOCTYPE HTML>
<html>
  <head>
  <script>
    function allowDrop(ev) {
      ev.preventDefault();
    }

    function drag(ev) {
      ev.dataTransfer.setData("text", ev.target.id);
    }

    function drop(ev) {
      ev.preventDefault();
      var data = ev.dataTransfer.getData("text");
      ev.target.appendChild(document.getElementById(data));
    }
  </script>
</head>
<body>
 <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
 <img id="drag1" src="img_logo.gif" draggable="true" ondragstart="drag(event)" width="336" height="69">
</body>
</html>
```

[Live Example](drag-drop.html) 

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Explain Application Cache in HTML5. OR What is a manifest file in HTML? 

HTML5 provides an application caching mechanism that lets web-based applications run offline. Developers can use the Application Cache (AppCache) interface to specify resources that the browser should cache and make available to offline users. Applications that are cached load and work correctly even if users click the refresh button when they are offline.

Using an application cache gives an application the following benefits:

* Offline browsing: users can navigate a site even when they are offline.
* Speed: cached resources are local, and therefore load faster.
* Reduced server load: the browser only downloads resources that have changed from the server.

Syntax:
```html
<html manifest="example.appcache">
 ...
</html>
```
[Live Example](application-cache.html) 

*Note: Using the application caching feature described here is at this point highly discouraged; it???s in the process of being removed from the Web platform. Use **Service Workers** instead. In fact as of Firefox 44, when AppCache is used to provide offline support for a page a warning message is now displayed in the console advising developers to use Service workers instead (bug 1204581).*

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## Explain Microdata in HTML5? 

Microdata is a standardized way to provide additional semantics in web pages. Microdata lets you define your own customized elements and start embedding custom properties in your web pages. At a high level, microdata consists of a group of name-value pairs.

The groups are called **items**, and each name-value pair is a **property**. Items and properties are represented by regular elements. Search engines benefit greatly from direct access to this structured data because it allows search engines to understand the information on web pages and provide more 
relevant results to users.

At a high level, microdata consists of a group of name-value pairs
* **itemscope**:- To create an item
* **itemprop**:- To add a property to an item

Example
```html
<div itemscope>
  <p>My name is <span itemprop="name">Elizabeth</span>.</p>
</div>

<div itemscope>
  <p>My name is <span itemprop="name">Daniel</span>.</p>
</div>
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## List the API available in HTML5? 

**1.) High Resolution Time API**   
The High Resolution Time API provides the current time in sub-millisecond resolution and such that it is not subject to system clock skew or adjustments.

It exposes only one method, that belongs to the `window.performance` object, called `now()`. It returns a `DOMHighResTimeStamp` representing the current time in milliseconds. The timestamp is very accurate, with precision to a thousandth of a millisecond, allowing for accurate tests of the performance of our code.
```javascript
var time = performance.now();
```

**2.) User Timing API** 
It allows us to accurately measure and report the performance of a section of JavaScript code. It deals with two main concepts: mark and measure. The former represents an instant (timestamp), while the latter represents the time elapsed between two marks.
```javascript
performance.mark("startFoo");
// A time consuming function
foo();
performance.mark("endFoo");

performance.measure("durationFoo", "startFoo", "endFoo");
```
**3.) Network Information API** 
This API belongs to the connection property of the `window.navigator` object. It exposes two read-only properties: `bandwidth` and `metered`. The former is a number representing an estimation of the current bandwidth, while the latter is a Boolean whose value is true if the user???s connection is subject to limitation and bandwidth usage, and false otherwise.

|Sl.No| API              | Description
|-----|--------------------------------|--------------------------------------------------------------------|
| 01. |navigator.connection.type    |Network Type                |
| 02. |navigator.connection.downlink  |Effective bandwidth estimate ( downlink )                |
| 03. |navigator.connection.rtt    |Effective round-trip time estimate ( rtt )                |
| 04. |navigator.connection.downlinkMax|Upper bound on the downlink speed of the first network hop ( downlinkMax )|      
| 05. |navigator.connection.effectiveType|Effective connection type |
| 06. |navigator.connection.saveData  |True if the user has requested a reduced data usage mode from the user agent ( saveData )|    

**4.) Vibration API** 
It exposes only one method, `vibrate()`, that belongs to the `window.navigator` object. This method accepts one parameter specifying the duration of the vibration in milliseconds. The parameter can be either an integer or an array of integers. In the second case, it???s interpreted as alternating vibration times and pauses.
```javascript
// Vibrate once for 2 seconds
navigator.vibrate(2000);
```

**5.) Battery Status API** 
The Battery Status API exposes four properties (`charging`, `chargingTime`, `discharingTime`, and `level`) and four events. The properties specify if the battery is in charge, the seconds remaining until the battery is fully charged, the seconds remaining until the battery is fully discharged, and the current level of the battery. These properties belongs to the `battery` property of the `window.navigator` object.
```javascript
// Retrieves the percentage of the current level of the device's battery
var percentageLevel = navigator.battery.level * 100;
```

**6.) Page Visibility API** 
The Page Visibility API enables us to determine the current visibility state of the page. The Page Visibility API is especially useful for saving resources and improving performance by letting a page avoid performing unnecessary tasks when the document isn't visible.
```javascript
//document.hidden retuns true if page is not visible.
console.log('Page Visibility: '+document.hidden); 
```
**7.) Fullscreen API** 
The Fullscreen API provides a way to request fullscreen display from the user, and exit this mode when desired. This API exposes two methods, `requestFullscreen()` and `exitFullscreen()`, allowing us to request an element to become fullscreen and to exit fullscreen.
```javascript
document.addEventListener("keypress", function(e) {
  if (e.keyCode === 13) { // Enter Key
    toggleFullScreen();
  }
}, false);

function toggleFullScreen() {
  if (!document.fullscreenElement) {
    document.documentElement.requestFullscreen();
  } else {
    if (document.exitFullscreen) {
    document.exitFullscreen(); 
    }
  }
}
```
*Example:* [HTML5 API](html5-api.html)

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What are different new form element types provided by HTML5? 

|Sl.No| Element   | Description  |
|-----|-------------|---------------------------|
| 01. |color    |Gives the end user a native color picker to choose a color.|
| 02. |date     |Offers a datepicker.|
| 03. |datetime   |An element to choose both date and time.|
| 04. |datetime-local |An element to choose both date and time, with local settings support.|
| 05. |email    |A field for entering e-mail address(es).|
| 06. |month    |Choose a full month.|
| 07. |number    |Picking a number.|
| 08. |range    |Offers a slider to set to a certain value/position.|
| 09. |search    |A field for search queries.|
| 10. |tel     |Choosing a telephone number.|
| 11. |time     |Input a certain time.|
| 12. |url     |Entering a URL.|
| 13. |week     |Picking a specific week.|


*Example:*
```html
<input type="color" value="#b97a57">

<input type="date" value="2020-06-08">

<input type="datetime" value="2020-06-09T20:35:34.32">

<input type="datetime-local" value="2020-06-09T22:41">

<input type="email" value="robert@robertnyman.com">

<input type="month" value="2020-06">

<input type="number" value="4">

<input type="range" value="15">

<!-- Note: If not set, default attribute values are min="0", max="100", step="1". -->

<input type="search" value="[Any search text]">

<input type="tel" value="[Any numeric value]">

<!-- Note: Most web browsers seem to let through any value at this time. -->

<input type="time" value="22:38">

<input type="url" value="https://www.google.com/">

<!-- Note: requires a protocol like http://, ftp:// etc in the beginning. -->


<input type="week" value="2020-W24">
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## How you can Use Modernizr in HTML5? 
Modernizr is a JavaScript library that detects which HTML5 and CSS3 features visitor???s browser supports. In detecting feature support, it allows developers to test for some of the new technologies and then provide fallbacks for browsers that do not support them. This is called **feature detection** and is much more efficient than browser sniffing.

**Using Modernizr with CSS** 
By default, Modernizr sets classes for all of your tests on the root element (`<html>` for websites). This means adding the class for each feature when it is supported, and adding it with a no- prefix when it is not (e.g. `.feature` or `.no-feature`).
```css
.no-cssgradients .header {
 background: url("images/glossybutton.png");
}

.cssgradients .header {
 background-image: linear-gradient(cornflowerblue, rebeccapurple);
}
```
**Using Modernizr with JavaScript** 
Modernizr keeps track of the results of all of it's feature detections via the `Modernizr` object. 
```javascript
if (Modernizr.canvas) {
  alert("This browser supports HTML5 canvas!");
} else {
  alert("no canvas :(");
}
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>

## What is the use of WebSocket API? 

The **WebSocket API** is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. With this API, you can send messages to a server and receive event-driven responses without having to poll the server for a reply.

**Interfaces** 

|Sl.No|  API   | Description  |
|-----|------------|----------------|
| 01. |WebSocket  |The primary interface for connecting to a WebSocket server and then sending and receiving data on the connection.|  
| 02. |CloseEvent |The event sent by the WebSocket object when the connection closes.  |
| 03. |MessageEvent|The event sent by the WebSocket object when a message is received from the server.|  
 
Example
```javascript
 // Create WebSocket connection.
const socket = new WebSocket('ws://localhost:8080/');

// Connection opened
socket.addEventListener('open', function(event) {
  socket.send('Hello Server!');
});

// Listen for messages
socket.addEventListener('message', function(event) {
  console.log('Message from server ', event.data);
});
```

<div align="right">
    <b><a href="#">??? back to top</a></b>
</div>