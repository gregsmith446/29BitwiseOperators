# 29BitwiseOperators  
Day 29 - Using the Bitwise Operators, for each test case, print the maximum possible value of A&amp;B on a new line.

  Why This Works -> 
      
    The if else statement uses a binary formula from Jekus's post on HackerRank  
      
    The formula for finding the answer is as follows:  
      
    When k is odd, k-1 is even.  
    Therefore, k-1 can ALWAYS be reached by the bitwise calculation (k - 1) & k  

    Since ((k-1) | k ) is ALWAYS k, then ((k-1) | k ) <= n is always TRUE  
    It becomes (k <= n), which meets the problem requirements.  

    example data:  

    in binary form... if:  

    k =                     10110;  
    k - 1 =                 10101;  
    (k - 1) & k =           10101;  
    
    Then  
      
    k - 1 == (k - 1) & k == 10101;  
    
    10101 == 10101  

    Summary --> You can perform the test ((k - 1) | k) <= n to determine the answer, the maximum possible value for N and K. 
