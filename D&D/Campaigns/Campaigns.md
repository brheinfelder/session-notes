---
obsidianUIMode: preview
---

```meta-bind-button
label: New Campaign
icon: plus
hidden: false
class: ""
tooltip: Create new Campaign
id: ""
style: primary
actions:
  - type: command
    command: templater-obsidian:create-Templates/D&D/Campaign Template.md

```
```dataview
LIST WITHOUT ID file.link
FROM #campaign 
WHERE contains(file.path,this.file.folder)
```
