```node.js
function compareTriplets(a, b) {
    // Write your code here
    let ap=0
    let bp = 0
    for (const i in a) {
        if(a[i]<b[i]){
            bp++
        }
        else if (a[i]==b[i]){
            
        }
        else{
            ap++
        }
    }
    return [ap,bp]
}
```
