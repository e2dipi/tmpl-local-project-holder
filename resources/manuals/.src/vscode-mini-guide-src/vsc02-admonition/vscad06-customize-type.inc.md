<!-- markdownlint-disable MD041-->
Accoedin to to the previous section, getting your own custom types is then as simple as invoking your own *type* and defining the corresponding CSS class according to the desired look. For example, creating the "foo" *type* simply amounts to using the following markdown code:

```markdown
!!!foo The Foo Title This is the **foo** admonition body
```

and defining the corresponding CSS class to take control over the following HTML code:

```html
<div class="admonition foo">
<p class="admonition-title">The Foo Title</p>
<p>This is the <strong>foo</strong> admonition body</p>
</div>
```

The following CSS code snippet shows how to customize the look of the "foo" admonition:

```css
.admonition.foo {
    border: 1px solid #000000;
    border-radius: 0.5em;
    padding: 0.5em;
    margin: 1em 0;
    background-color: #f0f0f0;
    color: #000000;
}

.admonition.foo .admonition-title {
    font-weight: bold;
    text-transform: uppercase;
    font-size: 90%;
    margin: 0;
    padding: 0;
    border: 0;
    background-color: transparent;
    color: #000000;
}
```

<!-- markdownlint-enable MD041-->
