---
tags:
  - campaign
obsidianUIMode: preview
---
<%* const name = await tp.system.prompt("Campaign Name");
await tp.file.move(tp.file.folder(true) + "/"+name + "/" + name)
%>
```meta-bind-button
label: New Session
icon: plus
hidden: false
class: ""
tooltip: ""
id: ""
style: primary
actions:
  - type: command
    command: templater-obsidian:create-Templates/D&D/Session Notes.md

```
# Sessions
```dataview
CALENDAR Date
FROM #session 
WHERE contains(file.path,this.file.folder)
```
