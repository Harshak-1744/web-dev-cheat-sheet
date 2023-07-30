# web-dev-cheat-sheet

## HTML Cheat Sheet

## Document Structure

```html
<!DOCTYPE html>
<html>
<head>
  <title>Title of the Document</title>
</head>
<body>
  <!-- Content goes here -->
</body>
</html>
```

## Headings and Text

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>

<p>This is a paragraph.</p>

<blockquote>Quoted text here.</blockquote>

<pre>
  Preformatted text here.
  It preserves whitespace and line breaks.
</pre>

<abbr title="Hypertext Markup Language">HTML</abbr>

<address>
  Address details here.
</address>

<hr>
```

## Text Formatting

```html
<b>Bold Text</b>

<strong>Strong Importance</strong>

<i>Italic Text</i>

<em>Emphasized Text</em>

<u>Underlined Text</u>

<s>Strikethrough Text</s>

<sup>Superscript</sup>

<sub>Subscript</sub>

<mark>Highlighted Text</mark>

<del>Deleted Text</del>

<ins>Inserted Text</ins>

<small>Small Text</small>

<big>Big Text</big>

<code>Code Text</code>

<kbd>Keyboard Input</kbd>

<samp>Sample Output</samp>

<var>Variable</var>

<cite>Citation</cite>

<q>Inline Quote</q>
```

## Lists

```html
<ul>
  <li>Unordered List Item 1</li>
  <li>Unordered List Item 2</li>
</ul>

<ol>
  <li>Ordered List Item 1</li>
  <li>Ordered List Item 2</li>
</ol>

<dl>
  <dt>Definition Term 1</dt>
  <dd>Definition Description 1</dd>
  <dt>Definition Term 2</dt>
  <dd>Definition Description 2</dd>
</dl>
```

## Links and Anchors

```html
<a href="https://www.example.com">Link</a>
```

## Images and Multimedia

```html
<img src="image.jpg" alt="Image Description">

<figure>
  <img src="image.jpg" alt="Image Description">
  <figcaption>Image Caption</figcaption>
</figure>

<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

<video controls width="640" height="360">
  <source src="video.mp4" type="video/mp4">
  Your browser does not support the video element.
</video>
```

## Tables

```html
<table>
  <caption>Table Caption</caption>
  <thead>
    <tr>
      <th>Header Cell 1</th>
      <th>Header Cell 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data Cell 1</td>
      <td>Data Cell 2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Footer Cell 1</td>
      <td>Footer Cell 2</td>
    </tr>
  </tfoot>
</table>
```

## Forms

```html
<form>
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>
  <label for="password">Password:</label>
  <input type="password" id="password" name="password" required>
  <!-- Additional form elements go here -->
  <button type="submit">Submit</button>
  <button type="reset">Reset</button>
</form>
```

## Semantic Elements (HTML5)

```html
<details>
  <summary>Summary or Caption for Details</summary>
  Additional details or controls here.
</details>

<time datetime="2023-07-30">July 30, 2023</time>

<progress value="50" max="100">50%</progress>

<meter value="0.8">80%</meter>
```

---
