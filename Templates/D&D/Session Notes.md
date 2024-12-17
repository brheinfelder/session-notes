---
recording-start: 
Date: <% tp.date.now("YYYY-MM-DD") %>
timestamps: 
cssclasses:
  - session
obsidianUIMode: preview
recording-link: ""
tags:
  - session
---
>[!recording|float-right-large] Session Recording
>`BUTTON[start-recording]`
>```dataviewjs
>const link = dv.current()['recording-link'];
>dv.paragraph(link);
>```
>```dataview
>LIST WITHOUT ID timestamps
>FLATTEN timestamps
>WHERE file.path = this.file.path
>```
# Session Summary

# Characters

# Places

<%* const date = tp.date.now("YYYY-MM-DD");
await tp.file.move(tp.file.folder(true) + "/Sessions/"+date + "/" + date)
%>

```meta-bind-button
label: "Start Recording"
icon: circle-play
hidden: true
class: start-recording
tooltip: Start Session Recording
id: start-recording
style: plain
actions:
  - type: command
    command: super-duper-audio-recorder:start-stop-recording
  - type: command
    command: templater-obsidian:Templates/D&D/Session Recording Start Snippet.md
  - type: regexpReplaceInNote
    regexp: (\`BUTTON\[start-recording\]\`)1?
    replacement: "`BUTTON[stop-recording]` `BUTTON[add-note]`"
    regexpFlags: s
```
```meta-bind-button
label: "Stop Recording"
icon: circle-stop
hidden: true
class: stop-recording
tooltip: Stop Audio Recording
id: stop-recording
style: plain
actions:
  - type: command
    command: super-duper-audio-recorder:start-stop-recording
  - type: command
    command: templater-obsidian:Templates/D&D/Session Recording Stop Snippet.md
  - type: regexpReplaceInNote
    regexp: (\`BUTTON\[stop-recording\]\` \`BUTTON\[add-note\]\`)1?
    replacement: "`BUTTON[start-recording]`"
    regexpFlags: s
```
```meta-bind-button
label: New Timestamp
icon: circle-plus
hidden: true
class: "add-note"
tooltip: "Add Timestamp Note"
id: "add-note"
style: plain
actions:
  - type: command
    command: templater-obsidian:Templates/D&D/Session Timestamp Snippet.md

```
