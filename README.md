# Furniture-App

hi
1.

function processData(input) {
    var lines = input.split('\n');
    var n = parseInt(lines[0]);
    var arr = lines[1].split(' ').map(Number);
    arr.sort(function(a, b) { return b - a; });
    console.log(arr[2]);
} 

process.stdin.resume();
process.stdin.setEncoding("ascii");
_input = "";
process.stdin.on("data", function (input) {
    _input += input;
});

process.stdin.on("end", function () {
   processData(_input);
});

