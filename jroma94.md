# Profile: [Your Full Name]

**NetID:** [jroma94]
**Major:** [CS + Design]
**Question that I chose from the memoization exercise:** [Count Ways with 3 moves]
**Link to the question article:** [https://www.geeksforgeeks.org/dsa/count-ways-reach-nth-stair-using-step-1-2-3/]
**My solution:**

int countWays(int n) {
        //base case
        if(n == 0){
            return 1;
        }
        
        //Invalid input
        if(n < 0){
            return 0;
        }
        
        //Recursion for running up a staircase with 1,2 or 3 steps at a time
        return countWays(n - 1) + countWays(n - 2) + countWays(n - 3);
    }
