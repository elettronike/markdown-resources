<link 	href='elettronike_markdown.css?version=1'
	rel='stylesheet' type="text/css" >
</link>

MarkDownManual
==============

------------------------------------------------------------------------

------------------------------------------------
Author: Fabio De Angelis
rev: A
date: 12-4-2020
------------------------------------------------



[Unordered Lists](#unordered-lists)
[Text Formatting (Span Eelements)](#span-elements)
[Blockquotes](#blockquotes)
[Lists](#lists)
[Images](#images)
      
      
 Block Elements

    Paragraphs and Line Breaks
    Headers
    Blockquotes
    Lists
    Code Blocks
    Horizontal Rules

Span Elements

    Links
    Emphasis
    Code
    Images

Miscellaneous

    Backslash Escapes
    Automatic Links     
      
      

## Why Use Markdown?
  
- Markdown can be used to create websites, documents, notes, books, presentations, email messages, and technical documentation.

- Markdown is portable. Files containing Markdown-formatted text can be opened using virtually any application. 
 If you decide you don’t like the Markdown application you’re currently using, you can import your Markdown files into another Markdown application. That’s in stark contrast to word processing applications like Microsoft Word that lock your content into a proprietary file format.

- Markdown is platform independent. You can create Markdown-formatted text on any device running any operating system.

- Markdown is future proof. Even if the application you’re using stops working at some point in the future, you’ll still be able to read your Markdown-formatted text using a text editing application. This is an important consideration when it comes to books, university theses, and other milestone documents that need to be preserved indefinitely.

- Markdown is used in Websites like Reddit and GitHub support Markdown, and lots of desktop and web-based applications support it.

## Markdown Philosophy

Markdown is intended to be as easy-to-read and easy-to-write as is feasible.

Readability, however, is emphasized above all else. A Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions. While Markdown’s syntax has been influenced by several existing text-to-HTML filters — including Setext, atx, Textile, reStructuredText, Grutatext, and EtText — the single biggest source of inspiration for Markdown’s syntax is the format of plain text email.

To this end, Markdown’s syntax is comprised entirely of punctuation characters, which punctuation characters have been carefully chosen so as to look like what they mean. E.g., asterisks around a word actually look like *emphasis*. Markdown lists look like, well, lists. Even blockquotes look like quoted passages of text, assuming you’ve ever used email.


## Markdown Processors

There are dozens of Markdown processors available. 
Many of them allow you to add extensions that enable extended syntax elements. 
Check your processor’s documentation for more information.


## Markdown Editors

**Gedit** integrates Markdown with [Gedit Markdown Preview](https://github.com/maoschanz/gedit-plugin-markdown_preview)

**Dillinger** is one of the best online Markdown editors. Just open the [Dillinger](https://dillinger.io/) site and start typing in the left pane. A preview of the rendered document appears in the right pane.

**markup.rocks** online, Pandoc based document editor editor and preview
[Markup.rocks](https://ipfs.io/ipfs/QmWPgJnUGLB1LPh9KMG9LEN4LVu5e17TwkEtcmTWdNn9V6/#README.md) 
is a client-side app that lets you edit, preview and convert between documents written in various markup languages in your browser.

# Basic Syntax

------------------------------------------------------------------------

## Overview

Nearly all Markdown applications support the basic syntax outlined in John Gruber’s original design document. 
There are minor variations and discrepancies between Markdown processors — those are noted inline wherever possible.

## Headings

To create a heading, add number signs (\#) in front of a word or phrase. 
The number of number signs you use should correspond to the heading level. 
For example, to create a heading level three (`<h3>`), use three number signs 
(e.g. `### My Header`).

|Markdown alternative| Markdown 	     |HTML                        |Rendered Output          |
|-------------:|------------------------|----------------------------|-------------------------|	
|======        | # Heading level 1     	|`<h1> Heading level 1</h1>` |<h1> Heading level 1</h1>|
|--------------| ## Heading level 2 	|`<h2> Heading level 2</h2>` |<h2> Heading level 2</h2>|	
|              | ### Heading level 3 	|`<h3> Heading level 3</h3>` |<h3> Heading level 3</h3>|	
|              | #### Heading level 4 	|`<h4> Heading level 4</h4>` |<h4> Heading level 4</h4>|	
|              | ##### Heading level 5 	|`<h5> Heading level 5</h5>` |<h5> Heading level 5</h5>|	
|              | ###### Heading level 6	|`<h6> Heading level 6</h6>` |<h6> Heading level 6</h6>|	

### Heading Best Practices

Markdown applications don’t agree on how to handle missing blank lines between a heading and the surrounding paragraphs. For compatibility, separate paragraphs and headings with one or more blank lines.

### Heading IDs

Many Markdown processors support custom IDs for headings — some Markdown processors automatically add them. Adding custom IDs allows you to link directly to headings and modify them with CSS. To add a custom heading ID, enclose the custom ID in curly braces on the same line as the heading.

_Markdown_ 	
> `##### My Great Heading {#custom-id}`

_HTML_ 	
> `<h5 id="custom-id">My Great Heading</h5>`    

_Rendered Output_
> <h5 id="custom-id">My Great Heading</h5>



### Linking to Heading IDs

You can link to headings with custom IDs in the file by creating a standard link with a number sign (#) followed by the custom heading ID as an alphanumeric string.

_Markdown_ 	
> `[Heading IDs](#custom-ids)` 	 	

_HTML_ 	
> `<a href="#custom-ids">Heading IDs</a>`    

_Rendered Output_
> [Heading IDs](#heading-ids)


Other websites can link to the heading by adding the custom heading ID to the full URL of the webpage (e.g, [Heading IDs](https://www.markdownguide.org/extended-syntax#heading-ids)).





## Paragraphs

- To create paragraphs, use a blank line to separate one or more lines of text.

- Don’t indent paragraphs with spaces or tabs.

## Line Breaks

To create a line break (`<br>`), end a line with **two or more spaces**, and then type return.

### Line Breaks - Best Practices

You can use two or more spaces (referred to as “trailing whitespace”) for line breaks in nearly every Markdown application, but it’s controversial. It’s hard to see trailing whitespace in an editor, and many people accidentally or intentionally put two spaces after every sentence. For this reason, you may want to use something other than trailing whitespace for line breaks. Fortunately, there is another option supported by nearly every Markdown application: the `<br>` HTML tag.<br>

For compatibility, use trailing white space or the `<br>` HTML tag at the end of the line.

There are two other options I don’t recommend using. CommonMark and a few other lightweight markup languages let you type a backslash (\\) at the end of the line, but not all Markdown applications support this, so it isn’t a great option from a compatibility perspective. And at least a couple lightweight markup languages don’t require anything at the end of the line — just type return and they’ll create a line break.

## Horizontal Rules

To create a horizontal rule, use three or more asterisks (`***`), dashes (`---`), or underscores (`___`) on a line by themselves.
The rendered output of all three looks identical.

***NOTE*** For compatibility, put blank lines before and after horizontal rules.

# Text Formatting (Span Eelements) {#span-elements}

------------------------------------------------------------------------

## Emphasis

You can add emphasis by making text bold or italic.

## Bold

To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

For example:

>> `**bold text**, other __bold text__ and bold in**si**de` 

will produce: 

>> **bold text**, other __bold text__ and bold in**si**de

## Italic

To italicize text, add one asterisk or underscore before and after a word or phrase.
To italicize the middle of a word for emphasis, add one asterisk without spaces around the letters.
Markdown applications don’t agree on how to handle underscores in the middle of a word. For compatibility, use asterisks to italicize the middle of a word for emphasis.

Markdown

>`Italicized text is the *cat's meow* or m*eo*w.`

HTML

> `Italicized text is the <em>cat's meow</em> or m<em>eo<em>w.`

Rendered Output

> Italicized text is the *cat's meow* or m*eo*w.

## Bold and Italic

To emphasize text with bold and italics at the same time, add three asterisks or underscores before and after a word or phrase. To bold and italicize the middle of a word for emphasis, add three asterisks without spaces around the letters.

Markdown applications don’t agree on how to handle underscores in the middle of a word. For compatibility, use asterisks to bold and italicize the middle of a word for emphasis.

Markdown: 

>> `This text is ***really important***.`    
>> `This text is __*really important*__.`    
>> `This text is _**really important**_.`    
>> `This text is ___really important___.`    

HTML:

>> `This text is <strong><em>really important</em></strong>.`

Rendered Output:

>> This text is ***really important***.

## Strikethrough

You can strikethrough words by putting a horizontal line through the center of them. 
This feature allows you to indicate that certain words are a mistake not meant for inclusion in the document. 
To strikethrough words, use two tilde symbols (~~) before and after the words.

`~~The world is flat.~~ We now know that the world is round.`

The rendered output looks like this:

~~The world is flat.~~ We now know that the world is round.

## Blockquotes {#blockquotes}

To create a blockquote, add a `>` in front of a paragraph.

>> `> Hic sunt leones.`

The rendered output looks like this:

>> _Hic sunt leones_.

### Blockquotes with Multiple Paragraphs

Blockquotes can contain multiple paragraphs. Add a `>` on the blank lines between the paragraphs.
 
```
>    In an extreme view, the world can be seen as only connections... 
>
>    nothing else.
```

The rendered output looks like this:

>>>    In an extreme view, the world can be seen as only connections... 
>>>
>>>    nothing else.

### Nested Blockquotes

Blockquotes can be nested. Add a `>>` in front of the paragraph you want to nest.
```
>    In an extreme view, the world can be seen as only connections... 
>
>>    nothing else.
```
The rendered output looks like this:

>>>    In an extreme view, the world can be seen as only connections... 
>>>
>>>   : nothing else.

### Blockquotes with Other Elements

Blockquotes can contain other Markdown formatted elements. Not all elements can be used — you’ll need to experiment to see which ones work.
```
		> #### The quarterly results look great!
		>
		> - Revenue was off the chart.
		> - Profits were higher than ever.
		>
		>  *Everything* is going according to **plan**.
```
The rendered output looks like this:

>>> #### Markdown rocks!
>>>
>>> - Is Simple.
>>> - Is Portable.
>>> - Is Popular.
>>>
>>>  *Everything* is **great**.


# Lists {#lists}

------------------------------------------------------------------------

You can organize items into ordered and unordered lists.

## Ordered Lists

To create an ordered list, add line items with numbers followed by periods. 
The numbers don’t have to be in numerical order,
but the list should start with the number one.

Markdown:
```
		1. First item  
		2. Second item  
		3. Third item  
		    11. Indented item   
		    12. Indented item   
		6. Fourth item   
```

HTML:
```html
		<ol>
		<li>First item</li>
		<li>Second item</li>
		<li>Third item
		<ol>
		<li>Indented item</li>
		<li>Indented item</li>
		</ol>
		</li>
		<li>Fourth item</li>
		</ol> 	
```

Rendered Output

>>> 1. First item  
> 2. Second item
> 3. Third item
> :   11. Indented item   
> :   12. Indented item   
> 6. Fourth item   


## Unordered Lists {#lnordered-lists}

To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.

Markdown:
```markdown
		+ First item
		* Second item
		- Third item
		    - Indented item
		    	- Indented item
		+ Fourth item
```

HTML:
```html
		<ul>
		<li>First item</li>
		<li>Second item</li>
		<li>Third item
		<ul>
		<li>Indented item</li>
		<ul>
		<li>Indented item</li>
		</ul>
		</ul>
		</li>
		<li>Fourth item</li>
		</ul>
```

Rendered Output: 

>>> + First item
>>> * Second item
>>> - Third item  
>>> 	- Indented item   
>>>			- Indented item
>>> + Fourth item 	

-----

### Adding Elements in Lists

To add another element in a list while preserving the continuity of the list,
indent the element four spaces or one tab, as shown in the following examples.

**Paragraphs**

```
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.
```
The rendered output looks like this:

: *   This is the first list item.
: *   Here's the second list item.
:   
:    I need to add another paragraph below the second list item.
:   
: *   And here's the third list item.

**Blockquotes**

```
		*   This is the first list item.
		*   Here's the second list item.

		    > A blockquote would look great below the second list item.

		*   And here's the third list item.
```
The rendered output looks like this:

> *   This is the first list item.
> *   Here's the second list item.
>   
> 		> A blockquote would look great below the second list item.
>   
> *   And here's the third list item.

## Definition Lists

Some Markdown processors allow you to create definition lists of terms and their corresponding definitions. 
To create a definition list, type the term on the first line. On the next line, type a colon followed by a space and the definition.
```
First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.
```
The HTML looks like this:

```
<dl>
  <dt>First Term</dt>
  <dd>This is the definition of the first term.</dd>
  <dt>Second Term</dt>
  <dd>This is one definition of the second term. </dd>
  <dd>This is another definition of the second term.</dd>
</dl>
```
The rendered output looks like this:

> First Term
> : This is the definition of the first term.

> Second Term
> : This is one definition of the second term.
> : This is another definition of the second term.

## Task Lists

Task lists allow you to create a list of items with checkboxes. 
In Markdown applications that support task lists, checkboxes will be displayed next to the content. To create a task list, add dashes (-) and brackets with a space ([ ]) in front of task list items. To select a checkbox, add an x in between the brackets ([x]).

```
 	- [x] Write the press release
 	- [ ] Update the website
 	- [ ] Contact the media
```

# Images {#images}

------------------------------------------------------------------------

```
		![image]( file:image.png "image title"){ width=500 }
```

The rendered output looks like this:

![Tux, the Linux mascot](/assets/images/tux.png)


## Images

To add an image, add an exclamation mark (!), followed by alt text in brackets, 
and the path or URL to the image asset in parentheses. 
You can optionally add a title after the URL in the parentheses.

![Philadelphia's Magic Gardens. This place was so cool!](/assets/images/philly-magic-gardens.jpg "Philadelphia's Magic Gardens")

The rendered output looks like this:

Philadelphia's Magic Gardens. This place was so cool!
Linking Images

To add a link to an image, enclose the Markdown for the image in brackets, and then add the link in parentheses.

[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)

The rendered output looks like this:

# Code 

------------------------------------------------------------------------

Code blocks are normally indented four spaces or one tab. 
When they’re in a list, indent them eight spaces or two tabs.
```
		1.  Open the file.
		2.  Find the following code block on line 21:

			  <head>
			    <title>Test</title>
			  </head>

		3.  Update the title to match the name of your website.
```
The rendered output looks like this:

>>> 1.  Open the file.
>>> 2.  Find the following code block on line 21:
>>> ```
>>>	  	    	<head>
>>>    			<title>Test</title>
>>>	  	    	</head>
>>> ```
>>> 3.  Update the title to match the name of your website.

## Inline Code

To denote a word or phrase as code, enclose it in **backticks** (\`).

Markdown:    

> ``  At the command prompt, type `nano`. `` 


HTML:   

> `At the command prompt, type <code>nano</code>.`

Rendered Output:

>>> At the command prompt, type `nano`. 


### Escaping Backticks

If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks (\`\`).

Markdown:    

> ``Use `code` in your Markdown file.``


HTML:   

> `<code>Use `code` in your Markdown file.</code>`

Rendered Output:

>>> Use `code` in your Markdown file. 


# Code Blocks

To create code blocks, indent every line of the block by at least four spaces or one tab.
```

    <html>
      <head>
      </head>
    </html>

```
The rendered output looks like this:

		<html>
		  <head>
		  </head>
		</html>

## Fenced Code Blocks

The basic Markdown syntax allows you to create code blocks by indenting lines by four spaces or one tab. 
If you find that inconvenient, try using fenced code blocks. 
Depending on your Markdown processor or editor, you’ll use three backticks (\`\`\`) or three tildes (~~~) on the lines before and after the code block. 
Indentation is automatic!

```
		```
		{
		  "firstName": "John",
		  "lastName": "Smith",
		  "age": 25
		}
		```
```

The rendered output looks like this:


```
		{
		  "firstName": "John",
		  "lastName": "Smith",
		  "age": 25
		}
```

**Tip**: Need to display backticks inside a code block? See this section to learn how to escape them.
Syntax Highlighting

Many Markdown processors support syntax highlighting for fenced code blocks. This feature allows you to add color highlighting for whatever language your code was written in. To add syntax highlighting, specify a language next to the backticks before the fenced code block.

```
		```json
		{
		  "firstName": "John",
		  "lastName": "Smith",
		  "age": 25
		}
		```
```
The rendered output looks like this:

```json
		{
		  "firstName": "John",
		  "lastName": "Smith",
		  "age": 25
		}
```


## Links {#Links}

------------------------------------------------------------------------

To create a link, enclose the link text in brackets (e.g., [Duck Duck Go](https://duckduckgo.com)) and then follow it immediately with the URL in parentheses (e.g., (https://duckduckgo.com)).

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

The rendered output looks like this:

My favorite search engine is Duck Duck Go.

### Links - Adding Titles

You can optionally add a title for a link. This will appear as a tooltip when the user hovers over the link. To add a title, enclose it in parentheses after the URL.
```
	[Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").
```

To quickly turn a URL or email address into a link, enclose it in angle brackets.
```
	<https://www.markdownguide.org>
	<fake@example.com>
```

### Formatting Links

To emphasize links, add asterisks before and after the brackets and parentheses. To denote links as code, add backticks in the brackets.

I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.

See the section on [`code`](#code).

The rendered output looks like this:

I love supporting the EFF.
This is the Markdown Guide.
See the section on code.

### Reference-style Links

Reference-style links are a special kind of link that make URLs easier to display and read in Markdown. Reference-style links are constructed in two parts: the part you keep inline with your text and the part you store somewhere else in the file to keep the text easy to read.

### Formatting the First Part of the Link

The first part of a reference-style link is formatted with two sets of brackets. The first set of brackets surrounds the text that should appear linked. The second set of brackets displays a label used to point to the link you’re storing elsewhere in your document.

Although not required, you can include a space between the first and second set of brackets. The label in the second set of brackets is not case sensitive and can include letters, numbers, spaces, or punctuation.

This means the following example formats are roughly equivalent for the first part of the link:

    [hobbit-hole][1]
    [hobbit-hole] [1]

#### Formatting the Second Part of the Link

The second part of a reference-style link is formatted with the following attributes:

    The label, in brackets, followed immediately by a colon and at least one space (e.g., [label]: ).
    The URL for the link, which you can optionally enclose in angle brackets.
    The optional title for the link, which you can enclose in double quotes, single quotes, or parentheses.

This means the following example formats are all roughly equivalent for the second part of the link:

    [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
    [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
    [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
    [1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
    [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
    [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
    [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)

You can place this second part of the link anywhere in your Markdown document. Some people place them immediately after the paragraph in which they appear while other people place them at the end of the document (like endnotes or footnotes).
An Example Putting the Parts Together

Say you add a URL as a standard URL link to a paragraph and it looks like this in Markdown:

In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.

Though it may point to interesting additional information, the URL as displayed really doesn’t add much to the existing raw text other than making it harder to read. To fix that, you could format the URL like this instead:

In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"

In both instances above, the rendered output would be identical:

    In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a hobbit-hole, and that means comfort.

and the HTML for the link would be:

<a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>

### Link local files

```
   [link](file:///d:/absolute.md)    # absolute filesystem path
   [link](./relative1.md)            # relative to opened file
   [link](/relativeToProject.md)     # relative to opened project
```

#### Link Best Practices

Markdown applications don’t agree on how to handle spaces in the middle of a URL. For compatibility, try to URL encode any spaces with **`%20`**.

```
		[link](https://www.example.com/my%20great%20page) 	
```

### Automatic Links

Markdown supports a shortcut style for creating “automatic” links for URLs and email addresses: simply surround the URL or email address with angle brackets. What this means is that if you want to show the actual text of a URL or email address, and also have it be a clickable link, you can do this:
```
	<http://example.com/>
```
Markdown will turn this into:

<a href="http://example.com/">http://example.com/</a>

Automatic links for email addresses work similarly, except that Markdown will also perform a bit of randomized decimal and hex entity-encoding to help obscure your address from address-harvesting spambots. 
For example, Markdown will turn this:
```
<address@example.com>
```
into something like this:
```
<a href="&#x6D;&#x61;i&#x6C;&#x74;&#x6F;:&#x61;&#x64;&#x64;&#x72;&#x65;
&#115;&#115;&#64;&#101;&#120;&#x61;&#109;&#x70;&#x6C;e&#x2E;&#99;&#111;
&#109;">&#x61;&#x64;&#x64;&#x72;&#x65;&#115;&#115;&#64;&#101;&#120;&#x61;
&#109;&#x70;&#x6C;e&#x2E;&#99;&#111;&#109;</a>
```
which will render in a browser as a clickable link to “address@example.com”.

(This sort of entity-encoding trick will indeed fool many, if not most, address-harvesting bots, but it definitely won’t fool all of them. It’s better than nothing, but an address published in this way will probably eventually start receiving spam.)



## Tables

------------------------------------------------------------------------

To add a table, use three or more hyphens (---) to create each column’s header, and use pipes (|) to separate each column. You can optionally add pipes on either end of the table.
```
	| Syntax      | Description |
	| ----------- | ----------- |
	| Header      | Title       |
	| Header      | Section     |
	| Paragraph   | Text        |
```

The rendered output looks like this:

>>> | Syntax      | Description |
>>> | ----------- | ----------- |
>>> | Header      | Title       |
>>> | Header      | Section       |
>>> | Paragraph   | Text        |


**Tip**: Creating tables with hyphens and pipes can be tedious. To speed up the process, try using the Markdown Tables Generator. Build a table using the graphical interface, and then copy the generated Markdown-formatted text into your file.

### Alignment

You can align text in the columns to the left, right, or center by adding a colon (:) to the left, right, or on both side of the hyphens within the header row.
```
	| Syntax      | Description | Test Text     |
	| :---        |    :----:   |          ---: |
	| Header      | Title       | Here's this   |
	| Paragraph   | Text        | And more      |
```

The rendered output looks like this:

> | Syntax      | Description | Test Text     |
> |:----------  |    :----:   |          ---: |
> | Header      | Title       | Here's this   |
> | Paragraph   | Text        | And more      |

You can format the text within tables. For example, you can add links, code (words or phrases in backticks (\`) only, not code blocks), and emphasis.

You can’t add headings, blockquotes, lists, horizontal rules, images, or HTML tags.

#### Escaping Pipe Characters in Tables

You can display a pipe ( | ) character in a table by using its HTML character code `&#124;`.

## Escaping Characters

To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash (\) in front of the character.

\* Without the backslash, this would be a bullet in an unordered list.

The rendered output looks like this:

* Without the backslash, this would be a bullet in an unordered list.
Characters You Can Escape

You can use a backslash to escape the following characters.
```
	Character  Name
	\          backslash
	`          backtick (see also escaping backticks in code)
	*          asterisk
	_          underscore
	{ }        curly braces
	[ ]        brackets
	( )        parentheses
	#          pound sign
	+          plus sign
	-          minus sign (hyphen)
	.          dot
	!          exclamation mark
	|          pipe (see also escaping pipe in tables)
```


## HTML

------------------------------------------------------------------------

Many Markdown applications allow you to use HTML tags in Markdown-formatted text. 
This is helpful if you prefer certain HTML tags to Markdown syntax. 
For example, some people find it easier to use HTML tags for images. 
Using HTML is also helpful when you need to change the attributes of an element, 
like specifying the color of text or changing the width of an image.

To use HTML, place the tags in the text of your Markdown-formatted file.

>`This **word** is bold. This <em>word</em> is italic.`

The rendered output looks like this:

>This **word** is bold. This <em>word</em> is italic.

### HTML Best Practices

For security reasons, not all Markdown applications support HTML in Markdown documents. 
When in doubt, check your Markdown application’s documentation.   
**Some applications support only a subset of HTML tags**.

Use blank lines to separate block-level HTML elements like 
`<div>`, `<table>`, `<pre>`, and `<p>` from the surrounding content. 
Try not to indent the tags with tabs or spaces — that can interfere with the formatting.

You can’t use Markdown syntax inside block-level HTML tags. 
For example, `<p>italic and **bold**</p>` won’t work.

### Inline HTML

Markdown’s syntax is intended for one purpose: to be used as a format for writing for the web.

Markdown is not a replacement for HTML, or even close to it. Its syntax is very small, corresponding only to a very small subset of HTML tags. The idea is not to create a syntax that makes it easier to insert HTML tags. In my opinion, HTML tags are already easy to insert. The idea for Markdown is to make it easy to read, write, and edit prose. HTML is a publishing format; Markdown is a writing format. Thus, Markdown’s formatting syntax only addresses issues that can be conveyed in plain text.

For any markup that is not covered by Markdown’s syntax, you simply use HTML itself. There’s no need to preface it or delimit it to indicate that you’re switching from Markdown to HTML; you just use the tags.

The only restrictions are that block-level HTML elements — e.g. <div>, <table>, <pre>, <p>, etc. — must be separated from surrounding content by blank lines, and the start and end tags of the block should not be indented with tabs or spaces. Markdown is smart enough not to add extra (unwanted) <p> tags around HTML block-level tags.

For example, to add an HTML table to a Markdown article:

This is a regular paragraph.

> <table>
>     <tr>
>         <td>Foo</td>
>     </tr>
> </table>

This is another regular paragraph.

**Note** that Markdown formatting syntax is not processed within block-level HTML tags. E.g., you can’t use Markdown-style *emphasis* inside an HTML block.

Span-level HTML tags — e.g. `<span>`, `<cite>`, or `<del>` — can be used anywhere in a Markdown paragraph, list item, or header. If you want, you can even use HTML tags instead of Markdown formatting; e.g. if you’d prefer to use HTML `<a>` or `<img>` tags instead of Markdown’s link or image syntax, go right ahead.

Unlike block-level HTML tags, Markdown syntax is processed within span-level tags.
Automatic Escaping for Special Characters

In HTML, there are two characters that demand special treatment: < and &. Left angle brackets are used to start tags; ampersands are used to denote HTML entities. If you want to use them as literal characters, you must escape them as entities, e.g. `&lt;`, and `&amp;`.

Ampersands in particular are bedeviling for web writers. If you want to write about ‘AT&T’, you need to write `‘AT&amp;T’`. You even need to escape ampersands within URLs. Thus, if you want to link to:

> http://images.google.com/images?num=30&q=larry+bird

you need to encode the URL as:

> http://images.google.com/images?num=30&amp;q=larry+bird

in your anchor tag href attribute. Needless to say, this is easy to forget, and is probably the single most common source of HTML validation errors in otherwise well-marked-up web sites.

Markdown allows you to use these characters naturally, taking care of all the necessary escaping for you. If you use an ampersand as part of an HTML entity, it remains unchanged; otherwise it will be translated into `&amp;`.

So, if you want to include a copyright symbol in your article, you can write:

> &copy;

and Markdown will leave it alone. But if you write:

> AT&T

Markdown will translate it to:

> AT&amp;T

Similarly, because Markdown supports inline HTML, if you use angle brackets as delimiters for HTML tags, Markdown will treat them as such. But if you write:

> 4 < 5

Markdown will translate it to:

> 4 &lt; 5

However, inside Markdown code spans and blocks, angle brackets and ampersands are always encoded automatically. This makes it easy to use Markdown to write about HTML code. (As opposed to raw HTML, which is a terrible format for writing about HTML syntax, because every single < and & in your example code needs to be escaped.)





# Extended Sintax

------------------------------------------------------------------------

The basic syntax outlined in John Gruber’s original design document added many of the elements needed on a day-to-day basis, but it wasn’t enough for some people. That’s where extended syntax comes in.

Several individuals and organizations took it upon themselves to extend the basic syntax by adding additional elements like tables, code blocks, syntax highlighting, URL auto-linking, and footnotes. These elements can be enabled by using a lightweight markup language that builds upon the basic Markdown syntax, or by adding an extension to a compatible Markdown processor.
Availability

Not all Markdown applications support extended syntax elements. You’ll need to check whether or not the lightweight markup language your application is using supports the extended syntax elements you want to use. If it doesn’t, it may still be possible to enable extensions in your Markdown processor.
Lightweight Markup Languages

There are several lightweight markup languages that are supersets of Markdown. 
They include Gruber’s basic syntax and build upon it by adding additional elements like tables, code blocks, syntax highlighting, URL auto-linking, and footnotes. 
Many of the most popular Markdown applications use one of the following lightweight markup languages:

```
    CommonMark
    GitHub Flavored Markdown (GFM)
    Markdown Extra
    MultiMarkdown
    R Markdown
```




## Footnotes

------------------------------------------------------------------------

Footnotes allow you to add notes and references without cluttering the body of the document. When you create a footnote, a superscript number with a link appears where you added the footnote reference. Readers can click the link to jump to the content of the footnote at the bottom of the page.

To create a footnote reference, add a caret and an identifier inside brackets (`[^1]`). Identifiers can be numbers or words, but they can’t contain spaces or tabs. Identifiers only correlate the footnote reference with the footnote itself — in the output, footnotes are numbered sequentially.

Add the footnote using another caret and number inside brackets with a colon and text (`[^1]: My footnote.`). You don’t have to put footnotes at the end of the document. You can put them anywhere except inside other elements like lists, block quotes, and tables.
```
	Here's a simple footnote,[^1] and here's a longer one.[^bignote]

	[^1]: This is the first footnote.

	[^bignote]: Here's one with multiple paragraphs and code.

	    Indent paragraphs to include them in the footnote.
	
    	`{ my code }`

    	Add as many paragraphs as you like.
```
The rendered output looks like this:

> Here's a simple footnote,[^1] and here's a longer one.[^bignote]



[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.
	    Indent paragraphs to include them in the footnote.	
    	    `{ my code }`
    	    Add as many paragraphs as you like.




## Emoji

------------------------------------------------------------------------

There are two ways to add emoji to Markdown files: copy and paste the emoji into your Markdown-formatted text, or type emoji shortcodes.
Copying and Pasting Emoji

In most cases, you can simply copy an emoji from a source like Emojipedia and paste it into your document. Many Markdown applications will automatically display the emoji in the Markdown-formatted text. The HTML and PDF files you export from your Markdown application should display the emoji.
Tip: If you're using a static site generator, make sure you encode HTML pages as UTF-8.

### Using Emoji Shortcodes

Some Markdown applications allow you to insert emoji by typing emoji shortcodes. These begin and end with a colon and include the name of an emoji.

Gone camping! :tent: Be back soon.

That is so funny! :joy:

The rendered output looks like this:

Gone camping! ⛺ Be back soon.

That is so funny! 😂
Note: You can use this list of emoji shortcodes, but keep in mind that emoji shortcodes vary from application to application. Refer to your Markdown application's documentation for more information.


## Automatic URL Linking

------------------------------------------------------------------------

Many Markdown processors automatically turn URLs into links. That means if you type http://www.example.com, your Markdown processor will automatically turn it into a link even though you haven’t used brackets.

>`http://www.example.com`

The rendered output looks like this:

>[http://www.example.com]()

### Disabling Automatic URL Linking

If you don’t want a URL to be automatically linked, you can remove the link by denoting the URL as code with backticks.

>`` `http://www.example.com` ``

The rendered output looks like this:

>`http://www.example.com`




