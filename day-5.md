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
