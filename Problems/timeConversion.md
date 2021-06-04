```node.js

function timeConversion(s) {
    // Write your code here
            
        let ans = ""
        let hour = Number(s.substring(0,2)) // gets the hour
        let minSec = s.substring(3,8)// gets the minutes and the seconds 
        let amOrPm = s.substring(8) // either AM or PM

        if(amOrPm == "PM" && hour != 12){
            console.log("here")
            hour += 12;
        }
        else if (amOrPm =="AM" && hour ==12){
            hour = 0;
        }
        
        if(hour<12){
            ans = "0"+hour+":"+minSec
            return ans
        }
        ans = hour + ":" +minSec
        return ans
}


```
