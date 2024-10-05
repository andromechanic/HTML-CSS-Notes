# HTML Workshop Notes

## Introduction to HTML

### Overview of HTML and Its Importance

**HTML (HyperText Markup Language)** is the standard language used to create web pages. It forms the backbone of any web content you view online, allowing text, images, videos, and other elements to be displayed in a structured format. Understanding HTML is fundamental for web development, making it an essential skill for anyone looking to create websites or web applications.

### Basic Structure of an HTML Document

An HTML document has a specific structure that ensures browsers can interpret and display its content correctly.

- **HTML Document Structure**:
    
    ```html
    htmlCopy code
    <!DOCTYPE html>
    <html>
      <head>
        <title>Page Title</title>
      </head>
      <body>
        <!-- Content goes here -->
      </body>
    </html>
    
    ```
    
    - `<!DOCTYPE html>`: Declares the document type and version of HTML being used. It's essential for standards compliance and proper rendering.
    - `<html>`: The root element that contains all other HTML elements.
    - `<head>`: Contains meta-information about the document, such as the title, character set, styles, and scripts.
    - `<title>`: Sets the title of the web page, which appears in the browser tab.
    - `<body>`: Contains the content of the web page, including text, images, videos, links, and more.

## HTML Elements and Attributes

### Understanding HTML Tags and Elements

HTML uses **tags** to mark up content. Tags are enclosed in angle brackets, like `<p>`, and usually come in pairs: an opening tag (`<p>`) and a closing tag (`</p>`). The content between the tags is called an **element**.

- **Tags**: Keywords surrounded by angle brackets, e.g., `<p>`.
- **Elements**: Consist of a start tag, content, and an end tag, e.g., `<p>This is a paragraph.</p>`.

### Common Attributes and How to Use Them

**Attributes** provide additional information about an element. They are included within the opening tag and usually come in name/value pairs like `name="value"`.

- **Example**:
    
    ```html
    htmlCopy code
    <img src="image.jpg" alt="Description">
    
    ```
    
- **Common Attributes**:
    - `id`: Unique identifier for an element, used for styling and scripting.
    - `class`: Specifies one or more class names for an element, used for styling.
    - `src`: Specifies the source file for an image.
    - `href`: Specifies the URL for a link.

## Text Formatting and Semantics

### Headings, Paragraphs, and Text Formatting

HTML provides various tags for text formatting, allowing you to structure and style text content.

- **Headings**: Define the hierarchical structure of your content. `<h1>` is the highest level heading, and `<h6>` is the lowest.
    
    ```html
    htmlCopy code
    <h1>Main Heading</h1>
    <h2>Subheading</h2>
    
    ```
    
- **Paragraphs**: Represent blocks of text.
    
    ```html
    htmlCopy code
    <p>This is a paragraph.</p>
    
    ```
    
- **Line Breaks**: Add a line break without starting a new paragraph.
    
    ```html
    htmlCopy code
    Line 1<br>Line 2
    
    ```
    

### Emphasizing Text with Bold and Italics

You can emphasize text using bold and italic styles.

- **Bold**: Use `<strong>` for strong importance and `<b>` for stylistic bold text.
    
    ```html
    htmlCopy code
    <strong>Important</strong>
    <b>Bold Text</b>
    
    ```
    
- **Italics**: Use `<em>` for emphasized text and `<i>` for stylistic italic text.
    
    ```html
    htmlCopy code
    <em>Emphasized</em>
    <i>Italic Text</i>
    
    ```
    

### Creating Lists: Ordered and Unordered

Lists are used to group related items.

- **Ordered Lists**: Create a numbered list with `<ol>`.
    
    ```html
    htmlCopy code
    <ol>
      <li>First item</li>
      <li>Second item</li>
    </ol>
    
    ```
    
- **Unordered Lists**: Create a bulleted list with `<ul>`.
    
    ```html
    htmlCopy code
    <ul>
      <li>First item</li>
      <li>Second item</li>
    </ul>
    
    ```
    

## Links and Navigation

### Creating Hyperlinks

Hyperlinks allow users to navigate from one page to another. They are created using the `<a>` (anchor) tag.

- **Anchor Tag**:
    
    ```html
    htmlCopy code
    <a href="https://example.com">Visit Example</a>
    
    ```
    
    - `href`: Specifies the URL of the page the link goes to.

### Understanding Absolute and Relative URLs

- **Absolute URLs**: Provide the complete web address, including the protocol (http:// or https://).
    
    ```html
    htmlCopy code
    <a href="https://example.com/page.html">Absolute URL</a>
    
    ```
    
- **Relative URLs**: Provide a path relative to the current page, useful for linking within the same website.
    
    ```html
    htmlCopy code
    <a href="page.html">Relative URL</a>
    
    ```
    

### Building a Basic Navigation Menu

A navigation menu helps users move between different sections or pages of a website.

- **Example**:
    
    ```html
    htmlCopy code
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
    
    ```
    

## Working with Images and Media

### Adding Images to Your Web Pages

Images enhance the visual appeal of your web pages.

- **Image Tag**:
    
    ```html
    htmlCopy code
    <img src="image.jpg" alt="Description">
    
    ```
    
    - `src`: Specifies the path to the image file.
    - `alt`: Provides alternative text for accessibility and when the image cannot be displayed.

### Understanding Image Attributes

- **Width and Height**: Control the size of the image.
    
    ```html
    htmlCopy code
    <img src="image.jpg" width="300" height="200">
    
    ```
    
- **Title**: Provides additional information when hovering over the image.
    
    ```html
    htmlCopy code
    <img src="image.jpg" title="Image Title">
    
    ```
    

### Embedding Videos and Audio

HTML5 introduced native support for embedding multimedia content.

- **Video Tag**:
    
    ```html
    htmlCopy code
    <video width="320" height="240" controls>
      <source src="movie.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    
    ```
    
    - `controls`: Adds playback controls (play, pause, volume).
- **Audio Tag**:
    
    ```html
    htmlCopy code
    <audio controls>
      <source src="audio.mp3" type="audio/mpeg">
      Your browser does not support the audio element.
    </audio>
    
    ```
    

## Creating Tables

### Basic Structure of Tables

Tables organize data into rows and columns.

- **Table Tags**: Use `<table>` to define a table, `<tr>` for table rows, `<th>` for table headers, and `<td>` for table cells.
    
    ```html
    htmlCopy code
    <table>
      <tr>
        <th>Header 1</th>
        <th>Header 2</th>
      </tr>
      <tr>
        <td>Data 1</td>
        <td>Data 2</td>
      </tr>
    </table>
    
    ```
    

### Adding Headers, Rows, and Cells

- **Headers**: Use `<th>` to define header cells.
    
    ```html
    htmlCopy code
    <th>Header</th>
    
    ```
    
- **Rows**: Use `<tr>` to define table rows.
    
    ```html
    htmlCopy code
    <tr><td>Data</td></tr>
    
    ```
    
- **Cells**: Use `<td>` to define data cells.
    
    ```html
    htmlCopy code
    <td>Data</td>
    
    ```
    

### Styling Tables for Better Readability

Tables can be styled for better presentation and readability.

- **Attributes**: Add `border`, `cellpadding`, and `cellspacing` to control the appearance.
    
    ```html
    htmlCopy code
    <table border="1" cellpadding="5" cellspacing="0">
      <!-- Table Content -->
    </table>
    
    ```
    
- **CSS for Styling**:
    
    ```css
    cssCopy code
    table {
      width: 100%;
      border-collapse: collapse;
    }
    th, td {
      border: 1px solid black;
      padding: 8px;
      text-align: left;
    }
    th {
      background-color: #f2f2f2;
    }
    
    ```
    

## Building Forms

### Form Elements and Input Types

Forms collect user input and are created using the `<form>` element.

- **Form Tag**:
    
    ```html
    htmlCopy code
    <form action="/submit" method="post">
      <!-- Form Elements -->
    </form>
    
    ```
    
    - `action`: URL where the form data will be submitted.
    - `method`: HTTP method used to submit the form (`get` or `post`).

### Input Types

HTML provides various input types to collect different kinds of user data.

- **Text Input**: Collects plain text.
    
    ```html
    htmlCopy code
    <input type="text" name="username">
    
    ```
    
- **Password Input**: Collects password entries (hidden characters).
    
    ```html
    htmlCopy code
    <input type="password" name="password">
    
    ```
    
- **Email Input**: Validates email format.
    
    ```html
    htmlCopy code
    <input type="email" name="email">
    
    ```
    
- **Submit Button**: Submits the form.
    
    ```html
    htmlCopy code
    <input type="submit" value="Submit">
    
    ```
    

### Creating a Basic Form

- **Example**:
    
    ```html
    htmlCopy code
    <form action="/submit" method="post">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>
    
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>
    
      <input type="submit" value="Submit">
    </form>
    
    ```
    

### Form Validation Basics

HTML5 provides built-in form validation attributes.

- **Required Field**: Ensures the input must be filled out before submitting.
    
    ```html
    htmlCopy code
    <input type="text" name="username" required>
    
    ```
    
- **Pattern**: Validates the input against a regular expression.
    
    ```html
    htmlCopy code
    <input type="text" name="zipcode" pattern="[0-9]{5}" title="Five digit zip code">
    
    ```
    

## HTML5 Semantic Elements

### Introduction to HTML5 Semantic Tags

HTML5 introduced semantic elements that provide meaning to the content, improving accessibility and SEO.

- **Examples**: `<header>`, `<footer>`, `<section>`, `<article>`, `<aside>`, and `<nav>`.

### Using `<header>`, `<footer>`, `<section>`, and `<article>`

- **`<header>`**: Represents the introductory content or set of navigational links.
    
    ```html
    htmlCopy code
    <header>
      <h1>Page Title</h1>
      <nav>
        <ul>
          <li><a href="index.html">Home</a></li>
          <li><a href="about.html">About</a></li>
          <li><a href="contact.html">Contact</a></li>
        </ul>
      </nav>
    </header>
    
    ```
    
- **`<footer>`**: Represents the footer of a document or section.
    
    ```html
    htmlCopy code
    <footer>
      <p>&copy; 2024 Your Company</p>
    </footer>
    
    ```
    
- **`<section>`**: Represents a standalone section of content.
    
    ```html
    htmlCopy code
    <section>
      <h2>Section Title</h2>
      <p>This is a section of content.</p>
    </section>
    
    ```
    
- **`<article>`**: Represents a self-contained composition that can be independently distributed.
    
    ```html
    htmlCopy code
    <article>
      <h2>Article Title</h2>
      <p>This is an article.</p>
    </article>
    
    ```
    

### Benefits of Semantic HTML

- **Accessibility**: Helps screen readers and assistive technologies understand the structure and purpose of the content.
- **SEO**: Improves search engine indexing and ranking by providing meaningful structure.
- **Maintainability**: Makes the code easier to read, understand, and maintain.

## Best Practices and Accessibility

### Writing Clean and Readable HTML Code

- **Indentation**: Use consistent indentation to improve readability.
- **Comments**: Add comments to explain sections of code.
    
    ```html
    htmlCopy code
    <!-- This is a comment -->
    
    ```
    
- **Meaningful Names**: Use descriptive names for `id` and `class` attributes.
    
    ```html
    htmlCopy code
    <div id="main-content" class="container">
    
    ```
    

### Basic Accessibility Guidelines

- **Alt Text**: Provide descriptive alternative text for images.
    
    ```html
    htmlCopy code
    <img src="image.jpg" alt="A description of the image">
    
    ```
    
- **Form Labels**: Ensure all form controls have associated labels.
    
    ```html
    htmlCopy code
    <label for="name">Name:</label>
    <input type="text" id="name" name="name">
    
    ```
    
- **Semantic Elements**: Use semantic elements to define the structure.
    
    ```html
    htmlCopy code
    <header>...</header>
    <nav>...</nav>
    <main>...</main>
    <footer>...</footer>
    
    ```
    

### Introduction to SEO Best Practices

- **Title and Meta Description**: Use meaningful titles and meta descriptions.
    
    ```html
    htmlCopy code
    <title>Page Title</title>
    <meta name="description" content="Description of the page content">
    
    ```
    
- **Headings**: Use headings (`<h1>`, `<h2>`, etc.) to structure content.
- **Alt Text**: Use descriptive alt text for images.
- **URL Structure**: Use clear and descriptive URLs.

## Hands-on Project

### Building a Simple Multi-page Website

Create a small website to apply the concepts learned during the workshop. This will include a homepage, an about page, and a contact page.

### Applying Workshop Concepts

- **Homepage (index.html)**:
    
    ```html
    htmlCopy code
    <!DOCTYPE html>
    <html>
    <head>
      <title>Homepage</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
      <header>
        <h1>Welcome to My Website</h1>
        <nav>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section>
          <h2>About Us</h2>
          <p>This is the homepage of my website.</p>
        </section>
      </main>
      <footer>
        <p>&copy; 2024 Your Company</p>
      </footer>
    </body>
    </html>
    
    ```
    
- **About Page (about.html)**:
    
    ```html
    htmlCopy code
    <!DOCTYPE html>
    <html>
    <head>
      <title>About Us</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
      <header>
        <h1>About Us</h1>
        <nav>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section>
          <h2>Our Story</h2>
          <p>This is the about page of my website.</p>
        </section>
      </main>
      <footer>
        <p>&copy; 2024 Your Company</p>
      </footer>
    </body>
    </html>
    
    ```
    
- **Contact Page (contact.html)**:
    
    ```html
    htmlCopy code
    <!DOCTYPE html>
    <html>
    <head>
      <title>Contact Us</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
      <header>
        <h1>Contact Us</h1>
        <nav>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section>
          <h2>Get in Touch</h2>
          <form action="/submit" method="post">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <input type="submit" value="Submit">
          </form>
        </section>
      </main>
      <footer>
        <p>&copy; 2024 Your Company</p>
      </footer>
    </body>
    </html>
    
    ```
    

# CSS Workshop Notes

## Introduction to CSS

### What is CSS and Its Importance

**CSS (Cascading Style Sheets)** is the language used to describe the presentation of a document written in HTML. It controls the layout of multiple web pages all at once, making it a powerful tool for web design and development. CSS allows you to apply styles such as fonts, colors, spacing, and layouts to HTML elements, enhancing the visual appeal and user experience of web pages.

### How CSS Works with HTML

CSS works by associating style rules with HTML elements. These rules define how the content of specified elements should be displayed. There are three ways to apply CSS to HTML:

- **Inline CSS**: Styles are applied directly within HTML elements using the `style` attribute.
    
    ```html
    htmlCopy code
    <p style="color: red;">This is a red paragraph.</p>
    
    ```
    
- **Internal CSS**: Styles are defined within a `<style>` tag in the HTML document’s `<head>`.
    
    ```html
    htmlCopy code
    <head>
      <style>
        p { color: blue; }
      </style>
    </head>
    
    ```
    
- **External CSS**: Styles are defined in an external file and linked to the HTML document using the `<link>` tag.
    
    ```html
    htmlCopy code
    <head>
      <link rel="stylesheet" href="styles.css">
    </head>
    
    ```
    

### Basic Structure of a CSS Rule

A CSS rule consists of a selector and a declaration block. The selector targets HTML elements, and the declaration block contains one or more declarations separated by semicolons.

- **CSS Rule Structure**:
    
    ```css
    cssCopy code
    selector {
      property: value;
      property: value;
    }
    
    ```
    
- **Example**:
    
    ```css
    cssCopy code
    p {
      color: red;
      font-size: 16px;
    }
    
    ```
    

## Selectors, Properties, and Values

### Types of Selectors

Selectors are used to target HTML elements for styling.

- **Element Selector**: Targets elements by their tag name.
    
    ```css
    cssCopy code
    p { color: green; }
    
    ```
    
- **Class Selector**: Targets elements by their class attribute. Prefixed with a dot (`.`).
    
    ```css
    cssCopy code
    .classname { color: blue; }
    
    ```
    
- **ID Selector**: Targets a single element by its id attribute. Prefixed with a hash (`#`).
    
    ```css
    cssCopy code
    #idname { color: red; }
    
    ```
    
- **Attribute Selector**: Targets elements based on the presence or value of an attribute.
    
    ```css
    cssCopy code
    input[type="text"] { color: purple; }
    
    ```
    
- **Pseudo-class Selector**: Targets elements based on their state.
    
    ```css
    cssCopy code
    a:hover { color: orange; }
    
    ```
    

### Using CSS Properties and Values

Properties are aspects of the elements you want to style, and values specify the styles you want to apply.

- **Example**:
    
    ```css
    cssCopy code
    h1 {
      color: navy;
      text-align: center;
    }
    
    ```
    

### Combining Selectors and Selector Specificity

You can combine selectors to apply styles more specifically.

- **Descendant Selector**: Targets elements that are descendants of another element.
    
    ```css
    cssCopy code
    div p { color: gray; }
    
    ```
    
- **Child Selector**: Targets immediate children of an element.
    
    ```css
    cssCopy code
    div > p { color: black; }
    
    ```
    
- **Selector Specificity**: Determines which styles are applied when multiple styles conflict. Specificity is calculated based on the types of selectors used.

## CSS Box Model

### Understanding the Box Model

The CSS box model represents the structure of an HTML element. It consists of the content, padding, border, and margin.

- **Box Model Components**:
    - **Content**: The actual content of the element.
    - **Padding**: Space between the content and the border.
    - **Border**: A line surrounding the padding (if any) and content.
    - **Margin**: Space outside the border.

### Visualizing and Modifying the Box Model

You can use CSS properties to visualize and modify each component of the box model.

- **Example**:
    
    ```css
    cssCopy code
    div {
      width: 100px;
      padding: 20px;
      border: 5px solid black;
      margin: 10px;
    }
    
    ```
    

### Using `box-sizing` Property

The `box-sizing` property allows you to control how the width and height of an element are calculated.

- **Values**:
    - `content-box`: Default value. Width and height include only the content.
    - `border-box`: Width and height include padding and border.
    
    ```css
    cssCopy code
    div {
      box-sizing: border-box;
    }
    
    ```
    

## Styling Text

### Setting Font Properties

CSS provides various properties to control the appearance of text.

- **Font Family**: Specifies the font to use.
    
    ```css
    cssCopy code
    p {
      font-family: "Arial", sans-serif;
    }
    
    ```
    
- **Font Size**: Specifies the size of the font.
    
    ```css
    cssCopy code
    p {
      font-size: 16px;
    }
    
    ```
    
- **Font Weight**: Specifies the thickness of the font.
    
    ```css
    cssCopy code
    p {
      font-weight: bold;
    }
    
    ```
    
- **Font Style**: Specifies the style of the font (normal, italic, oblique).
    
    ```css
    cssCopy code
    p {
      font-style: italic;
    }
    
    ```
    

### Text Color, Alignment, and Decoration

You can control the color, alignment, and decoration of text.

- **Text Color**: Sets the color of the text.
    
    ```css
    cssCopy code
    p {
      color: blue;
    }
    
    ```
    
- **Text Alignment**: Aligns text horizontally.
    
    ```css
    cssCopy code
    p {
      text-align: center;
    }
    
    ```
    
- **Text Decoration**: Adds decorations to text (underline, overline, line-through).
    
    ```css
    cssCopy code
    p {
      text-decoration: underline;
    }
    
    ```
    

### Using Web Fonts with @font-face

You can use custom fonts by defining them with the `@font-face` rule.

- **Example**:
    
    ```css
    cssCopy code
    @font-face {
      font-family: "CustomFont";
      src: url("customfont.woff2") format("woff2");
    }
    p {
      font-family: "CustomFont", sans-serif;
    }
    
    ```
    

## Backgrounds and Borders

### Setting Background Color and Images

CSS allows you to set background colors and images for elements.

- **Background Color**:
    
    ```css
    cssCopy code
    div {
      background-color: lightblue;
    }
    
    ```
    
- **Background Image**:
    
    ```css
    cssCopy code
    div {
      background-image: url("background.jpg");
    }
    
    ```
    

### Controlling Background Repeat, Position, and Size

You can control how background images are displayed.

- **Background Repeat**: Controls whether the background image repeats.
    
    ```css
    cssCopy code
    div {
      background-repeat: no-repeat;
    }
    
    ```
    
- **Background Position**: Specifies the position of the background image.
    
    ```css
    cssCopy code
    div {
      background-position: center;
    }
    
    ```
    
- **Background Size**: Specifies the size of the background image.
    
    ```css
    cssCopy code
    div {
      background-size: cover;
    }
    
    ```
    

### Adding and Styling Borders

CSS provides properties to add and style borders.

- **Border Style**: Sets the style of the border.
    
    ```css
    cssCopy code
    div {
      border-style: solid;
    }
    
    ```
    
- **Border Width**: Sets the width of the border.
    
    ```css
    cssCopy code
    div {
      border-width: 2px;
    }
    
    ```
    
- **Border Color**: Sets the color of the border.
    
    ```css
    cssCopy code
    div {
      border-color: red;
    }
    
    ```
    

## Layout Techniques

### Introduction to CSS Positioning

CSS positioning allows you to control the placement of elements.

- **Static Positioning**: The default positioning for elements.
    
    ```css
    cssCopy code
    div {
      position: static;
    }
    
    ```
    
- **Relative Positioning**: Positions the element relative to its normal position.
    
    ```css
    cssCopy code
    div {
      position: relative;
      top: 10px;
      left: 10px;
    }
    
    ```
    
- **Absolute Positioning**: Positions the element relative to its nearest positioned ancestor.
    
    ```css
    cssCopy code
    div {
      position: absolute;
      top: 10px;
      left: 10px;
    }
    
    ```
    
- **Fixed Positioning**: Positions the element relative to the viewport.
    
    ```css
    cssCopy code
    div {
      position: fixed;
      top: 10px;
      left: 10px;
    }
    
    ```
    

### Using Flexbox for Flexible Layouts

Flexbox is a layout model that allows you to create flexible and responsive layouts.

- **Flex Container**: Define a flex container.
    
    ```css
    cssCopy code
    .container {
      display: flex;
    }
    
    ```
    
- **Flex Items**: Control the behavior of flex items.
    
    ```css
    cssCopy code
    .item {
      flex: 1;
    }
    
    ```
    

### Introduction to CSS Grid Layout

CSS Grid Layout provides a two-dimensional grid-based layout system.

- **Grid Container**: Define a grid container.
    
    ```css
    cssCopy code
    .container {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-gap: 10px;
    }
    
    ```
    
- **Grid Items**: Place items within the grid.
    
    ```css
    cssCopy code
    .item {
      grid-column: span 2;
    }
    
    ```
    

## Responsive Design and Media Queries

### Basics of Responsive Design

Responsive design ensures that web pages look good on all devices by adapting their layout.

- **Fluid Layouts**: Use percentage-based widths to create flexible layouts.
    
    ```css
    cssCopy code
    .container {
      width: 80%;
    }
    
    ```
    

### Using Media Queries to Adjust Styles

Media queries allow you to apply styles based on device characteristics.

- **Example**:
    
    ```css
    cssCopy code
    @media (max-width: 600px) {
      .container {
        width: 100%;
      }
    }
    
    ```
    

### Responsive Units

Responsive units help create designs that adapt to different screen sizes.

- **Percentages**: Set sizes relative to the parent element.
    
    ```css
    cssCopy code
    .box {
      width: 50%;
    }
    
    ```
    
- **EMs and REMs**: Set sizes relative to the font size.
    
    ```css
    cssCopy code
    .text {
      font-size: 2em;
    }
    
    ```
    
- **Viewport Units**: Set sizes relative to the viewport.
    
    ```css
    cssCopy code
    .box {
      width: 50vw;
      height: 50vh;
    }
    
    ```
    

## Styling Links, Lists, and Navigation

### Customizing Link Styles

CSS allows you to style links for different states.

- **Example**:
    
    ```css
    cssCopy code
    a:link {
      color: blue;
    }
    a:visited {
      color: purple;
    }
    a:hover {
      color: red;
    }
    a:active {
      color: orange;
    }
    
    ```
    

### Styling Lists

CSS can style both ordered and unordered lists.

- **Example**:
    
    ```css
    cssCopy code
    ul {
      list-style-type: square;
    }
    li {
      margin: 5px 0;
    }
    
    ```
    

### Creating and Styling Navigation Menus

You can create and style navigation menus using CSS.

- **Example**:
    
    ```css
    cssCopy code
    nav ul {
      list-style-type: none;
      padding: 0;
    }
    nav li {
      display: inline;
      margin-right: 10px;
    }
    nav a {
      text-decoration: none;
      color: navy;
    }
    
    ```
    

## Transitions, Transformations, and Animations

### Adding CSS Transitions for Smooth Changes

Transitions allow you to change property values smoothly over a given duration.

- **Example**:
    
    ```css
    cssCopy code
    .box {
      transition: background-color 0.5s ease;
    }
    .box:hover {
      background-color: yellow;
    }
    
    ```
    

### Using 2D and 3D Transformations

Transformations allow you to move, rotate, scale, and skew elements.

- **Example**:
    
    ```css
    cssCopy code
    .box {
      transform: rotate(45deg);
    }
    
    ```
    

### Creating Simple CSS Animations

CSS animations allow you to animate elements over time.

- **Example**:
    
    ```css
    cssCopy code
    @keyframes example {
      from {background-color: red;}
      to {background-color: yellow;}
    }
    .box {
      animation-name: example;
      animation-duration: 4s;
    }
    
    ```
    

## Advanced CSS Features

### Understanding and Using Pseudo-elements

Pseudo-elements allow you to style specific parts of an element.

- **Example**:
    
    ```css
    cssCopy code
    p::before {
      content: "Note: ";
      font-weight: bold;
    }
    p::after {
      content: " End.";
      font-weight: bold;
    }
    
    ```
    

### CSS Variables (Custom Properties)

CSS variables allow you to reuse values throughout your CSS.

- **Example**:
    
    ```css
    cssCopy code
    :root {
      --main-color: #3498db;
    }
    p {
      color: var(--main-color);
    }
    
    ```
    

### Introduction to CSS Preprocessors

CSS preprocessors extend CSS with variables, nested rules, and functions.

- **Sass Example**:
    
    ```scss
    scssCopy code
    $main-color: #3498db;
    body {
      color: $main-color;
    }
    
    ```
    

## Best Practices and Performance

### Writing Maintainable and Scalable CSS

- **Organize Styles**: Group related styles together.
- **Use Consistent Naming**: Use a consistent naming convention for classes and IDs.
- **Comment Your Code**: Add comments to explain complex styles.

### Using CSS Resets and Normalization

CSS resets and normalization ensure consistent styling across different browsers.

- **CSS Reset**: Removes all default browser styling.
    
    ```css
    cssCopy code
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
    ```
    
- **Normalization**: Provides better cross-browser consistency.
    
    ```css
    cssCopy code
    /* Include normalize.css */
    
    ```
    

### Optimizing CSS for Performance

- **Minify CSS**: Remove whitespace and comments to reduce file size.
- **Combine Files**: Combine multiple CSS files into one to reduce HTTP requests.
- **Use Efficient Selectors**: Use simple and efficient selectors to improve performance.

## Hands-on Project

### Building a Responsive Web Page with CSS

Create a responsive web page to apply the concepts learned during the workshop. This will include a homepage, an about page, and a contact page.

- **Homepage (index.html)**:
    
    ```html
    htmlCopy code
    <!DOCTYPE html>
    <html>
    <head>
      <title>Homepage</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
      <header>
        <h1>Welcome to My Website</h1>
        <nav>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section>
          <h2>About Us</h2>
          <p>This is the homepage of my website.</p>
        </section>
      </main>
      <footer>
        <p>&copy; 2024 Your Company</p>
      </footer>
    </body>
    </html>
    
    ```
    
- **About Page (about.html)**:
    
    ```html
    htmlCopy code
    <!DOCTYPE html>
    <html>
    <head>
      <title>About Us</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
      <header>
        <h1>About Us</h1>
        <nav>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section>
          <h2>Our Story</h2>
          <p>This is the about page of my website.</p>
        </section>
      </main>
      <footer>
        <p>&copy; 2024 Your Company</p>
      </footer>
    </body>
    </html>
    
    ```
    
- **Contact Page (contact.html)**:
    
    ```html
    htmlCopy code
    <!DOCTYPE html>
    <html>
    <head>
      <title>Contact Us</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    <body>
      <header>
        <h1>Contact Us</h1>
        <nav>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section>
          <h2>Get in Touch</h2>
          <form action="/submit" method="post">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <input type="submit" value="Submit">
          </form>
        </section>
      </main>
      <footer>
        <p>&copy; 2024 Your Company</p>
      </footer>
    </body>
    </html>
    
    ```