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



-------------------------------------
function processData(input) {
    //Enter your code here
    let arr = input.split(' ').map(Number);
    let sorted = true;
    for (let i = 1; i < arr.length; i++) {
        if (arr[i] < arr[i - 1]) {
            sorted = false;
            break;
        }
    }
    console.log(sorted);
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

