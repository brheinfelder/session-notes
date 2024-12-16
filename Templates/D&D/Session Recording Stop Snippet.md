<%* await sleep(2000);
const path = tp.file.folder(true);
let files = tp.app.vault.getFiles();
let recording = null;
files.forEach((file) => {
	if(file.path.includes("Recordings")) {
		tp.app.fileManager.renameFile(file, path + "/" + tp.frontmatter.Date + " Session Recording.wav");
		recording = file;
	}
}
)
await sleep(100);
const folder = tp.app.vault.getFolderByPath("Recordings");
tp.app.vault.delete(folder);
tp.app.fileManager.processFrontMatter(tp.file.find_tfile(tp.file.path(true)), (fm) => {
  fm['recording-link'] = "![["+recording.name+"]]";
});
%>