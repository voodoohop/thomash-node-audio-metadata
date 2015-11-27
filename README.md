# thomash-node-audio-metadata

extract audio metadata from wav, mp3, aiff and many other formats. uses a javascript cross-compiled taglib.

### install
    npm install thomash-node-audio-metadata

### usage
    var MetadataFile = require("thomash-node-audio-metadata");
	
	var f = new MetadataFile("/path/to/audio/file";
	f.readTaglibMetadata(function(data) {
		console.log(data);
	});
	
    // example result: {"metadata":{"album":"Brazil Classics, Vol. 5: The Hips of Tradition","albumartist":"Tom Zé","artist":"Tom Zé","comment":"Am","composer":"Tom Zé","date":"1992","genre":"Latin","initialkey":"Am","label":"Luaka Bop","length":"153160","title":"Lua-Gira-Sol [Moon-Turn-Flower]","tracknumber":"13"},"audio":{"length":153,"bitrate":320,"channels":2,"samplerate":44100}	

