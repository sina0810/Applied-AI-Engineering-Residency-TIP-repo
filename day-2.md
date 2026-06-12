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
