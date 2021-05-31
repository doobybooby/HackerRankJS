```node.js
function diagonalDifference(arr) {
    // Write your code here
    const len = arr.length
    let lrd = 0
    let rld = 0
    for(let i =0;i<len;i++){
        for(let j=0;j<len;j++){
            if(i===j) {lrd+=arr[i][j]}
            if(i+j===len-1) {rld += arr[i][j]}
        }
    }
    return Math.abs(lrd-rld)
}

//idk why the code below didn't work...
function diagonalDifference(arr){
  const len = arr.length
  let lrd = 0
  let rld = 0
  let j = len-1
  for(let i=0;i<len;i++){
    lrd += arr[i][i]
    rld += arr[i][j]
    j--
  }
  return Math.abs(lrd-rld)
}

```
