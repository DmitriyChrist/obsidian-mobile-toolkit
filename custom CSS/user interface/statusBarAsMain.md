## Description

I use it as the main bar. Additional commands are created through the Commander plugin.  
Note: Since icons of Core plugins appear in the status bar by default, you can disable them either in the settings or hide them using the Commander plugin.  
Tip: If you activate "Show editing mode in status bar" in Settings => Editor, a default icon for switching modes (Reading, Preview, and Source) will appear in this status bar.


***
- author: DOChrist
- link: https://github.com/DmitriyChrist/Custom_Obs_journal_DOC
- init idea: https://forum.obsidian.md/t/css-to-show-status-bar-on-mobile-devices/77185

***



## Code

```css

/*Custom status-bar*/
.app-container .status-bar {
  display: flex;
  position: fixed;
  bottom: 23vh;
  background: none !important;
  z-index: var(--layer-cover);
  transform-origin:  right top;
  transform: rotate(90deg);
  border: none;
    /*border: orange 2px solid;*/
}

.app-container .status-bar .svg-icon {
    --icon-stroke: 1;
  display: inline-block;
  transform: rotate(-90deg) scale(1.3);
 /*border: 2px solid #ffb74d;*/
}

/*Improve click-area of Commander icon in status-bar*/
.cmdr.status-bar-item.clickable-icon {
  /*padding-left: 1em;*/
  padding-right: 1.5em;
  /*background: #ffb74d;*/
}

.theme-light .app-container .status-bar .svg-icon {
  color: #000000;
  opacity: 0.4;
}

.theme-dark .app-container .status-bar .svg-icon {
  color: #ffb74d;
  opacity: 0.7;
}
```


