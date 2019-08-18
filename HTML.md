### HTML

### Markup provides content with structure

#### Display types:

-Block display type *takes up 100% of the width of the page.* Can be moved up, down, left and right.

-Inline display type *takes up only the width of the elements within.* Can be only moved left or right. 

##### HTML5 -> Semantic markup structures 

<header>
<nav>
<main>
<article>
<footer>
<aside>
<section>

Basic form validation - Empty forms, email validation built-in

Attributes are key/value pairs that provide meta information - more information about that element
class attribute. One key, multiple values. E.g. class = "active cool", not class="active" class="cool"

The difference between h1 and h2 is purely importance.

###Lists:
-<ol>: Ordered list. Useful for showing importance and steps of a process
-<ul>: Unordered list. Great for items with roughly the same relative performance.
-<dl>: Definition list. Used for a series of terms and their definitions.
--<li>: List item, used for ol and ul lists to denote a listed item
--<dt>: Definition term, the term to be defined in the definition list.
--<dd>: Definition description, a way to describe the term.

### Links
*URL - Uniform Resource Locator*
-Can be absolute (https://www.google.com) or relative (contact.html)

<a href="www.google.com">link</a>
-Created by the <a> tag
-href="www.google.com" is the hyperlink reference. There are several different types of hyperlink references:
1. Standard links. These are links to new pages.
2. #target links. These are links to elements specified by ids. Useful for linking to precise portions of a page.
3. mailto: links. These specify email addresses to be opened by an email client.

Some of these can be chained together, e.g <a href="www.imdb.com/#bottom" target="_blank">link</a>

#### Opening a link in a new window
<a href="www.google.com" target="_blank">link</a>


#### Brian's observations
-<table> is meant purely for tabular data. Do not make layouts with <table>
-One h1 per page. Please. Teh SEO.
-THE GODS WILL SMITE YOU IF YOU USE INLINE CSS.
-Do not capitalize your elements. People will see this and hate you.