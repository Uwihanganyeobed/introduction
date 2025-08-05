# 🚀 Complete HTML/CSS Cheatsheet - Beginner to Intermediate

## 📋 Table of Contents
1. [HTML Fundamentals](#html-fundamentals)
2. [HTML Structure & Semantic Tags](#html-structure--semantic-tags)
3. [HTML Forms & Input Elements](#html-forms--input-elements)
4. [CSS Fundamentals](#css-fundamentals)
5. [CSS Selectors](#css-selectors)
6. [CSS Box Model](#css-box-model)
7. [CSS Layout Systems](#css-layout-systems)
8. [CSS Styling Properties](#css-styling-properties)
9. [CSS Responsive Design](#css-responsive-design)
10. [CSS Animations & Transitions](#css-animations--transitions)
11. [Best Practices & Tips](#best-practices--tips)

---

## 🏗️ HTML Fundamentals

### Basic HTML Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Content goes here -->
    <script src="script.js"></script>
</body>
</html>
```

### Essential Meta Tags
```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Page description">
<meta name="keywords" content="keyword1, keyword2">
<meta name="author" content="Your Name">
<meta property="og:title" content="Page Title">
<meta property="og:description" content="Page description">
<meta property="og:image" content="image.jpg">
```

### Text & Content Tags
```html
<!-- Headings -->
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Section Heading</h3>
<h4>Subsection</h4>
<h5>Minor Heading</h5>
<h6>Smallest Heading</h6>

<!-- Text Content -->
<p>Paragraph text</p>
<span>Inline text</span>
<strong>Bold/Important text</strong>
<em>Italic/Emphasized text</em>
<mark>Highlighted text</mark>
<small>Small text</small>
<del>Deleted text</del>
<ins>Inserted text</ins>
<sub>Subscript</sub>
<sup>Superscript</sup>

<!-- Quotations -->
<blockquote>Long quotation</blockquote>
<q>Short quotation</q>
<cite>Citation</cite>

<!-- Code -->
<code>Inline code</code>
<pre>Preformatted text</pre>
<kbd>Keyboard input</kbd>
<var>Variable</var>
<samp>Sample output</samp>
```

### Lists
```html
<!-- Unordered List -->
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>

<!-- Ordered List -->
<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>

<!-- Description List -->
<dl>
    <dt>Term 1</dt>
    <dd>Definition 1</dd>
    <dt>Term 2</dt>
    <dd>Definition 2</dd>
</dl>
```

### Links & Navigation
```html
<!-- Basic Link -->
<a href="https://example.com">External Link</a>
<a href="page.html">Internal Link</a>
<a href="#section">Anchor Link</a>
<a href="mailto:email@example.com">Email Link</a>
<a href="tel:+1234567890">Phone Link</a>

<!-- Link Attributes -->
<a href="https://example.com" target="_blank">Opens in new tab</a>
<a href="https://example.com" rel="noopener noreferrer">Secure external link</a>
<a href="document.pdf" download>Download Link</a>
```

### Images & Media
```html
<!-- Images -->
<img src="image.jpg" alt="Description" width="300" height="200">
<img src="image.jpg" alt="Description" loading="lazy">

<!-- Responsive Images -->
<picture>
    <source media="(max-width: 768px)" srcset="mobile.jpg">
    <source media="(max-width: 1200px)" srcset="tablet.jpg">
    <img src="desktop.jpg" alt="Description">
</picture>

<!-- Video -->
<video controls width="640" height="360">
    <source src="video.mp4" type="video/mp4">
    <source src="video.webm" type="video/webm">
    Your browser doesn't support video.
</video>

<!-- Audio -->
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    <source src="audio.ogg" type="audio/ogg">
    Your browser doesn't support audio.
</audio>
```

---

## 🏛️ HTML Structure & Semantic Tags

### Page Structure
```html
<header>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<main>
    <article>
        <header>
            <h1>Article Title</h1>
            <time datetime="2024-01-15">January 15, 2024</time>
        </header>
        <section>
            <h2>Section Heading</h2>
            <p>Content goes here...</p>
        </section>
    </article>
    
    <aside>
        <h3>Related Links</h3>
        <ul>
            <li><a href="#">Link 1</a></li>
            <li><a href="#">Link 2</a></li>
        </ul>
    </aside>
</main>

<footer>
    <p>&copy; 2024 Your Website</p>
</footer>
```

### Semantic HTML5 Elements
```html
<header>     <!-- Page or section header -->
<nav>        <!-- Navigation menu -->
<main>       <!-- Main content area -->
<article>    <!-- Standalone content -->
<section>    <!-- Thematic grouping -->
<aside>      <!-- Sidebar content -->
<footer>     <!-- Page or section footer -->
<figure>     <!-- Image with caption -->
<figcaption> <!-- Caption for figure -->
<details>    <!-- Collapsible content -->
<summary>    <!-- Heading for details -->
<time>       <!-- Date/time -->
<address>    <!-- Contact information -->
```

### Tables
```html
<table>
    <caption>Table Caption</caption>
    <thead>
        <tr>
            <th scope="col">Header 1</th>
            <th scope="col">Header 2</th>
            <th scope="col">Header 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
            <td>Data 3</td>
        </tr>
        <tr>
            <td colspan="2">Spanning two columns</td>
            <td>Data 6</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>Footer 1</td>
            <td>Footer 2</td>
            <td>Footer 3</td>
        </tr>
    </tfoot>
</table>
```

---

## 📝 HTML Forms & Input Elements

### Form Structure
```html
<form action="/submit" method="post" enctype="multipart/form-data">
    <fieldset>
        <legend>Personal Information</legend>
        
        <!-- Text Inputs -->
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required>
        
        <!-- Other Input Types -->
        <input type="tel" placeholder="Phone Number">
        <input type="url" placeholder="Website URL">
        <input type="number" min="0" max="100" step="1">
        <input type="range" min="0" max="100" value="50">
        <input type="date">
        <input type="time">
        <input type="datetime-local">
        <input type="color">
        <input type="file" accept="image/*" multiple>
        
        <!-- Checkboxes and Radio Buttons -->
        <input type="checkbox" id="newsletter" name="newsletter">
        <label for="newsletter">Subscribe to newsletter</label>
        
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label>
        
        <!-- Select Dropdown -->
        <select name="country" id="country">
            <option value="">Select a country</option>
            <option value="us">United States</option>
            <option value="ca">Canada</option>
            <option value="uk">United Kingdom</option>
        </select>
        
        <!-- Textarea -->
        <textarea name="message" rows="4" cols="50" placeholder="Your message"></textarea>
        
        <!-- Buttons -->
        <button type="submit">Submit</button>
        <button type="reset">Reset</button>
        <button type="button">Custom Button</button>
    </fieldset>
</form>
```

### Form Validation Attributes
```html
<input type="text" required>                    <!-- Required field -->
<input type="email" pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$">
<input type="text" minlength="3" maxlength="20">
<input type="number" min="0" max="100">
<input type="password" autocomplete="new-password">
<input type="text" placeholder="Enter your name" autofocus>
<input type="email" readonly>
<input type="text" disabled>
```

---

## 🎨 CSS Fundamentals

### CSS Syntax & Structure
```css
/* Selector */
selector {
    property: value;
    property: value;
}

/* Example */
h1 {
    color: blue;
    font-size: 24px;
    margin: 10px 0;
}
```

### Ways to Add CSS
```html
<!-- 1. Inline CSS -->
<p style="color: red; font-size: 16px;">Inline styled text</p>

<!-- 2. Internal CSS -->
<head>
    <style>
        p { color: blue; }
    </style>
</head>

<!-- 3. External CSS -->
<head>
    <link rel="stylesheet" href="styles.css">
</head>
```

### Comments
```css
/* This is a single-line comment */

/*
This is a
multi-line
comment
*/
```

---

## 🎯 CSS Selectors

### Basic Selectors
```css
/* Universal Selector */
* { margin: 0; padding: 0; }

/* Element Selector */
p { color: black; }
h1 { font-size: 2em; }

/* Class Selector */
.highlight { background-color: yellow; }
.btn { padding: 10px 20px; }

/* ID Selector */
#header { background-color: #333; }
#navigation { width: 100%; }
```

### Attribute Selectors
```css
/* Has attribute */
input[required] { border: 2px solid red; }

/* Exact attribute value */
input[type="email"] { background: lightblue; }

/* Contains substring */
a[href*="example"] { color: green; }

/* Starts with */
a[href^="https"] { color: blue; }

/* Ends with */
a[href$=".pdf"] { color: red; }
```

### Pseudo-classes
```css
/* Link states */
a:link { color: blue; }
a:visited { color: purple; }
a:hover { color: red; }
a:active { color: orange; }

/* Form states */
input:focus { outline: 2px solid blue; }
input:disabled { opacity: 0.5; }
input:checked { background: green; }
input:invalid { border: 2px solid red; }

/* Structural pseudo-classes */
li:first-child { font-weight: bold; }
li:last-child { border-bottom: none; }
li:nth-child(2n) { background: #f0f0f0; }
li:nth-child(odd) { background: white; }
li:nth-child(even) { background: #f9f9f9; }

/* Other useful pseudo-classes */
div:empty { display: none; }
p:not(.special) { color: gray; }
```

### Pseudo-elements
```css
/* Before and after */
p::before { content: "→ "; }
p::after { content: " ←"; }

/* First letter and line */
p::first-letter { font-size: 2em; }
p::first-line { font-weight: bold; }

/* Selection */
::selection { background: yellow; }
```

### Combinators
```css
/* Descendant selector */
div p { color: blue; }

/* Child selector */
ul > li { margin: 5px; }

/* Adjacent sibling */
h1 + p { margin-top: 0; }

/* General sibling */
h1 ~ p { color: gray; }
```

---

## 📦 CSS Box Model

### Box Model Components
```css
.box {
    /* Content */
    width: 300px;
    height: 200px;
    
    /* Padding (inside the border) */
    padding: 20px;
    padding-top: 10px;
    padding-right: 15px;
    padding-bottom: 10px;
    padding-left: 15px;
    
    /* Border */
    border: 2px solid #333;
    border-top: 1px solid red;
    border-radius: 10px;
    
    /* Margin (outside the border) */
    margin: 10px;
    margin: 10px 20px;        /* vertical | horizontal */
    margin: 10px 20px 30px;   /* top | horizontal | bottom */
    margin: 10px 20px 30px 40px; /* top | right | bottom | left */
}
```

### Box Sizing
```css
/* Default box-sizing */
.default-box {
    box-sizing: content-box; /* width/height applies to content only */
}

/* Better box-sizing */
.better-box {
    box-sizing: border-box; /* width/height includes padding and border */
}

/* Global reset */
* {
    box-sizing: border-box;
}
```

### Display Properties
```css
/* Block elements */
div { display: block; }         /* Takes full width */
span { display: inline-block; }  /* Inline but can have width/height */
span { display: inline; }        /* Inline, no width/height */

/* Hide elements */
.hidden { display: none; }       /* Completely removes from layout */
.invisible { visibility: hidden; } /* Hides but keeps space */

/* Flex and Grid */
.flex-container { display: flex; }
.grid-container { display: grid; }
```

---

## 🗂️ CSS Layout Systems

### Flexbox
```css
/* Flex Container */
.flex-container {
    display: flex;
    
    /* Direction */
    flex-direction: row;        /* row | row-reverse | column | column-reverse */
    
    /* Wrapping */
    flex-wrap: nowrap;          /* nowrap | wrap | wrap-reverse */
    
    /* Shorthand */
    flex-flow: row wrap;        /* flex-direction + flex-wrap */
    
    /* Main axis alignment */
    justify-content: flex-start; /* flex-start | flex-end | center | space-between | space-around | space-evenly */
    
    /* Cross axis alignment */
    align-items: stretch;       /* stretch | flex-start | flex-end | center | baseline */
    
    /* Multi-line alignment */
    align-content: stretch;     /* stretch | flex-start | flex-end | center | space-between | space-around */
    
    /* Gap between items */
    gap: 10px;
    row-gap: 10px;
    column-gap: 20px;
}

/* Flex Items */
.flex-item {
    /* Grow, shrink, basis */
    flex-grow: 1;               /* How much to grow */
    flex-shrink: 1;             /* How much to shrink */
    flex-basis: auto;           /* Initial main size */
    
    /* Shorthand */
    flex: 1 1 auto;             /* grow | shrink | basis */
    flex: 1;                    /* Common: grow=1, shrink=1, basis=0 */
    
    /* Individual alignment */
    align-self: center;         /* auto | flex-start | flex-end | center | baseline | stretch */
    
    /* Order */
    order: 2;                   /* Changes visual order */
}
```

### CSS Grid
```css
/* Grid Container */
.grid-container {
    display: grid;
    
    /* Define columns and rows */
    grid-template-columns: 1fr 2fr 1fr;
    grid-template-columns: repeat(3, 1fr);
    grid-template-columns: 100px auto 100px;
    grid-template-rows: 50px 200px 50px;
    
    /* Gap between items */
    gap: 10px;
    row-gap: 10px;
    column-gap: 20px;
    
    /* Alignment */
    justify-content: center;    /* start | end | center | stretch | space-around | space-between | space-evenly */
    align-content: center;      /* start | end | center | stretch | space-around | space-between | space-evenly */
    justify-items: center;      /* start | end | center | stretch */
    align-items: center;        /* start | end | center | stretch */
    
    /* Grid areas */
    grid-template-areas:
        "header header header"
        "sidebar main main"
        "footer footer footer";
}

/* Grid Items */
.grid-item {
    /* Positioning */
    grid-column: 1 / 3;         /* Start at column 1, end at column 3 */
    grid-row: 1 / 2;            /* Start at row 1, end at row 2 */
    
    /* Shorthand */
    grid-area: 1 / 1 / 2 / 3;   /* row-start / col-start / row-end / col-end */
    
    /* Named areas */
    grid-area: header;
    
    /* Individual alignment */
    justify-self: center;       /* start | end | center | stretch */
    align-self: center;         /* start | end | center | stretch */
}
```

### Positioning
```css
/* Static (default) */
.static { position: static; }

/* Relative */
.relative {
    position: relative;
    top: 10px;
    left: 20px;
}

/* Absolute */
.absolute {
    position: absolute;
    top: 0;
    right: 0;
}

/* Fixed */
.fixed {
    position: fixed;
    bottom: 20px;
    right: 20px;
}

/* Sticky */
.sticky {
    position: sticky;
    top: 0;
}
```

### Float & Clear
```css
/* Float (legacy layout) */
.float-left { float: left; }
.float-right { float: right; }
.clear-both { clear: both; }
```

---

## 🎨 CSS Styling Properties

### Typography
```css
.text-styling {
    /* Font family */
    font-family: Arial, sans-serif;
    font-family: "Times New Roman", serif;
    font-family: "Courier New", monospace;
    
    /* Font size */
    font-size: 16px;
    font-size: 1.2em;
    font-size: 1.5rem;
    
    /* Font weight */
    font-weight: normal;        /* normal | bold | bolder | lighter | 100-900 */
    font-weight: 400;           /* 400 = normal, 700 = bold */
    
    /* Font style */
    font-style: normal;         /* normal | italic | oblique */
    
    /* Text decoration */
    text-decoration: none;      /* none | underline | line-through | overline */
    text-decoration: underline dotted red;
    
    /* Text transform */
    text-transform: uppercase;  /* uppercase | lowercase | capitalize */
    
    /* Line height */
    line-height: 1.5;
    line-height: 24px;
    
    /* Letter spacing */
    letter-spacing: 1px;
    letter-spacing: 0.1em;
    
    /* Word spacing */
    word-spacing: 2px;
    
    /* Text alignment */
    text-align: left;           /* left | right | center | justify */
    
    /* Text indent */
    text-indent: 20px;
    
    /* White space */
    white-space: nowrap;        /* nowrap | pre | pre-wrap | pre-line */
    
    /* Word wrap */
    word-wrap: break-word;
    word-break: break-all;
    
    /* Text overflow */
    text-overflow: ellipsis;
    overflow: hidden;
    white-space: nowrap;
}
```

### Colors & Backgrounds
```css
.color-background {
    /* Text color */
    color: red;
    color: #ff0000;
    color: rgb(255, 0, 0);
    color: rgba(255, 0, 0, 0.5);
    color: hsl(0, 100%, 50%);
    color: hsla(0, 100%, 50%, 0.5);
    
    /* Background color */
    background-color: lightblue;
    background-color: transparent;
    
    /* Background image */
    background-image: url('image.jpg');
    background-image: linear-gradient(to right, red, blue);
    background-image: radial-gradient(circle, red, blue);
    
    /* Background properties */
    background-repeat: no-repeat;   /* repeat | repeat-x | repeat-y | no-repeat */
    background-position: center;    /* top | center | bottom | left | right | x% y% */
    background-size: cover;         /* auto | cover | contain | x% y% */
    background-attachment: fixed;   /* scroll | fixed | local */
    
    /* Shorthand */
    background: url('image.jpg') no-repeat center/cover;
}
```

### Borders & Shadows
```css
.borders-shadows {
    /* Border */
    border: 2px solid red;
    border-top: 1px dotted blue;
    border-radius: 10px;
    border-radius: 50%;         /* Circle */
    border-radius: 10px 20px 30px 40px; /* top-left | top-right | bottom-right | bottom-left */
    
    /* Border styles */
    border-style: solid;        /* solid | dashed | dotted | double | groove | ridge | inset | outset */
    
    /* Box shadow */
    box-shadow: 2px 2px 5px rgba(0,0,0,0.3);
    box-shadow: inset 0 0 10px rgba(0,0,0,0.5);
    box-shadow: 0 0 10px red, 0 0 20px blue; /* Multiple shadows */
    
    /* Text shadow */
    text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
    text-shadow: 1px 1px 2px red, 0 0 10px blue;
}
```

### Transforms & Effects
```css
.transforms {
    /* 2D Transforms */
    transform: translate(50px, 100px);
    transform: translateX(50px);
    transform: translateY(100px);
    transform: rotate(45deg);
    transform: scale(1.5);
    transform: scaleX(2);
    transform: scaleY(0.5);
    transform: skew(20deg, 10deg);
    
    /* 3D Transforms */
    transform: rotateX(45deg);
    transform: rotateY(45deg);
    transform: rotateZ(45deg);
    transform: translateZ(100px);
    
    /* Multiple transforms */
    transform: translate(50px, 100px) rotate(45deg) scale(1.2);
    
    /* Transform origin */
    transform-origin: top left;
    transform-origin: 50% 50%;
    
    /* Opacity */
    opacity: 0.5;               /* 0 = transparent, 1 = opaque */
    
    /* Filters */
    filter: blur(5px);
    filter: brightness(150%);
    filter: contrast(200%);
    filter: grayscale(100%);
    filter: hue-rotate(90deg);
    filter: saturate(200%);
    filter: sepia(100%);
    filter: blur(2px) brightness(80%);
}
```

---

## 📱 CSS Responsive Design

### Media Queries
```css
/* Mobile First Approach */
/* Base styles for mobile */
.container {
    width: 100%;
    padding: 10px;
}

/* Tablet styles */
@media (min-width: 768px) {
    .container {
        width: 750px;
        margin: 0 auto;
    }
}

/* Desktop styles */
@media (min-width: 1024px) {
    .container {
        width: 1000px;
        padding: 20px;
    }
}

/* Large desktop */
@media (min-width: 1200px) {
    .container {
        width: 1200px;
    }
}

/* Common breakpoints */
@media (max-width: 767px) { /* Mobile */ }
@media (min-width: 768px) and (max-width: 1023px) { /* Tablet */ }
@media (min-width: 1024px) { /* Desktop */ }

/* Orientation */
@media (orientation: landscape) { }
@media (orientation: portrait) { }

/* Print styles */
@media print {
    body { font-size: 12pt; }
    .no-print { display: none; }
}
```

### Flexible Units
```css
/* Relative units */
.relative-units {
    width: 50%;                 /* Percentage of parent */
    font-size: 1.2em;          /* Relative to parent font size */
    padding: 2rem;              /* Relative to root font size */
    width: 50vw;                /* 50% of viewport width */
    height: 100vh;              /* 100% of viewport height */
    font-size: 4vw;             /* 4% of viewport width */
    font-size: 4vh;             /* 4% of viewport height */
    font-size: 2vmin;           /* 2% of smaller viewport dimension */
    font-size: 2vmax;           /* 2% of larger viewport dimension */
}

/* Absolute units */
.absolute-units {
    width: 300px;               /* Pixels */
    font-size: 12pt;            /* Points */
    margin: 1cm;                /* Centimeters */
    padding: 10mm;              /* Millimeters */
    border: 1in;                /* Inches */
}
```

### Responsive Images
```css
/* Responsive images */
img {
    max-width: 100%;
    height: auto;
}

/* Responsive background images */
.hero {
    background-image: url('hero-mobile.jpg');
    background-size: cover;
    background-position: center;
}

@media (min-width: 768px) {
    .hero {
        background-image: url('hero-desktop.jpg');
    }
}
```

---

## ⚡ CSS Animations & Transitions

### Transitions
```css
.transition-example {
    /* Transition property */
    transition: all 0.3s ease;
    transition: opacity 0.5s linear;
    transition: transform 0.2s ease-in-out;
    
    /* Multiple transitions */
    transition: 
        opacity 0.3s ease,
        transform 0.2s ease-in-out,
        background-color 0.5s linear;
    
    /* Transition timing functions */
    transition-timing-function: ease;        /* ease | ease-in | ease-out | ease-in-out | linear */
    transition-timing-function: cubic-bezier(0.25, 0.1, 0.25, 1);
    
    /* Transition delay */
    transition-delay: 0.1s;
}

.transition-example:hover {
    opacity: 0.8;
    transform: scale(1.1);
    background-color: lightblue;
}
```

### Keyframe Animations
```css
/* Define keyframes */
@keyframes slideIn {
    from {
        transform: translateX(-100%);
        opacity: 0;
    }
    to {
        transform: translateX(0);
        opacity: 1;
    }
}

@keyframes bounce {
    0%, 20%, 50%, 80%, 100% {
        transform: translateY(0);
    }
    40% {
        transform: translateY(-30px);
    }
    60% {
        transform: translateY(-15px);
    }
}

/* Apply animations */
.animated-element {
    animation: slideIn 0.5s ease-out;
    animation: bounce 2s infinite;
    
    /* Animation properties */
    animation-name: slideIn;
    animation-duration: 0.5s;
    animation-timing-function: ease-out;
    animation-delay: 0.2s;
    animation-iteration-count: infinite;    /* 1 | infinite | number */
    animation-direction: normal;            /* normal | reverse | alternate | alternate-reverse */
    animation-fill-mode: both;              /* none | forwards | backwards | both */
    animation-play-state: running;          /* running | paused */
}
```

---

## ✅ Best Practices & Tips

### CSS Organization
```css
/* 1. Use consistent naming conventions */
.btn { }                    /* Block */
.btn--primary { }           /* Modifier */
.btn__icon { }              /* Element */

/* 2. Group related styles */
/* ==========================================================================
   Layout
   ========================================================================== */

/* ==========================================================================
   Typography
   ========================================================================== */

/* ==========================================================================
   Components
   ========================================================================== */

/* 3. Use CSS custom properties (variables) */
:root {
    --primary-color: #3498db;
    --secondary-color: #2ecc71;
    --font-size-base: 16px;
    --font-family-base: Arial, sans-serif;
    --spacing-unit: 1rem;
    --border-radius: 4px;
    --box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.button {
    background-color: var(--primary-color);
    font-size: var(--font-size-base);
    padding: var(--spacing-unit);
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
}
```

### Performance Optimization
```css
/* 1. Minimize reflows and repaints */
.optimized {
    /* Use transform instead of changing position */
    transform: translateX(100px);           /* Good */
    /* left: 100px; */                      /* Avoid */
    
    /* Use opacity instead of visibility */
    opacity: 0;                             /* Good */
    /* visibility: hidden; */               /* Less optimal */
    
    /* Use will-change for heavy animations */
    will-change: transform;
}

/* 2. Avoid expensive selectors */
/* Bad */
* { }
[id="navigation"] * { }
div > div > div > p { }

/* Good */
.navigation { }
.nav-item { }
.text-content { }

/* 3. Use efficient CSS properties */
.efficient {
    /* Use shorthand properties */
    margin: 10px 20px;                      /* Good */
    /* margin-top: 10px; margin-right: 20px; margin-bottom: 10px; margin-left: 20px; */ /* Verbose */
    
    /* Combine similar properties */
    border: 1px solid #ccc;                 /* Good */
    /* border-width: 1px; border-style: solid; border-color: #ccc; */ /* Verbose */
}
```

### Accessibility Best Practices
```css
/* 1. Ensure sufficient color contrast */
.accessible-text {
    color: #333;                            /* Dark on light */
    background-color: #fff;
    /* Minimum contrast ratio: 4.5:1 for normal text, 3:1 for large text */
}

/* 2. Provide focus indicators */
button:focus,
input:focus,
a:focus {
    outline: 2px solid #0066cc;
    outline-offset: 2px;
}

/* 3. Use relative units for scalability */
.scalable-text {
    font-size: 1.2rem;                      /* Scales with user preferences */
    line-height: 1.5;                       /* Relative to font size */
}

/* 4. Ensure clickable areas are large enough */
button,
.clickable {
    min-height: 44px;                       /* Minimum touch target size */
    min-width: 44px;
}

/* 5. Hide content properly for screen readers */
.sr-only {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    margin: -1px;
    overflow: hidden;
    clip: rect(0, 0, 0, 0);
    white-space: nowrap;
    border: 0;
}

/* 6. Respect user preferences */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }
}

@media (prefers-color-scheme: dark) {
    body {
        background-color: #1a1a1a;
        color: #ffffff;
    }
}
```

### Common CSS Utilities
```css
/* Reset and normalize */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Clearfix */
.clearfix::after {
    content: "";
    display: table;
    clear: both;
}

/* Visually hidden */
.visually-hidden {
    position: absolute !important;
    width: 1px !important;
    height: 1px !important;
    padding: 0 !important;
    margin: -1px !important;
    overflow: hidden !important;
    clip: rect(0, 0, 0, 0) !important;
    white-space: nowrap !important;
    border: 0 !important;
}

/* Responsive utilities */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.text-center { text-align: center; }
.text-left { text-align: left; }
.text-right { text-align: right; }

.d-block { display: block; }
.d-inline { display: inline; }
.d-inline-block { display: inline-block; }
.d-flex { display: flex; }
.d-grid { display: grid; }
.d-none { display: none; }

/* Spacing utilities */
.m-0 { margin: 0; }
.m-1 { margin: 0.25rem; }
.m-2 { margin: 0.5rem; }
.m-3 { margin: 1rem; }
.m-4 { margin: 1.5rem; }
.m-5 { margin: 3rem; }

.p-0 { padding: 0; }
.p-1 { padding: 0.25rem; }
.p-2 { padding: 0.5rem; }
.p-3 { padding: 1rem; }
.p-4 { padding: 1.5rem; }
.p-5 { padding: 3rem; }

/* Responsive display utilities */
@media (max-width: 767px) {
    .d-mobile-none { display: none; }
    .d-mobile-block { display: block; }
}

@media (min-width: 768px) {
    .d-tablet-none { display: none; }
    .d-tablet-block { display: block; }
}

@media (min-width: 1024px) {
    .d-desktop-none { display: none; }
    .d-desktop-block { display: block; }
}
```

### Debugging CSS
```css
/* 1. Border debugging */
* {
    border: 1px solid red;                  /* Temporary - shows all elements */
}

/* 2. Specific element debugging */
.debug {
    background-color: rgba(255, 0, 0, 0.1); /* Light red background */
    border: 2px solid red;
    position: relative;
}

.debug::before {
    content: "DEBUG";
    position: absolute;
    top: 0;
    left: 0;
    background: red;
    color: white;
    padding: 2px 4px;
    font-size: 10px;
}

/* 3. Grid debugging */
.grid-debug {
    background-image: 
        linear-gradient(rgba(255, 0, 0, 0.1) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255, 0, 0, 0.1) 1px, transparent 1px);
    background-size: 20px 20px;
}
```

### CSS Methodologies
```css
/* BEM (Block Element Modifier) */
.card { }                                   /* Block */
.card__header { }                           /* Element */
.card__body { }                             /* Element */
.card__footer { }                           /* Element */
.card--featured { }                         /* Modifier */
.card__header--large { }                    /* Element modifier */

/* OOCSS (Object-Oriented CSS) */
/* Structure */
.media {
    display: flex;
    align-items: flex-start;
}

.media__object {
    flex-shrink: 0;
    margin-right: 1rem;
}

.media__body {
    flex: 1;
}

/* Skin */
.media--reverse .media__object {
    order: 1;
    margin-left: 1rem;
    margin-right: 0;
}

/* Atomic CSS */
.mt-1 { margin-top: 0.25rem; }
.p-2 { padding: 0.5rem; }
.text-center { text-align: center; }
.bg-blue { background-color: blue; }
.text-white { color: white; }
```

---

## 🎯 Common Patterns & Components

### Navigation Menu
```css
/* Horizontal navigation */
.nav {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
}

.nav__item {
    margin-right: 2rem;
}

.nav__link {
    text-decoration: none;
    color: #333;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    transition: background-color 0.3s;
}

.nav__link:hover,
.nav__link--active {
    background-color: #f0f0f0;
}

/* Mobile hamburger menu */
.mobile-nav {
    display: none;
}

@media (max-width: 767px) {
    .nav {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 100%;
        left: 0;
        width: 100%;
        background: white;
        box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    
    .nav--active {
        display: flex;
    }
    
    .mobile-nav {
        display: block;
        background: none;
        border: none;
        font-size: 1.5rem;
        cursor: pointer;
    }
}
```

### Card Component
```css
.card {
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    overflow: hidden;
    transition: transform 0.3s, box-shadow 0.3s;
}

.card:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 8px rgba(0,0,0,0.15);
}

.card__image {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.card__content {
    padding: 1.5rem;
}

.card__title {
    margin: 0 0 0.5rem 0;
    font-size: 1.25rem;
    font-weight: 600;
}

.card__text {
    color: #666;
    line-height: 1.6;
    margin-bottom: 1rem;
}

.card__footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 1.5rem 1.5rem;
}
```

### Button Variations
```css
.btn {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    border: none;
    border-radius: 4px;
    text-decoration: none;
    text-align: center;
    cursor: pointer;
    font-size: 1rem;
    font-weight: 500;
    transition: all 0.3s;
    user-select: none;
}

.btn--primary {
    background-color: #3498db;
    color: white;
}

.btn--primary:hover {
    background-color: #2980b9;
}

.btn--secondary {
    background-color: #95a5a6;
    color: white;
}

.btn--outline {
    background-color: transparent;
    color: #3498db;
    border: 2px solid #3498db;
}

.btn--outline:hover {
    background-color: #3498db;
    color: white;
}

.btn--large {
    padding: 1rem 2rem;
    font-size: 1.2rem;
}

.btn--small {
    padding: 0.5rem 1rem;
    font-size: 0.9rem;
}

.btn:disabled {
    opacity: 0.6;
    cursor: not-allowed;
}
```

### Modal/Overlay
```css
.modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,0.5);
    z-index: 1000;
}

.modal--active {
    display: flex;
    align-items: center;
    justify-content: center;
}

.modal__content {
    background: white;
    border-radius: 8px;
    padding: 2rem;
    max-width: 500px;
    width: 90%;
    max-height: 80vh;
    overflow-y: auto;
    position: relative;
}

.modal__close {
    position: absolute;
    top: 1rem;
    right: 1rem;
    background: none;
    border: none;
    font-size: 1.5rem;
    cursor: pointer;
}
```

---

## 📚 Quick Reference Tables

### CSS Units
| Unit | Description | Example |
|------|-------------|---------|
| `px` | Pixels (absolute) | `font-size: 16px;` |
| `em` | Relative to parent font size | `padding: 1.5em;` |
| `rem` | Relative to root font size | `margin: 2rem;` |
| `%` | Percentage of parent | `width: 50%;` |
| `vw` | Viewport width | `width: 100vw;` |
| `vh` | Viewport height | `height: 100vh;` |
| `vmin` | Smaller viewport dimension | `font-size: 4vmin;` |
| `vmax` | Larger viewport dimension | `font-size: 4vmax;` |

### Common Breakpoints
| Device | Width | Media Query |
|--------|-------|-------------|
| Mobile | 320px - 767px | `@media (max-width: 767px)` |
| Tablet | 768px - 1023px | `@media (min-width: 768px)` |
| Desktop | 1024px+ | `@media (min-width: 1024px)` |
| Large Desktop | 1200px+ | `@media (min-width: 1200px)` |

### Flexbox Cheatsheet
| Property | Values | Description |
|----------|--------|-------------|
| `justify-content` | `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly` | Main axis alignment |
| `align-items` | `flex-start`, `flex-end`, `center`, `baseline`, `stretch` | Cross axis alignment |
| `flex-direction` | `row`, `row-reverse`, `column`, `column-reverse` | Main axis direction |
| `flex-wrap` | `nowrap`, `wrap`, `wrap-reverse` | Wrapping behavior |
| `flex-grow` | `0`, `1`, `2`, etc. | How much to grow |
| `flex-shrink` | `0`, `1`, `2`, etc. | How much to shrink |

### Grid Cheatsheet
| Property | Values | Description |
|----------|--------|-------------|
| `grid-template-columns` | `1fr 2fr 1fr`, `repeat(3, 1fr)` | Define columns |
| `grid-template-rows` | `100px auto 50px` | Define rows |
| `gap` | `10px`, `10px 20px` | Gap between items |
| `grid-column` | `1 / 3`, `span 2` | Column positioning |
| `grid-row` | `1 / 2`, `span 3` | Row positioning |
| `justify-content` | `start`, `end`, `center`, `stretch` | Grid alignment |
| `align-content` | `start`, `end`, `center`, `stretch` | Grid alignment |

---

## 🔥 Pro Tips & Tricks

### 1. CSS Reset vs Normalize
```css
/* CSS Reset (aggressive) */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* CSS Normalize (gentle) - use normalize.css library */
/* Preserves useful defaults, corrects bugs, improves consistency */
```

### 2. Modern CSS Features
```css
/* CSS Grid minmax() */
.grid {
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}

/* CSS Clamp() for responsive typography */
.responsive-text {
    font-size: clamp(1rem, 2.5vw, 2rem);
}

/* CSS aspect-ratio */
.video-container {
    aspect-ratio: 16 / 9;
}

/* CSS logical properties */
.modern-spacing {
    margin-inline: 1rem;        /* margin-left + margin-right */
    padding-block: 2rem;        /* padding-top + padding-bottom */
}
```

### 3. Performance Tips
```css
/* Use transform for animations */
.animate {
    transform: translateX(100px);   /* Good - uses GPU */
    /* left: 100px; */              /* Bad - causes reflow */
}

/* Contain property for optimization */
.card {
    contain: layout style paint;
}

/* Use will-change sparingly */
.heavy-animation {
    will-change: transform;
}

/* Remove will-change after animation */
.animation-complete {
    will-change: auto;
}
```

### 4. Debugging Techniques
```css
/* Outline debugging */
* { outline: 1px solid red; }

/* Background debugging */
div { background: rgba(255,0,0,0.1); }

/* Print debugging */
.debug::before {
    content: "Width: " attr(data-width);
}
```

---

## 🎨 Color Theory & Design

### Color Systems
```css
/* HSL (Hue, Saturation, Lightness) */
.color-hsl {
    color: hsl(210, 50%, 50%);          /* Blue */
    background: hsla(210, 50%, 50%, 0.8); /* Blue with transparency */
}

/* Color palette generation */
:root {
    --primary-hue: 210;
    --primary-saturation: 50%;
    
    --primary-50: hsl(var(--primary-hue), var(--primary-saturation), 95%);
    --primary-100: hsl(var(--primary-hue), var(--primary-saturation), 90%);
    --primary-200: hsl(var(--primary-hue), var(--primary-saturation), 80%);
    --primary-500: hsl(var(--primary-hue), var(--primary-saturation), 50%);
    --primary-900: hsl(var(--primary-hue), var(--primary-saturation), 10%);
}
```

### Typography Scale
```css
:root {
    --font-scale: 1.25;
    
    --font-xs: 0.75rem;
    --font-sm: 0.875rem;
    --font-base: 1rem;
    --font-lg: 1.125rem;
    --font-xl: 1.25rem;
    --font-2xl: 1.5rem;
    --font-3xl: 1.875rem;
    --font-4xl: 2.25rem;
    --font-5xl: 3rem;
}
```

---

## 📖 Learning Resources & Next Steps

### What to Practice Next:
1. **Build complete layouts** - Header, navigation, main content, sidebar, footer
2. **Create responsive components** - Cards, modals, forms, navigation menus
3. **Master CSS Grid and Flexbox** - Practice different layout patterns
4. **Learn CSS animations** - Hover effects, page transitions, micro-interactions
5. **Study design systems** - Consistency, spacing, typography, color palettes
6. **Explore CSS frameworks** - Bootstrap, Tailwind CSS, Bulma
7. **Learn CSS preprocessors** - Sass, Less for advanced functionality
8. **Practice accessibility** - Screen reader support, keyboard navigation, color contrast

### Common Interview Questions:
- Explain the CSS box model
- Difference between `display: block`, `inline`, and `inline-block`
- How does CSS specificity work?
- What are CSS pseudo-classes and pseudo-elements?
- Explain flexbox vs grid
- How do you make a website responsive?
- What are CSS custom properties?
- How do you center elements in CSS?

### Tools to Master:
- **Browser DevTools** - Inspecting, debugging, testing
- **CSS Validators** - W3C CSS Validator
- **Preprocessing** - Sass, Less, Stylus
- **Post-processing** - Autoprefixer, PostCSS
- **Build tools** - Webpack, Vite, Parcel
- **Design tools** - Figma, Adobe XD, Sketch

---

## 🎯 Final Notes

This cheatsheet covers the fundamentals to intermediate concepts of HTML and CSS. Remember:

- **Practice regularly** - Build projects, not just read theory
- **Focus on semantic HTML** - Use the right elements for the right content
- **Think mobile-first** - Design for small screens, then enhance for larger ones
- **Keep accessibility in mind** - Your websites should be usable by everyone
- **Stay updated** - Web standards evolve, keep learning new features
- **Use developer tools** - They're your best friend for debugging and learning

Happy coding! 🚀
