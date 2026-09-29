---
course: html
slug: text-basics
title: Text Basics
description: "HTML gives you several ways to mark up text — headings, emphasis, line breaks, and notes to yourself that the browser ignores."
---

## Headings and paragraphs

HTML has six levels of headings, `<h1>` through `<h6>`, used to show the structure of your content — `<h1>` is the most important, `<h6>` the least. Regular text goes in a `<p>` (paragraph) tag.

```html live
<h1>Main heading</h1>
<h2>A smaller heading</h2>
<p>This is a regular paragraph of text.</p>
```

**Result:**

<h1>Main heading</h1>
<h2>A smaller heading</h2>
<p>This is a regular paragraph of text.</p>

## Adding emphasis

To make text stand out, use `<em>` for emphasis and `<strong>` for importance. Both usually render as italic and bold, but they mean something different to the browser and to screen readers — not just a visual style.

```html live
<p>You should <em>really</em> read this.</p>
<p>This step is <strong>required</strong> before continuing.</p>
```

**Result:**

<p>You should <em>really</em> read this.</p>
<p>This step is <strong>required</strong> before continuing.</p>

## What does it mean?

`<em>` tells the browser "the reader should stress this word" — it's read with vocal emphasis by screen readers, not just shown in italics. `<strong>` tells the browser "this is important," and is read with more weight, not just shown in bold.

You'll also come across `<u>`, which underlines text. It looks like a good way to underline for style, but it's not — `<u>` has a specific, narrow meaning (like marking a spelling mistake or a proper name), and browsers underline links by default too, so using `<u>` elsewhere can confuse readers into thinking your text is a link.

> [!NOTE]
> If you just want something to look underlined, that's a job for CSS (`text-decoration: underline`), not `<u>`. Save `<u>` for its actual purpose, not for styling.

## Line breaks and comments

`<br>` forces a line break inside text, without starting a new paragraph. It's self-closing — no `</br>` needed.

```html live
<p>Roses are red<br>Violets are blue</p>
```

**Result:**

<p>Roses are red<br>Violets are blue</p>

Comments let you leave notes in your code that the browser completely ignores — useful for explaining tricky bits, or temporarily "turning off" a line without deleting it.

```html live
<!-- This line won't show up on the page -->
<p>But this one will.</p>
```

> [!NOTE]
> Don't overuse `<br>` to create spacing between paragraphs — that's what CSS margins are for. `<br>` is for breaking a line within the same block of content, like an address or a poem.

## A few more useful tags

- `<small>` — for fine print, like disclaimers or copyright text
- `<mark>` — highlights text, like a highlighter pen
- `<sub>` and `<sup>` — subscript and superscript, useful for things like H₂O or x²
- `<blockquote>` — for quoting text from another source
- `<hr>` — draws a horizontal line, useful for separating sections

```html live
<p><small>© 2026 All rights reserved.</small></p>
<p>Don't forget to <mark>submit by Friday</mark>.</p>
<p>Water is H<sub>2</sub>O.</p>
<p>2<sup>3</sup> = 8</p>
<blockquote>The best way to learn HTML is by writing it.</blockquote>
<hr>
<p>Content after the divider.</p>
```

**Result:**

<p><small>© 2026 All rights reserved.</small></p>
<p>Don't forget to <mark>submit by Friday</mark>.</p>
<p>Water is H<sub>2</sub>O.</p>
<p>2<sup>3</sup> = 8</p>
<blockquote>The best way to learn HTML is by writing it.</blockquote>
<hr>
<p>Content after the divider.</p>

> [!NOTE]
> `<hr>` is self-closing, just like `<br>` — no closing tag needed.

## Try it yourself

Write a short paragraph about yourself. Make one word `<em>` and one word `<strong>`. Add a `<br>` to split a sentence onto two lines, and leave a comment above it explaining what you changed.