The ability to expand Obsidian’s functionality via community plugins is amazing. However, I often encounter these problems when working with plugins:
- Doesn’t work on mobile
- Hasn’t been updated for a long time
- Causes bugs or works unstably
- Complete dependency on the plugin developer

All of this made me look for alternative ways to extend the functionality of Obsidian’s mobile app.

Fortunately, I quickly found a solution that works for me—writing JS scripts and running them through the [CodeScript toolkit](https://github.com/mnaoumov/obsidian-codescript-toolkit) plugin.

You can run JS scripts in several ways:
- StartUp: scripts run at app launch
- Invoke: scripts run on command
- Code-button/code-block: scripts run from a note

This approach helps avoid common plugin compatibility and support issues on mobile and enhances your control over functionality. 
