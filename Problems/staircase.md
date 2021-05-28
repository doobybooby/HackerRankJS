```node.js
function staircase(n) {
    // Write your code here
    for(let i =0;i<n;i++){
        //s = n-i-1
        //# = i+1
        let string = "";
        for(let j = 0;j<n-i-1;j++){
            string += " "
        }
        for(let k =0;k<i+1;k++){
            string += "#"
        }
        console.log(string)
    }
}
```
