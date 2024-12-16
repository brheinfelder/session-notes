# Intro
This is the beginnings of tools that I intend to build for D&D 5e in Obsidian. For now it just takes the form of a vault template, but I will probably venture into developing a dedicated plugin some time down the line. I am open to feature suggestions, but I will be prioritizing the features that I myself will use. I have no idea if any of this is compatible with mobile versions of Obsidian and I won't be trying to ensure compatibility until the point where I feel it is necessary to develop my own plugin. For now, the following features are included:
- Campaigns Homepage
- Campaign Overview
- Session Note Template
	- Audio Recording Interface
		- Timestamp Notes
	- Summary, Characters, Locations sections

I will update this list as I continue development.
# Quick Start
## Installation
1) Install [Obsidian.md](https://Obsidian.md)
2) Take note of item 2 under 'Closing Remarks' at the bottom of this page
3) Create a local copy of this vault template
	1) Using Git (Option 1)
		1) Create local folder on your computer
		2) navigate to local folder using command prompt:
		   `cd path/to/folder`
		3) Clone repository:
		   `git clone https://github.com/brheinfelder/session-notes.git`
	1) Using Zip (Option 2)
		1) Download Zip file
		![image](https://github.com/brheinfelder/session-notes/blob/main/Documentation/zip-download.png)
		2) Unzip file to desired location
3) Launch Obsidian
4) Open repository as vault
5) If you are a new Obsidian user, I highly recommend having a look through the Obsidian documentation. It is an extremely powerful note taking app when you understand the full extent of what it can do.

![image](https://github.com/brheinfelder/session-notes/blob/main/Documentation/obsidian-open-folder.png)
## Vault Structure
As of now, there are 3 top-level directories in the vault:
1) **D&D:** This is where all the 'functional' files live for this template. These are the files that you will be interacting with directly.
2) **Documentation:** This folder contains information and images pertaining to the usage of the vault. For now it's pretty empty, but as features are added, there will likely be more in-depth docs on certain features. This folder can be safely deleted if you'd like. Note that if you *do* delete this folder, your only source of documentation will be the GitHub page, which may not render some of the markdown elements correctly.
3) **Templates:** This is where all the 'behind-the-scenes' files are stored. These are files you will not interact with directly. To maintain vault functionality, do not reorganize or move this folder. I would also recommend against modifying any of the files in this folder unless you know what you're doing.
## Creating Your First Session Note
To start taking session notes, you first have to make a campaign. Unfold the `D&D` folder and click `Campaigns`. On this new page, click `new campaign` and a enter a name for the campaign. A campaign home page will be created. I know this is a lot of clicking for fairly little return, but I plan to have more features/information displayed on these home pages in the future, so this is my way of implementing the infrastructure for that. On the new campaign home page, you can click `New Session` when you're ready to start taking session notes. See [Session Notes](Templates/D&D/Session%20Notes.md) for more info.
# Closing Remarks
Last few things:
1) If you're an experienced Obsidian user, you may notice that there are many core features missing from this vault. I wanted to make this as easy to integrate with other notes as possible, so I stripped it down to the absolute bare minimum feature set needed for these files to work (plus some custom css snippets). None of the core plugins I turned off should break any of the files here (no guarantees), so feel free to go toggle them back on.
2) This vault does come with packaged community plugins necessary for the vault to function. In general, downloading such a vault would be a security risk and you shouldn't do this with other vaults as they may contain malicious code. However, this vault is primarily made for me and those who know me and packaging the plugins is the easiest way to deploy with minimal fuss. If you would like a more secure way to use this vault, follow the download steps from above, but before opening the vault in obsidian navigate to the folder in your file browser and delete the contents of `.obsidian` except for the `snippets` directory. Then, when you open the vault, go to settings > community plugins > browse, and install and enable the following plugins:
	1) [Badges](https://github.com/gapmiss/badges)
	2) [Dataview](https://github.com/blacksmithgu/obsidian-dataview)
	3) [Folder Notes](https://github.com/LostPaul/obsidian-folder-notes)
	4) [Force Note View Mode](https://github.com/bwydoogh/obsidian-force-view-mode-of-note)
	5) [Meta Bind](https://github.com/mProjectsCode/obsidian-meta-bind-plugin)
	6) [Modal Forms](https://github.com/danielo515/obsidian-modal-form)
	7) [Super Duper Audio Recorder](https://github.com/madpin/super-duper-audio-recorder)
	8) [Style Settings](https://github.com/mgmeyers/obsidian-style-settings)
	9) [Templater](https://github.com/SilentVoid13/Templater)
3) This whole vault is a very active work-in-progress and is currently in pretty rough shape, but I wanted to get something 'usable' published as soon as I could. Feedback, Feature requests, and bug reports are *very* welcome and appreciated. Just open a GitHub issue and let me know what you think!