## Description

Place this code snippet in the note where you want all headers to be automatically collapsed upon opening.

***
- author: DOChrist
- link: https://github.com/DmitriyChrist/Custom_Obs_journal_DOC
***

## Code

````
```code-button
---
isRaw: true
---
const ctx = codeButtonContext;
// Execute command to collapse all headers
ctx.app.commands.executeCommandById('editor:fold-all');
```
````






