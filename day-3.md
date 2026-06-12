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
## Algorithm (Plain English)
1. First create a variable to start from first index from the left side of the string. 
2. Start the other variable to start at the end of the string.
3. Add a while loop which means while this condition is true. 
4. Swip the variables positions in place. 
5. Move the left pointer to the right, and move the right pointer to the left
6. At the end return the string. 

<!-- THIS SOLUTION IN PTHTON: -->
this is how to get the last index in Python len(s)-1

        left = 0
        right = len(s)-1

        while(left < right):
            s[left], s[right] = s[right], s[left]
            left +=1
            right -=1
        return s
