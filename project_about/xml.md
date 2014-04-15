##Why are we using XML?

- why XML in particular to create texts of the inscriptions
- benefits and accessibility of XML
- possibility for future development

## Why markup?

- You should never use visual formatting to encode information about a text.
	- e.g. the Leiden Conventions

- Markup creates **source text**
	- We can make decisions about visual presentation without changing the source text

---

## The Benefits

- no ambiguity - consider words in italics
	- Is it a book title?  
	- Is it in a foreign language?  
	- Is it just italics for emphasis?  
	- With markup WE KNOW

---

## The Benefits

- automated processing
	- and not just one program

- easily integrated with other things (like version control systems!)

---

## What is XML?

- eXtensible Markup Language
- Rules that explicitly identify semantics of text
- Uses the same characters as the text, but are clearly distinguishable from the text

---

## XML looks like this...

	<html> <head>
  		<meta charset="UTF-8"/>
  		<title>CHS Summer seminar, 2011</title>
  		...
  		</head>
  		<body>
  		<header>Homer Multitext Seminar, Summer 2011</header>
   		...
  		<article>
  		<h1>CHS Summer seminar, 2011</h1>
  		<h2>Schedule</h2>

---

## The Basics

- **elements**: describe the document's semantics
	
	<p>One paragraph of text contained within an element “p”.</p> 

- **attributes**:  provide further information about an element
	
	<p n=”2”>One paragraph of text contained within an element “p”.</p> 

- **processing instructions**:  how to process the document
	
	<?xml version="1.0" encoding="UTF-8"?>

	- but we don't add these to our documents!

---

## Well-Formed XML

- the "Chinese box"
	- everything is fully contained in their parent element

---

	<body>
		<p>
			<l n="1"> This is a <choice>
									<abbr>ln</abbr>
									<expan>line</expan>
									</choice></l>
		</p>
	</body>

---

## Validation

- Markup language can be verified automatically by a **parser**
- **schema**:  rule set

---

## Guidelines for scholarly text editing

- **TEI**: Text Encoding Initiative guidelines
- [Index of elements][index]

[index]: http://www.tei-c.org/release/doc/tei-p5-doc/en/html/REF-ELEMENTS.html
