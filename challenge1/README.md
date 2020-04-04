# challenge 1

Given an integer called sum and an array of integers called numbers, check whether there’s a combination of any 
two elements in the numbers array that can be added to equal sum exactly.

#### Here’s an example:
Input: sum = 17, numbers = [1, 9, 2, 19, 14, 8]
Answer: true since 9 + 8 = 17

## Solutions here...:
#### Solution1:

`
   
    private static boolean function(Integer sum, Integer[] numbers) {
    
        List<Integer> toList = Arrays.asList(numbers);

        for(Integer num: toList) {
            if(toList.contains(sum - num)) {
                return true;
            }
        }
        return false;
    }
`
