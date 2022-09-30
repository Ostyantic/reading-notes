
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

## *Breakdown*

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

## Basic HTML structure

```
<!DOCTYPE HTML>
<html>
  <head>
  INFO FOR THE BROWSER GOES HERE, not visible
    <title>Website Title</title>
  </head>
  <body>
   CONTENT GOES HERE
  </body>
</html>
```

## **Semantics**

In programming, semantics refers to the meaning of a piece of code. Below are a few example of semantic elements:


`<h1>` - A top level header

`<p>` - A paragraph

`<img>` - An image

## **Wireframes**

### What is a wireframe?
It is a practice used to define and plan the structure of how a website, app, or product will look. This process focuses on how the designer or client wants the user to process information on a site. Think of wireframes as the blueprint to a website before it is built.

Example of wireframes taken from CareerFoundry student Samuel Adaramola:

![wireframe](https://dpbnri2zg3lc2.cloudfront.net/en/wp-content/uploads/old-blog-uploads/versions/samuel-student-wireframe---x----972-715x---.png)

## 6 steps to make a wireframe

1. Do your research
2. Prep your research for quick reference
3. Make sure you have your user flow mapped out
4. Draft, don't draw & Sketch, dont illustrate
5. Add some detail and get testing
6. Start turning your wireframes into prototypes

## 3 key wireframing principles

1. ***Clarity***
    - Your wireframe needs to answer the questions of what that site page is, what the user can do there, and if it satisfies their needs.
2. ***Confidence***
    - Ease of navigation through your site and clear calls-to-action increase user confidence in your brand.
3. ***Simplicity***
    - Too much information, copy, or links, can be distracting to the user
