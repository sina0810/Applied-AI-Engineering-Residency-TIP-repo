# Day 4

 <!-- This is sulution for JS  -->
function containsDuplicate(nums) {
  const seen = new Set();
  for (let i = 0; i < nums.length; i++) {
    if (seen.has(nums[i])) {
      return true;
    }
    seen.add(nums[i]);
  }
  return false;
}
## Algorithm (Plain English)
1. Start by sorting the list. 
2. Loop through the sorted list from the start all the way to the one element before the end of the list. 
3. Compare if the element we looking at is the same as the one ahead of it. 
4. If yes return true
5. If not the same return false at the end of the list. 

 <!-- This is sulution for Python -->
 - we need to becarefull to not go outside of the list wihle looping, so we need to use len and -1

class Solution:
    def containsDuplicate(self, nums: List[int]) -> bool:
        sort_nums = sorted(nums)
        for i in range(len(sort_nums) - 1):
            if sort_nums[i] == sort_nums[i + 1]:
                return True

        return False  