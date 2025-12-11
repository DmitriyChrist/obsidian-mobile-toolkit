## Description

This snippet highlights the active line number.
There is also an additional setting for the CSS Editor plugin to reduce differences between editors.
***
- author: DOChrist
- link: https://github.com/DmitriyChrist/Custom_Obs_journal_DOC
***
![](https://i.imgur.com/wMvLbCP.jpeg)
## Code

```css

.workspace-leaf-content[data-type="css-editor-view"] .cm-line {
 /*Text like text editor*/
 /* font-family: var(--font-text);
  font-size: var(--font-text-size);*/
  /*Text like code-block*/
  font-family: var(--font-monospace);
  font-size: var(--code-size);
}

/*styles for numberline*/
.cm-lineNumbers .cm-gutterElement {
  font-size: var(--font-ui-smaller) !important;
  font-family: var(--font-monospace) !important;
  /*color: var(--text-faint) !important;*/
  color: #888888 !important;
}

/*styles for active*/
.cm-gutterElement.cm-activeLineGutter,
.cm-gutterElement.cm-active {
  color: red !important;
}


/* background for active line */
.cm-active.cm-line {
  background-color: rgba(255, 255, 0, 0.15) !important;
}
```


