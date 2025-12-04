## Description

## Obsidian Image Caption Numbering Snippet

This CSS snippet automatically numbers image captions in Obsidian notes, displaying them as "Fig 1. Caption text" below each embedded image.

## Key Features
- Works in **Reading View**, **Live Preview**, and **mobile devices**
- Sequential numbering across the entire note (Fig 1, Fig 2, etc.)
- Styled captions with centered text and accent color
- Supports Obsidian's embedded image syntax `![[image.png|caption]]`

## Usage Syntax

**Basic caption:**
```
![[test.png|test caption]]
or
![test caption](test.png)
```

**Caption + custom size:**
```
![[test.png|test caption|150]] 
or
![test caption|250](test.png)
```



***
- author: DOChrist
- link: https://github.com/DmitriyChrist/Custom_Obs_journal_DOC
***
![](https://i.imgur.com/ecIDKHL.jpeg)
![](https://i.imgur.com/hykbkC6.jpeg)
## Code

```css
/* Counter for Reading mode */
.markdown-reading-view,
.markdown-preview-view {
    counter-reset: figure-counter;
}

/* Counter for Live Preview */
.markdown-source-view.mod-cm6 .cm-content {
    counter-reset: figure-counter;
}

/* Increment on each image */
.image-embed {
    counter-increment: figure-counter;
}

/* Caption with numbering */
.image-embed[alt]::after {  
    content: "Fig " counter(figure-counter) ". " attr(alt);  
    display: block;  
    margin: 0.2rem 1rem 1rem 1rem;  
    font-size: 90%;  
    line-height: 1.4;  
/* color: var(--text-faint); */ 
    color: var(--text-accent);  
    text-align: center;  
}
```


