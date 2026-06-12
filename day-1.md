# Day 1
<!-- A solution for FizzBuzz in JS-->

    fizzBuzz(n) {
        const result = [];
        
        for (let i = 1; i <= n; i++) {
            if (i % 15 === 0) {
                result.push("FizzBuzz");
            } else if (i % 3 === 0) {
                result.push("Fizz");
            } else if (i % 5 === 0) {
                result.push("Buzz");
            } else {
                result.push(i.toString());
            }
        }
        
        return result;
    }

## Algorithm (Plain English)
1. Start with an empty list to store results.
2. Loop through every number from 1 to n.
3. If the number is divisible by both 3 and 5, add "FizzBuzz" to the list.
4. If the number is only divisible by 3, add "Fizz".
5. If the number is only divisible by 5, add "Buzz".
6. Otherwise, add the number itself as a string.
7. Return the list.

<!-- A solution for FizzBuzz in Python-->
Note: - we need to use range and start from 1 and we add n + 1 to it. 
- we need == for equal
- indentation matters the most
- use (append) instead (push)
- use str to convert into string 

class Solution:
    def fizzBuzz(self, n: int) -> List[str]:
        result = []
        for i in range(1, n + 1):
            if i % 15 == 0:
                result.append("FizzBuzz")
            elif i % 3 == 0:
                result.append("Fizz")
            elif i % 5 == 0:
                result.append("Buzz")
            else:
                result.append(str(i))
        return result
