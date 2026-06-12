# Day 3
 <!-- This is sulution for JS  -->
var reverseString = function(s) {
    let left = 0
    let right = s.length - 1

    while (left < right){
        [s[left], s[right]] = [s[right], s[left]]
        left++
        right--
    }
    
    return s
};

<!-- THIS SOLUTION IN PTHTON: -->
this is how to get the last index in Python len(s)-1

        left = 0
        right = len(s)-1

        while(left < right):
            s[left], s[right] = s[right], s[left]
            left +=1
            right -=1
        return s
