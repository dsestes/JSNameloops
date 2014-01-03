JSNameloops
===========
/*jshint multistr:true */
text = "hello hello hello matt hello hello";
var myName = "matt";
var hits = [];

for(var i = 0; i < text.length; i++){
	if (text[i] == "m") {
	for(var j = i; j < (i + myName.length); j++){
		hits.push(text[j]);
	}
} 
}
if (hits.length === 0) {
	console.log("Your name wasn't found!");
} else {
	console.log(hits);
}
