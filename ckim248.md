Cheyoung Kim
CS+DESIGN
debugging, making a loop
debugging, vim, 

int countWays(int n) {
    // code here
    

   

        // Base cases
        if (n == 0 || n == 1)
            return 1;

        return countWays(n - 1) + countWays(n - 2);
    }

    
