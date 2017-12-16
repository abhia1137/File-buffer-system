
var  numbers = [2,4,1,5,4]

function isBiggerThanTwo (num) {  
  return num > 2
}

numbers.filter(isBiggerThanTwo)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++
console.log('first');
var fs = require('fs'); 
fs.readFile('./files/NewFile.txt', 'utf8', function(err, content){
	console.log('Scond');
	
});
console.log('Third')

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
var express = require('express');
var app =express();
app.get('/ab', function(req, res){
	res.send('First');
})
console.log("Second");
app.listen(2222, function(){
	console.log('yes server is running');
})
console.log('Third');
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

var fs = require('fs');
let eventNum = 0;
fs.watch('NewFile.txt', 'utf8', function(event,filename){ // Event loop 
	eventNum++
	console.log('Event ' + eventNum+ ": "+event+ ", for file " +filename);
});
fs.watch('NewFile1.txt', 'utf8', function(event,filename){
	eventNum++
	console.log('Event ' + eventNum+ ": "+event+ ", for file " +filename);
});

console.log('Looking for the change');
