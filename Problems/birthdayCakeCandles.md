```node.js
function birthdayCakeCandles(candles) {
    // Write your code here
    let max = candles[0]
    let frequency = 0
    
    for(const i in candles){
        if(candles[i]>max){
            max=candles[i]
        }
    }
    for(const i in candles){
        if(candles[i]==max){
            frequency++
        }
    }
    return frequency
}
```
