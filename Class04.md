
# **Structure web pages with HTML**

## What is HTML?

- Stands for ***Hypertext Markup Language***.

HTML is a markup language that define the structure of you content. It has different "elements", which you use to enclose, or wrap, different parts of the content to make it look or act a certain way.

## Why do we use HTML?

- To get content on the page for users to see
- To structure web pages
  - Tag and Elements make up the structure

**Example**:

![Element](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)

## *Breakdown*:

1. Opening tag - This consists of the name of the element. It is wrapped in opening and closing angle brackets and it basically states where the element begins. `<p>` is the paragraph element.

2. Content - This is the content of the element, which is just plain text in this case.

3. Closing tag - Similar to the opening tag, except it also has a forward slash, which is used to state the end of the element.

4. Element - The Opening & Closing tags and content in between all make this up.

Elements can even have attributes assigned to them which are use to add extra information without actually appearing as content.

**Example:**

![Attributes](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-attribute-small.png)

An attribute should **always** have the following:

  1. A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
  2. The attribute name followed by an equal sign.
  3. The attribute value wrapped by opening and closing quotation marks.

Element can be put inside other elements which is called **nesting**.

**Example**:
```
<p>I am <strong>soooo</strong> tired.</p>
``` 
