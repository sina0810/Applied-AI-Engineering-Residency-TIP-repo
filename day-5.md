# Day 5
 <!-- This is sulution for JS  -->

function isPalindrome(x) {
  if (x < 0) return false;
  const str = x.toString();
  let left = 0;
  let right = str.length - 1;
  while (left < right) {
    if (str[left] !== str[right]) return false;
    left++;
    right--;
  }
  return true;
}

## Algorithm (Plain English)
1. First we check if the list if empty and if yes we return false. 
2. Start by adding the digits into a list and convert each elements into a string. 
3. Make a copy of the list so we can use that for the comparison. 
4. Reverse the list for the comparison.
5. Add the if statement to see if the original list is equal to the reversed list.
6. If yes return true
6. If not the same return false.  
 <!-- This is sulution for Python  -->
- we need to make add the nums into a list and them convert them into a str so we can work with them. 
- we need a copy for the list so we can compart it to the reversed one later to see it they are palindrome. 
class Solution:
    def isPalindrome(self, x: int) -> bool:
        if x < 0:
            return False
        digits = list(str(x))

        copy_digits = digits.copy()

        digits.reverse() 

        if digits ==  copy_digits:
            return True
        else:
            return False
