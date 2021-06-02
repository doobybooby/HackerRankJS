```node.js
function gradingStudents(grades) {
    // Write your code here
    let copy =[]
    let ans = []
    for(const i in grades){
        copy.push(grades[i])
    }
    
    for(const i in copy){
        if(copy[i]<38){
            ans.push(copy[i])
        }
        else if(copy[i]%5>2){
            //round up
            let current = copy[i]
            while(current%5!=0){
                current++
            }
            ans.push(current)
        }
        else{
            ans.push(copy[i])
        }
    }
    return ans
}
```
