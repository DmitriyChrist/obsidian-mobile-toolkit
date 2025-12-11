## Description
This tutorial shows how to control the width of your notes in Obsidian by creating a CSS snippet and applying it selectively or globally.

### Creating a CSS Snippet for Wide Pages

First, create a new CSS snippet that defines a custom width class. Follow the [CSS snippets documentation](https://help.obsidian.md/snippets#Writing+CSS+for+Obsidian) for adding snippets to Obsidian.

Create a file named `wide-page.css` in your snippets folder with this code:

```css
.wide-page {
  --file-line-width: 100%;
}
```

This creates a reusable CSS class called `wide-page` that sets the line width to 100% of the available space.

### Applying to Specific Notes

To apply this width to individual notes, add the `cssclasses` property to the note's frontmatter or Properties panel:

```yaml
cssclasses:
  - wide-page
```

The note will now use the full width defined in your CSS snippet.

### Making Wide Pages Default

To apply full width to all notes permanently, add this code to your CSS snippet:

```css
.markdown-preview-sizer,
.markdown-source-view.mod-cm6.is-readable-line-width .cm-line,
.markdown-source-view.mod-cm6.is-readable-line-width .cm-content {
  width: var(--file-line-width, 100%);
}
```

This targets both reading and editing modes, making all notes use the full width by default. The `var(--file-line-width, 100%)` fallback ensures compatibility with the per-note class approach.

***
