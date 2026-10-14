# HTML Beginner Study Notes (Part 1)

> Designed for a **0-knowledge student**. This explains **what every tag is, why it exists, how it works, when to use it, common mistakes, SEO meaning, and visual behavior.**

---

# 1. `<!DOCTYPE html>`

## Definition
`<!DOCTYPE html>` tells the browser:

> **"This document is written using the HTML5 standard."**

It is **not an HTML tag**. It is a declaration.

## Why is it needed?

Browsers have two rendering modes:

1. **Standards Mode** ✅ (modern behavior)
2. **Quirks Mode** ❌ (old browser compatibility mode)

Without `<!DOCTYPE html>`, many browsers switch to **Quirks Mode**, where layouts and CSS may behave differently.

## What version is used without DOCTYPE?

There is **no default HTML version**.

Instead, browsers assume an old compatibility mode that behaves similarly to very old HTML (HTML 4-era behavior). That is why every modern page starts with:

```html
<!DOCTYPE html>
```

---

# 2. `<html>`

## Definition

This is the **root element** of every HTML page.

Everything belongs inside it.

```html
<html lang="en">

</html>
```

---

## `lang="en"`

### Definition

Tells browsers, screen readers, and search engines what language the page uses.

Example

```html
<html lang="en">
<html lang="hi">
<html lang="gu">
<html lang="fr">
```

### Why?

Search engines understand the language.

Screen readers pronounce words correctly.

Translation tools work better.

---

# What is SEO?

**SEO = Search Engine Optimization**

SEO means making your website easier for search engines like Google or Bing to understand so it can appear higher in search results.

Good HTML helps SEO.

Examples:

- meaningful headings
- `<strong>`
- `<em>`
- `alt`
- `title`
- language
- metadata

---

# 3. `<head>`

## Definition

The `<head>` contains information **about the webpage**, not information shown on the webpage.

Think of it like a student's identity card.

The identity card contains:

- name
- class
- roll number

but those details are not the student.

Similarly, `<head>` contains information about the webpage.

Typical contents:

- `<title>`
- `<meta>`
- CSS
- JavaScript
- favicon

---

# 4. `<meta>`

## Definition

Meta means **metadata**.

Metadata means:

> "Information about information."

The user usually cannot see meta tags, but browsers and search engines use them.

---

## `charset="UTF-8"`

```html
<meta charset="UTF-8">
```

### What is Character Encoding?

A computer stores only numbers.

Character encoding tells the browser which number represents which character.

Example

65 → A

97 → a

8364 → €

Without encoding the browser may display garbage text.

---

## What is UTF-8?

UTF = **Unicode Transformation Format**

UTF-8 is the world's most common character encoding.

It supports almost every language.

Examples it supports:

English

```
Hello
```

Hindi

```
नमस्ते
```

Gujarati

```
નમસ્તે
```

Japanese

```
こんにちは
```

Chinese

```
你好
```

Emoji

😀 ❤️ 🎉

Indian Rupee

₹

Without UTF-8 these may become unreadable symbols.

---

## Viewport

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### Why?

Phones have small screens.

Laptops have large screens.

Viewport tells the browser:

> "Display this page according to the device width."

### `width=device-width`

Use the full width of the current device.

### `initial-scale=1.0`

Initial zoom should be 100%.

Without viewport:

- text may appear tiny
- users must zoom manually
- page is not mobile friendly

---

# 5. `<title>`

Appears on:

- browser tab
- bookmarks
- search engine result title

Good titles improve SEO.

---

# 6. `<body>`

Everything visible goes inside `<body>`.

---

# 7. `<p>`

## Definition

Paragraph tag.

It is for normal text paragraphs.

### Why create `<p>` when normal text works?

Because browsers need to know:

"This is one complete paragraph."

That helps:

- spacing
- accessibility
- SEO
- screen readers

### Whitespace behavior

HTML collapses spaces.

```html
<p>Hello          World</p>
```

Output

```
Hello World
```

Even 20 spaces become one space.

Also:

```html
<p>
Hello


World
</p>
```

Output

```
Hello World
```

Extra Enter and spaces are ignored.

### Visual spacing

Each `<p>` automatically starts on a new line and has top/bottom margin.

Example

```html
<p>First</p>
<p>Second</p>
```

Output

First

(blank space)

Second

---

# 8. `<pre>`

## Definition

Pre = Preformatted Text.

Unlike `<p>`, it keeps everything exactly as typed.

### Comparison

`<p>`

Input

```
Hello      World
```

Output

```
Hello World
```

`<pre>`

Input

```
Hello      World
```

Output

```
Hello      World
```

Spaces, tabs and line breaks are preserved.

Use it for:

- poems
- source code
- ASCII art
- formatted text

---

# 9. `<strong>` vs `<b>`

Both look bold.

Difference:

`<b>`

Only changes appearance.

`<strong>`

Changes appearance **and** tells browsers/search engines:

"This text is important."

Better for accessibility and SEO.

---

# 10. `<em>` vs `<i>`

Both usually look italic.

`<i>`

Only italic styling.

`<em>`

Means emphasis.

Screen readers may change voice stress when reading `<em>`.

Better semantic meaning.

---

# 11. `<address>`

Contains contact information.

Examples:

- company address
- author email
- phone number

Usually appears italic.

Do not use it for random home addresses unless it represents contact information.

---

# 12. `<a>`

Creates hyperlinks.

Syntax

```html
<a href="https://example.com" target="_blank">Visit</a>
```

Important attributes

## href

Destination.

Without href the anchor is not a normal clickable link.

## target

`_blank`

Open new tab.

`_self`

Same tab (default).

---

# 13. `<img>`

```html
<img src="cat.jpg" alt="White cat" width="200" height="150">
```

Important attributes

## src

Location of image.

## alt

Alternative text.

Shown if image fails to load.

Also read by screen readers.

Important for accessibility and SEO.

## width / height

Controls displayed image size.

---

# 14. `<iframe>`

Embeds another webpage or resource.

Examples:

- YouTube
- Google Maps
- PDF
- Another webpage

Syntax

```html
<iframe src="page.html" width="500" height="300"></iframe>
```

Common errors

Many websites refuse embedding.

Reasons:

- `X-Frame-Options`
- `Content-Security-Policy`

Instead of loading, you may see:

- blank page
- connection refused
- page blocked

This is normal.

---

# 15. Lists

## Ordered List

```html
<ol>
 <li>One</li>
 <li>Two</li>
</ol>
```

Produces numbered list.

---

## Unordered List

```html
<ul>
 <li>Apple</li>
 <li>Mango</li>
</ul>
```

Produces bullets.

---

## `<li>`

Represents one item.

Must be inside `<ol>` or `<ul>`.

---

# 16. Description List

```html
<dl>
 <dt>HTML</dt>
 <dd>HyperText Markup Language</dd>
</dl>
```

## `<dl>`

Description List container.

## `<dt>`

Description Term.

## `<dd>`

Definition of that term.

Think of a dictionary.

Word → Meaning.

---

# 17. `<marquee>`

⚠ IMPORTANT

`<marquee>` is **deprecated**.

It is **NOT part of HTML5**.

Old browsers supported it.

Modern websites use CSS animations or JavaScript instead.

Do not use `<marquee>` in new projects.

---

# Revision Tips

- `<p>` = paragraph (spaces collapse)
- `<pre>` = preserve spaces exactly
- `<b>` = bold only
- `<strong>` = bold + important
- `<i>` = italic only
- `<em>` = italic + emphasis
- `<ol>` = numbered list
- `<ul>` = bullet list
- `<li>` = list item
- `<dt>` = word
- `<dd>` = meaning
- `<iframe>` = embed another resource
- `<img alt>` = accessibility + SEO
- `UTF-8` = universal character encoding
- `viewport` = mobile responsiveness
