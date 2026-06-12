# Day 2
<!-- Solution for JS Two Sum -->

function twoSum(nums, target) {
  for (let i = 0; i < nums.length; i++) {
    for (let j = i + 1; j < nums.length; j++) {
      if (nums[i] + nums[j] === target) {
        return [i, j];
      }
    }
  }
} 

## Algorithm (Plain English)
1. Start by looping through the list, loop from 0 to the end of the list.
2. Start the inner loop so we can loop the list twice for the comparison, make sure to start after the outter loop. 
3. Add first if statement to compare the ouuter index to the inner index, and see if they add up to the target. 
4. If they are add up to the target return their indexes.


<!-- Soulution for Python  -->
We need to use   for num in range(1, len(nums)):
                so we are counting from the index 1, we add 1, and then we add len(nums), 
                that means we need to start at the index 1 in the list. 
                in pthaon we can only have one type of values 
                   

class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        for i in range(len(nums)):
            for j in (range(i+1, len(nums))):
                if nums[i] + nums[j] == target:
                    return([i, j])
