# HTML
HTML stands for HyperText Markup Language.

- HyperText = links between pages.
- Markup Language = a way to mark or label parts of a page (like headings, paragraphs, images).

Think of HTML as the skeleton of a webpage.
It tells the browser what to show — like &quot;this is a heading&quot;, &quot;this is a paragraph&quot;, &quot;this is an image&quot;. Use tags (like &lt;h1&gt;, &lt;p&gt;, &lt;img&gt;) to mark different parts.

Note: HTML = &quot;How To Make Layout&quot;. It helps lay out the structure of a webpage.

#### **HTML Document**
An HTML document is just a file (usually ending with .html) that contains HTML code.
It is the full page that the browser reads to show a website.

It’s like the recipe that tells the browser how to build and display a webpage.

Basic structure of an HTML document
```
&lt;!DOCTYPE html&gt;
&lt;html&gt;
  &lt;head&gt;
    &lt;title&gt;Page Title&lt;/title&gt;
  &lt;/head&gt;
  &lt;body&gt;
    &lt;h1&gt;Hello, World!&lt;/h1&gt;
    &lt;p&gt;Welcome to my website!&lt;/p&gt;
  &lt;/body&gt;
&lt;/html&gt;
```

* `&lt;!DOCTYPE html&gt; `
  Tells the browser: "Hey, this is an HTML5 document!". Without   this line, the browser might get confused and display the page wrongly. It's like telling the browser what language you're speaking. The &lt;!DOCTYPE&gt; declaration is not case sensitive.

* `&lt;html&gt;` : 
  Start of the webpage. Everything you want to show or set up must be inside &lt;html&gt; and &lt;/html&gt;. It's like a container for the whole page.

* `&lt;head&gt;` :
  Contains meta information about the HTML page. it include page title, link to css, link to icons

* `&lt;title&gt;` : 
  Sets the name that appears on the browser's tab. If you write `&lt;title&gt;`My Website`&lt;/title&gt;`, then the browser tab will show "My Website".

* `&lt;body&gt;` : 
  Visible part of the page. Whatever you write inside &lt;body&gt; (headings, text, images, videos, buttons) — people can see it when they visit the site.

-----

#### **HTML Element**
An HTML element is defined by a start tag, some content, and an end tag.

Never skip the end tag, some elemets display correctly even if we forget. However, never rely on this Unexpected results and errors may occur if you forget the end tag.

HTML tags are not case sensitive, `&lt;P&gt; means the same as &lt;p&gt;`. Recommends lowercase in HTML.

```
&lt;p&gt;Hello, world!&lt;/p&gt;
```
Think of an element like a sandwich. The top bread = start tag (`&lt;p&gt;`), The filling = content ("Hello, world!") and The bottom bread = end tag (`&lt;/p&gt;`).

#### **Types of HTML Elelments**
There are two types of html elements : Container Elements and Empty Elements.

1. Container Elements : 
  Have both a start tag and an end tag. Ex, `&lt;p&gt;`Paragraph text`&lt;/p&gt;`

2. Empty Elements : 
  Only have a start tag (no content, no end tag). Ex, `&lt;img src="image.jpg" alt="Picture"&gt;`
`&lt;br&gt;` (line break), `&lt;hr&gt;` (horizontal line)

#### **Nested HTML Elements**
 Nested means one element is placed inside another element. In HTML, when you put one element inside another, it’s called nesting.
```
&lt;p&gt;This is a &lt;strong&gt;very important&lt;/strong&gt; message.&lt;/p&gt;

&lt;p&gt; : parent element (paragraph)
&lt;strong&gt; : child element (makes the text bold)
```

```
&lt;div&gt;
  &lt;h1&gt;My Blog&lt;/h1&gt;
  &lt;p&gt;Welcome to my blog. Enjoy &lt;em&gt;reading&lt;/em&gt; the posts!&lt;/p&gt;
&lt;/div&gt;
```

Rules of Nesting : 

* Always close inner elements first.
* Keep it clean and properly indented to make it easy to read.
-----

#### **HTML Attributes**
Attributes are extra information that you add to an HTML element. They help control or modify how an element behaves or looks.
```
&lt;tagname attributeName="value"&gt;Content&lt;/tagname&gt;
```
Attributes are always inside the start tag. Attributes are name-value pairs: name="value". You can have multiple attributes in one tag.
```
&lt;a href="https://google.com" target="_blank" title="Visit Google"&gt;Google&lt;/a&gt;
```

**href attribute**

Sets where a link should go (the URL). ```&lt;a href="https://google.com"&gt;Visit Google&lt;/a&gt;```. When you click "Visit Google", it opens Google.

**src attribute**

Tells which image file to display. ```&lt;img src="cat.jpg" alt="Cute Cat"&gt;```. Show cat picture.

**width and height**

Set the size of an image. ```&lt;img src="cat.jpg" width="300" height="200" alt="Cute Cat"&gt;```. Image will be 300 pixels wide and 200 pixels tall.

**alt attribute**

Shows alternative text if the image can't load. ```&lt;img src="missing.jpg" alt="Image not found"&gt;```. If the image is missing, "Image not found" is shown.

**style attribute**

Adds CSS styles like color, font size, background, etc. ```&lt;p style="color:blue; font-size:20px;"&gt;Hello World!&lt;/p&gt;```.The text "Hello World!" will be blue and bigger.

**lang attribute**

Declares the language of the page (for browsers and search engines). ```&lt;html lang="en"&gt;```. Page is written in english.

**title attribute**

Shows extra information when you hover the mouse over the element.```&lt;p title="This is a paragraph."&gt;Hover over me!&lt;/p&gt;```. When you hover your mouse, a tooltip "This is a paragraph." appears.

----

#### **HTML Headings**
Headings are used to give titles to sections of a web page.

Types of Headings
There are 6 levels of headings in HTML:

```
&lt;h1&gt; → Biggest and most important heading
&lt;h2&gt; → Second most important
&lt;h3&gt; → Third most important
&lt;h4&gt; → Fourth
&lt;h5&gt; → Fifth
&lt;h6&gt; → Smallest and least important heading
```

Imagine a Newspaper : 
- Main Title = &lt;h1&gt; (e.g., "Today's Top News")
- Section Title = &lt;h2&gt; ("Sports", "Weather", "Politics")
- Smaller Story Title = &lt;h3&gt;, &lt;h4&gt;, etc.

----

#### **HTML Paragraphs**
A paragraph in HTML is used to write normal text — like sentences, descriptions, articles, etc. Use the &lt;p&gt; tag to create a paragraph.

A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.
```
&lt;-- single paragraph --&gt;

&lt;p&gt;This is my first paragraph in HTML!&lt;/p&gt;
```

```
&lt;!-- multiple paragraph --&gt;

&lt;p&gt;HTML is very easy to learn.&lt;/p&gt;
&lt;p&gt;It is used to create web pages.&lt;/p&gt;
&lt;p&gt;Each paragraph is a separate block of text!&lt;/p&gt;
```

**`&lt;hr&gt;` : Horizontal Line**

`&lt;hr&gt;` stands for Horizontal Rule. It draws a horizontal line across the web page. It is used to separate sections of content. It does not need a closing tag. (&lt;hr&gt; alone is enough).

```
&lt;!-- line will appear between the two paragraphs --&gt;

&lt;h1&gt;Welcome to My Website&lt;/h1&gt;
&lt;p&gt;This is the first section.&lt;/p&gt;

&lt;hr&gt;

&lt;p&gt;This is the second section, separated by a line.&lt;/p&gt;
```

**`&lt;br&gt;` : Line Break**

`&lt;br&gt;` stands for Break (line break). It moves the next text to a new line without starting a new paragraph. It also does not need a closing tag. (&lt;br&gt; alone!)
```
&lt;p&gt;Hello &lt;br&gt;How are you Joshi? &lt;br&gt; Have a nice day! &lt;/p&gt;
```

**`&lt;pre&gt;` : Preformatted Text**

It is used to display text exactly as you type it. This means:Spaces and line breaks are preserved.The text is shown in a monospace font (like code). It’s typically used for displaying things like code snippets or ASCII art.
```
&lt;pre&gt;
This is some preformatted text.
  It keeps all spaces and line breaks.
  Useful for displaying code or ASCII art.
&lt;/pre&gt;
```
----

#### **HTML Styles**

HTML Styles allow you to change the look and feel of your web page, things like color, font size, background, margins, and more.

Styles are added in three main ways:
  * Inline styles
  * Internal styles
  * External styles

**1. Inline Styles**

You can add styles directly to an element using the style attribute. It’s called inline because the style is written inside the HTML tag itself.

```
&lt;!-- syntax --&gt;
&lt;tag style="property:value;"&gt;

&lt;!-- example --&gt;
&lt;p style="color: red; font-size: 20px;"&gt;This is a red paragraph with big text!&lt;/p&gt;
```

**2. Internal Styles**

You can add styles in the head section of your HTML document using the &lt;style&gt; tag. These styles will apply to the whole page.

```
&lt;!-- syntax --&gt;
&lt;head&gt;
  &lt;style&gt;
    /* CSS rules go here */
  &lt;/style&gt;
&lt;/head&gt;


&lt;!-- example --&gt;
&lt;head&gt;
  &lt;style&gt;
    p {
      color: green;
      font-size: 18px;
    }
  &lt;/style&gt;
&lt;/head&gt;

&lt;body&gt;
  &lt;p&gt;This paragraph is green with 18px font size.&lt;/p&gt;
&lt;/body&gt;
```

**3. External Styles**

You can use a separate CSS file to define your styles. This way, you keep HTML and CSS separate and more organized.

```
&lt;!-- syntax --&gt;
&lt;head&gt;
  &lt;link rel="stylesheet" href="styles.css"&gt;
&lt;/head&gt;

&lt;!-- styles.css --&gt;
p{
  color: blue;
  font-size: 16px;
}
```

| Property             | What It Does                                             | Example                        |
|----------------------|----------------------------------------------------------|--------------------------------|
| `color`              | Changes the text color                                   | `color: red;`                  |
| `font-size`          | Changes the font size                                    | `font-size: 18px;`             |
| `background-color`   | Changes the background color of an element              | `background-color: yellow;`    |
| `font-family`        | Changes the font style                                   | `font-family: Arial, sans-serif;` |
| `margin`             | Adds space outside the element                           | `margin: 20px;`                |
| `padding`            | Adds space inside the element                            | `padding: 10px;`               |
| `border`             | Adds a border around an element                          | `border: 1px solid black;`     |

---
----

#### **HTML Text Formatting**

In HTML, text formatting refers to how text appears on the web page. You can modify its style, structure, and layout using various HTML tags and attributes.

**1. `&lt;b&gt;` : Bold Text**

  Makes the text bold. ``` &lt;b&gt;This text is bold.&lt;/b&gt;```

**2. `&lt;strong&gt;` : Strong Emphasis (Bold)**

Indicates strong emphasis, typically shown as bold in browsers.
&lt;strong&gt; is semantically meaningful and indicates importance, while &lt;b&gt; just makes text bold without any meaning. ```&lt;strong&gt;This is strongly emphasized text (bold).&lt;/strong&gt;```

**3. &lt;i&gt; : Italic Text**

Makes the text italic. ```&lt;i&gt;This text is italic.&lt;/i&gt;```

**4. &lt;em&gt; : Emphasized Text (Italic)**

Indicates emphasis, usually displayed in italic in browsers.&lt;em&gt; conveys meaning (emphasis), while &lt;i&gt; just styles the text. ```&lt;em&gt;This text is emphasized (italic).&lt;/em&gt;```

**5. &lt;u&gt; : Underlined Text**

Underlines the text. ```&lt;u&gt;This text is underlined.&lt;/u&gt;```

**6. &lt;mark&gt; : Highlighted Text**

Highlights the text by changing the background color. ```&lt;mark&gt;This text is highlighted.&lt;/mark&gt;```.

**7. &lt;small&gt; : Smaller Text**

Makes the text smaller than the surrounding text. ```&lt;small&gt;This text is smaller.&lt;/small&gt;```

**8. &lt;sub&gt; : Subscript Text**

Displays text as subscript (below the baseline). ```H&lt;sub&gt;2&lt;/sub&gt;O```. This will display H₂O where the "2" is subscripted.

**9. &lt;sup&gt; : Superscript Text**

Displays text as superscript (above the baseline). ```E = mc&lt;sup&gt;2&lt;/sup&gt;```. This will display E = mc², with the "2" as a superscript.

**10. &lt;del&gt; : Deleted Text**

Indicates deleted text (typically shown with a strikethrough). ```&lt;del&gt;This text is deleted.&lt;/del&gt;```. 

**11. &lt;ins&gt; — Inserted Text**

Indicates inserted text (typically shown with an underline). ```&lt;ins&gt;This text is inserted.&lt;/ins&gt;```.


| Tag            | What It Does                                            | Example                                   |
|----------------|---------------------------------------------------------|-------------------------------------------|
| `&lt;b&gt;`          | Makes the text bold                                     | `&lt;b&gt;Bold text&lt;/b&gt;`                        |
| `&lt;strong&gt;`     | Strong emphasis (typically bold)                        | `&lt;strong&gt;Important text&lt;/strong&gt;`         |
| `&lt;i&gt;`          | Italicizes the text                                    | `&lt;i&gt;Italic text&lt;/i&gt;`                      |
| `&lt;em&gt;`         | Emphasizes text (typically italic)                      | `&lt;em&gt;Emphasized text&lt;/em&gt;`                |
| `&lt;u&gt;`          | Underlines the text                                    | `&lt;u&gt;Underlined text&lt;/u&gt;`                  |
| `&lt;s&gt;`          | Adds a strikethrough to the text                        | `&lt;s&gt;Strikethrough text&lt;/s&gt;`               |
| `&lt;mark&gt;`       | Highlights text                                         | `&lt;mark&gt;Highlighted text&lt;/mark&gt;`           |
| `&lt;small&gt;`      | Makes text smaller                                      | `&lt;small&gt;Small text&lt;/small&gt;`               |
| `&lt;sub&gt;`        | Makes text subscript                                    | `H&lt;sub&gt;2&lt;/sub&gt;O`                          |
| `&lt;sup&gt;`        | Makes text superscript                                  | `E = mc&lt;sup&gt;2&lt;/sup&gt;`                      |
| `&lt;del&gt;`        | Indicates deleted text                                  | `&lt;del&gt;Deleted text&lt;/del&gt;`                 |
| `&lt;ins&gt;`        | Indicates inserted text                                 | `&lt;ins&gt;Inserted text&lt;/ins&gt;`                |
| `&lt;code&gt;`       | Represents inline code                                  | `&lt;code&gt;let x = 5;&lt;/code&gt;`                 |
| `&lt;pre&gt;`        | Displays preformatted text                              | `&lt;pre&gt;Preformatted text&lt;/pre&gt;`            |
| `&lt;blockquote&gt;` | Defines a block quote                                   | `&lt;blockquote&gt;Quoted text&lt;/blockquote&gt;`    |
| `&lt;q&gt;`          | Defines a short inline quote                            | `&lt;q&gt;Short quote&lt;/q&gt;`                      |
| `&lt;span&gt;`       | Generic inline container for styling                    | `&lt;span&gt;Styled text&lt;/span&gt;`                |
| `&lt;br&gt;`         | Adds a line break                                       | `&lt;br&gt;`                                    |

---

----

#### **HTML Comments**
HTML comments are used to add explanatory notes or comments within the code, which are not displayed on the web page. They are helpful for documenting the code, explaining sections of HTML, or leaving reminders for future development.

```
&lt;!-- This is a comment --&gt;
```

Example for understanding comment
```
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
    &lt;title&gt;HTML Comments Example&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;

    &lt;!-- This is the main heading --&gt;
    &lt;h1&gt;Welcome to My Website&lt;/h1&gt;

    &lt;!-- This section contains the navigation menu --&gt;
    &lt;nav&gt;
        &lt;ul&gt;
            &lt;li&gt;&lt;a href="#"&gt;Home&lt;/a&gt;&lt;/li&gt;
            &lt;li&gt;&lt;a href="#"&gt;About&lt;/a&gt;&lt;/li&gt;
            &lt;li&gt;&lt;a href="#"&gt;Services&lt;/a&gt;&lt;/li&gt;
            &lt;li&gt;&lt;a href="#"&gt;Contact&lt;/a&gt;&lt;/li&gt;
        &lt;/ul&gt;
    &lt;/nav&gt;

    &lt;!-- This paragraph contains some basic text --&gt;
    &lt;p&gt;Here is a simple paragraph of text.&lt;/p&gt;

    &lt;!-- Remember to update the footer section later --&gt;
    &lt;footer&gt;
        &lt;p&gt;Footer information goes here.&lt;/p&gt;
    &lt;/footer&gt;

&lt;/body&gt;
&lt;/html&gt;
```

**Hide Content**

HTML comments can be used to temporarily hide content. While it is not a method for dynamically hiding content during runtime like CSS or JavaScript, it can be useful when you want to disable certain parts of your code for testing or debugging without removing them entirely.

```
&lt;!-- This content is hidden and will not be displayed in the browser --&gt;
&lt;p&gt;This paragraph will be hidden because it is inside a comment.&lt;/p&gt;
```

**Hide Inline Content**

 HTML comments can be used to hide inline content anywhere within your HTML code, including in the middle of elements or between text. This is useful when you want to temporarily disable part of your content, such as a specific paragraph, image, or text, without deleting it.
```
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;title&gt;Hide Inline Content Example&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;

    &lt;h1&gt;Welcome to My Website&lt;/h1&gt;
    
    &lt;p&gt;This is a visible paragraph of text.&lt;/p&gt;

    &lt;!-- &lt;p&gt;This paragraph is hidden inline and won't be displayed.&lt;/p&gt; --&gt;

    &lt;p&gt;This is another visible paragraph.&lt;/p&gt;

    &lt;p&gt;&lt;strong&gt;This is bold text.&lt;/strong&gt; &lt;!-- This part of text is hidden --&gt; More text here.&lt;/p&gt;

&lt;/body&gt;
&lt;/html&gt;
```

----

#### **HTML Links**

HTML links are created using the &lt;a&gt; (anchor) element. The &lt;a&gt; element is used to define hyperlinks, which allow users to click and navigate to another webpage, section of the same page, or external resource.

By default, links will appear as follows in all browsers:
- An unvisited link is underlined and blue
- A visited link is underlined and purple
- An active link is underlined and red

```
&lt;!-- syntax --&gt;
&lt;a href="URL"&gt;Link Text&lt;/a&gt;

&lt;!-- example : In this example, the user will be directed to "https://www.example.com" when they click on the text "Visit Example Website." --&gt;

&lt;a href="https://www.example.com"&gt;Visit Example Website&lt;/a&gt;
```

**Types of Links**

**1. External Links**

Links that point to a different website or domain.
```
&lt;a href="https://www.google.com"&gt;Go to Google&lt;/a&gt;
```
When clicked, this will take the user to the Google homepage.

**2.Internal Links**

Links that navigate within the same website or domain.
```
&lt;a href="/about.html"&gt;About Us&lt;/a&gt;
```
Clicking this link will navigate the user to the about.html page within the same website.

**3. Anchor Links (Internal Navigation)**

Links that point to a specific part of the same page, often used for navigation within long pages.
```
&lt;a href="#section2"&gt;Go to Section 2&lt;/a&gt;
```
This would navigate the user to an element on the page with the id="section2", like this:
```
&lt;div id="section2"&gt;This is Section 2&lt;/div&gt;
```

**4. Email Links**

Links that allow the user to open their default email client and send an email.
```
&lt;a href="mailto:someone@example.com"&gt;Send an Email&lt;/a&gt;
```
Clicking this link will open the user's email client with the recipient's email pre-filled.

**5. Phone Links**

Links that initiate a phone call on mobile devices.
```
&lt;a href="tel:+1234567890"&gt;Call Us&lt;/a&gt;
```
On a mobile device, this would trigger the phone dialer with the given phone number.

Example of Multiple Links
```
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;title&gt;HTML Links Example&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;h1&gt;Welcome to My Website&lt;/h1&gt;
    &lt;p&gt;Click the links below to navigate:&lt;/p&gt;
    
    &lt;a href="https://www.google.com"&gt;Go to Google&lt;/a&gt;&lt;br&gt;
    &lt;a href="/about.html"&gt;About Us&lt;/a&gt;&lt;br&gt;
    &lt;a href="#contact"&gt;Go to Contact Section&lt;/a&gt;&lt;br&gt;
    &lt;a href="mailto:someone@example.com"&gt;Send an Email&lt;/a&gt;&lt;br&gt;
    &lt;a href="tel:+1234567890"&gt;Call Us&lt;/a&gt;
    
    &lt;h2 id="contact"&gt;Contact Section&lt;/h2&gt;
    &lt;p&gt;Here is the contact information.&lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;
```
