---
title: "Markdown examples"
date: 2022-04-26T13:20:54-07:00
draft: false
---
This post provides a sample of commonly used Markdown formatting.<!--more-->

Chalk uses the default Hugo [syntax highlighting shortcode](https://gohugo.io/content-management/syntax-highlighting/#highlight-shortcode) `highlight`.

{{< highlight html >}}
<!-- This is a comment -->
<div class="grid">
  <h1>This is a heading</h1>
  <p>
    This is a paragraph text.
  </p>
</div>
{{< /highlight >}}

## Headings

Chalk includes 3 headings by default:

## Heading first level
### Heading second level
#### Heading third level

{{< highlight markdown >}}
## Heading first level
### Heading second level
#### Heading third level
{{< /highlight >}}

## Lists

Unordered list example:
* Unordered list item 1
* Unordered list item 2
* Unordered list item 3
* Unordered list item 4

Ordered list example:
1. Ordered list item 1
2. Ordered list item 1
3. Ordered list item 1
4. Ordered list item 1

{{< highlight markdown >}}
* Unordered list item 1
* Unordered list item 2

1. Order list item 1
2. Order list item 1
{{< /highlight >}}

## Emoji support :star:

Emoji's can be used everywhere in :cat2: your markdown!

Add `enableEmoji = true` to your config.toml file.

## Quotes

A quote looks like this:

> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna.

```markdown
> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna.
```

## Media

Images can be added with a default `<img>` tag.
If you wish that an image can be enlarged on click use the `image` shortcode. You can pass 3 variables:
- `path`: Image to show in the blog post.
- `path_detail`: Image to show when enlarging.
- `alt`: Alt text for image in blog post.

{{< image path="images/sample-image.jpeg" path_detail="images/sample-image@2x.jpeg" alt="Sample image" >}}

```markdown
{{</* image path="images/sample-image.jpeg" path_detail="images/sample-image@2x.jpeg" alt="Sample image" */>}}
```
