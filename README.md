# css-html-tuts
my css html practice repo

HTML Basics
# What is HTML?
- Hypertext Markup Language - standard markup language used to create web pages
- Basically tells your browser how to display webpages

# What does HTML look like
- HTML uses tags and elements to enclose different parts of the content
<p>My name is Vengat</p>
<!DOCTYPE html>   # informs the browser that the document type is html
<html>  # informs the browser that the document type is HTML
<head>  # put content here that visitors shouldnt see Eg link to javascript or stylesheet files
    <meta charset="utf-8">
    <title>Title</title>
</head>
<body>
</body>
</html>

Intro to CSS

# What is CSS
- Cascading Style Sheets - language to style and lay out web pages
- Can use to style font, colour, spacing, layout of page, animations
- Language for styling your document and determining how it is presented

# How can we alter the appearance of HTML with CSS?
- Web browser looks for CSS rules
    # What's a CSS rule?
    - Selector = essentially 'selects' the HTML element(s) you want to style
    - Properties - properties which you want to change

# CSS Declarations
- Where you set the CSS properties to specific values

some-element {
    background-color: rgb(0, 0, 255);
    font-size: 50px;
}

# The CSS Box Model
- Each element in a HTML element can be thought of as a rectangular box
- The standard box model describes the space an element takes up
- Each box has four edges: margin, border, padding, content edges

- Think of nested rectangles

Margin Edge
|--------------------------------------
|Border Edge
|    |-----------------------------
|    |Padding Edge
|    |    |------------------
|    |    |Content Edge
|    |    |    |-------                
|    |    |    |
|    |    |    |
|    |    |    |
|    |    |    |
|    |    |    |--------
|    |    |
|    |    |-------------------
|    |
|    |-----------------------------
|
|--------------------------------------

# CSS Specificity
- Specificity is super important with css
    0. Type selectors (eg h1, div, header, p)
    1. Class selectors 
    2. ID selectors


- This qualifies the direct sibling h4 of h3

#second-example h3+h4 {
    font-family: 'Courier New', Courier, monospace;
    background-color: indianred;
}