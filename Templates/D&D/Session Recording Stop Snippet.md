<%* const title = await tp.system.prompt("Confirm Recording", "Confirm", true);
const path = tp.file.folder(true);
const files = tp.app.vault.getFiles();
let recording = null;
files.forEach((file) => {
	if(file.path.includes(path + "/resources")) {
		recording = file;
	}
}
)
tp.app.fileManager.processFrontMatter(tp.file.find_tfile(tp.file.path(true)), (fm) => {
  fm['recording-link'] = "![["+recording.name+"]]";
});
%>