<%* var duration = Number(moment.duration(moment().diff(tp.frontmatter['recording-start'])).asSeconds());
let seconds = Math.floor(duration);
const hours = Math.floor(seconds / 3600);
seconds = seconds % 3600;
const minutes = Math.floor(seconds / 60);
seconds = seconds % 60;
const values = {
	time: hours+"h "+minutes+"m "+seconds+"s",
	badgetext: "Add",
	desc: "New Timestamp",
};
const modalForm = app.plugins.plugins.modalforms.api;
const result = await modalForm.openForm("timestamp",{values: values});
await sleep(100);
tp.app.fileManager.processFrontMatter(tp.file.find_tfile(tp.file.path(true)), (fm) => {
	if (!Array.isArray(fm['timestamps'])) {
	    fm['timestamps'] = [];
	}
	console.log(result);
	fm['timestamps'].push("`[!!time:" + result.get("time") + "]` " + "`[!!" + result.get("badgetype") + ":" + result.get("badgetext") + "]` " + result.get("desc"));
});
%>