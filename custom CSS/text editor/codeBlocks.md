## Description

my style
***
- author: DOChrist
- link: https://github.com/DmitriyChrist/Custom_Obs_journal_DOC
- initial idea:
***

## Code

```css
/*Code blocks*/
/* Reading mode */
.theme-dark .markdown-rendered pre {
  border: 1px solid var(--color-accent);
  border-radius: var(--radius-m);
  box-shadow: var(--shadow-lm-only);
  background: var(--code-background);
}

/* Live preview - start block */
.theme-dark .cm-s-obsidian div.HyperMD-codeblock-begin-bg {
  background: var(--code-background);
  border-top: 1px solid var(--color-accent);
  border-top-right-radius: 8px !important;
  border-top-left-radius: 8px !important;
  padding: 4px;
}

/* Live preview - end block */
.theme-dark .cm-s-obsidian div.HyperMD-codeblock-end-bg {
  background: var(--code-background);
  border-bottom: 1px solid var(--color-accent);
  border-bottom-right-radius: 8px;
  border-bottom-left-radius: 8px;
}

/* Live preview - body block */
.theme-dark .cm-s-obsidian div.HyperMD-codeblock-bg {
  border-right: 1px solid var(--color-accent);
  border-left: 1px solid var(--color-accent);
  background: var(--code-background);
}


/* Light theme */
.theme-light .markdown-rendered pre {
  border: 1px solid var(--color-accent);
  border-radius: var(--radius-m);
  box-shadow: var(--shadow-lm-only);
  background: var(--code-background);
}

.theme-light .cm-s-obsidian div.HyperMD-codeblock-begin-bg {
  background: var(--code-background);
  border-top: 1px solid var(--color-accent);
  border-top-right-radius: 8px !important;
  border-top-left-radius: 8px !important;
  margin-top: 8px;
}

.theme-light .cm-s-obsidian div.HyperMD-codeblock-end-bg {
  background: var(--code-background);
  border-bottom: 1px solid var(--color-accent);
  border-bottom-right-radius: 8px;
  border-bottom-left-radius: 8px;
}

.theme-light .cm-s-obsidian div.HyperMD-codeblock-bg {
  border-right: 1px solid var(--color-accent);
  border-left: 1px solid var(--color-accent);
  background: var(--code-background);
}
```


