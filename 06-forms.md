---
course: html
slug: forms-basics
title: Basic Forms
description: "Forms let users enter information and send it to a website. Here's how to build a basic one."
---

## The form tag

Everything a user fills out and submits goes inside a `<form>` tag.

```html live
<form>
  <p>Form content goes here.</p>
</form>
```

## Label and input

`<input>` creates a field for the user to type into. `<label>` gives that field a visible name. Connect them using `for` on the label and a matching `id` on the input.

```html live
<form>
  <label for="username">Username</label>
  <input type="text" id="username" name="username">
</form>
```

**Result:**

<form>
  <label for="username">Username</label>
  <input type="text" id="username" name="username">
</form>

## What does it mean?

- `id="username"` on the input matches `for="username"` on the label — this links them together, so clicking the label focuses the input.
- `name="username"` is what identifies this field when the form is submitted.
- `type="text"` makes it a plain text field. Other common types: `email`, `password`, `number`.

## Placeholder

`placeholder` shows a light hint inside the field before the user types anything.

```html live
<form>
  <label for="email">Email</label>
  <input type="email" id="email" name="email" placeholder="you@example.com">
</form>
```

**Result:**

<form>
  <label for="email">Email</label>
  <input type="email" id="email" name="email" placeholder="you@example.com">
</form>

> [!NOTE]
> `placeholder` disappears once you start typing — never use it as a replacement for `<label>`.

## Try it yourself

Add a third field for phone number, with its own label, id, name, and placeholder.