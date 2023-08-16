<!-- markdownlint-disable MD041-->
The HTML structure of an admonition consists of a  *division* container in which the header and every "chunk" of text in the body are considered as two separate *paragraphs*. Only the *division* and the title *paragraph*, are assigned a CSS class; the body *paragraph* is not. For example, the following `markdown code`:

```markdown
!!!note The Note Title is considered as a paragraph And so is also the note's body, with the dirrernce that is not assigned a CSS class. It is worth noting that the body can be made of several paragraphs, as shown below.
```

will generate *note* admonition with both a title and a body.  The corresponding HTML code will then consist three distinct `<p>` elements within a `<div>`. More precisely, the generated `HTML code` will be:

```html

<div class="admonition note">
<p class="admonition-title">The Note Title is considered as a paragraph</p>
<p>And so is also the note's body, with the dirrernce that is not assigned a CSS class.</p>
<p>It is worth noting that the body can be made of several paragraphs, as shown below.</p>
</div>

```
<!-- markdownlint-enable MD041-->
