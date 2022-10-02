
# Design web pages with CSS

## What is CSS?

CSS stands for ***Cascading Style Sheets**. It is a rule based language that allows one to create great-looking web pages by styling elements in HTML to ones liking.

## What is CSS used for?

It is used for specifying how documents are presented to users in how they are style, laid out, etc. The documents are presented (converted into a form usuable by your audience) by browers (aka user agents), such as Firefox, Chrome, or MS Edge. CSS can do many things such as styling text (changing the color, font, size, etc.), turning a single column of text into a layout, used for creatign effects such as animation, and so much more! It's a really powerful tool once you get the hang of it!

## Syntax

Example

```
section p {
    color: red;
    font-size: 5em;
}
```

---

- CSS opens with a selector, in the above case the element `section p` (any element that has a paragraph element within a section element) is being selected to be styled.
- The selector is then followed by a set of curly braces `{ }`.
- Within the curly braces is one or more delcarations, which take the form of property and value pairs. The property `color` is identified before the colon `:` and given the value of `red` and ended with semi-colon `;`
- The property `font-size` is also identified and given the value of `5em`.

---

CSS [properties](https://css-tricks.com/almanac/properties/) have different allowable values depending on which property is being specified. In the example above is `color` property, which changes the color of text and the `font-size` property, which changes the size of the text.

## How to add CSS to your document

1. Create a file in the same folder as your HTML document and save it as `style.css`. The `.css` extension shows that this is a CSS file.
2. Link the `style.css` file to `index.html` somewhere in the `<head>` (I like to put it under `<title>`).

```
<link rel="stylesheet" href="styles.css" />
```

This `<link>` element tells the browser that we have a stylesheet, using the `rel` attribute, and the location of that stylesheet as the value of the `href` attribute.

### ***Three Ways to Insert CSS***

- External CSS

```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

- Internal CSS

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

- Inline CSS

```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

### ***Cascading Order***

What style will be used when there is more than one style specified for an HTML element?

All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default