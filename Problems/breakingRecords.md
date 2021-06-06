```node.js
function breakingRecords(scores) {
    // Write your code here
    let ans = ""
    let minCount = 0
    let maxCount = 0
    let minRec = scores[0]
    let maxRec = scores[0]
    
    if(scores.length<=1) return [0,0]
    else{
        for(let i =0;i<scores.length;i++){
            if(scores[i]<minRec){
                minRec = scores[i]
                minCount+=1
            }
            else if(scores[i]>maxRec){
                maxRec = scores[i]
                maxCount+=1
            }
        }
    }
    return [maxCount, minCount]
}
```
