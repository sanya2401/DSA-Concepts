We use frequency count method to analyse the time and space complexity of an algorithm.

"""Example 1 - Single Loop"""

Algorithm sum(A,n)
{
    s=0;                     1
    for(i=0;i<n;i++)         n+1
    {
        s=s+A[i];            n
    }
    return s;                1   
}
Time:
Explanation: The constant statements are understood. The for loop has three statements:
i=0, which executes for 1 unit of time,
i<n, which will execute for n+1 times ; n with true values and n+1 th when false
i++ executes for n times

For analysis we take the biggest term which is n+1,
Now whatever is inside the loop executes for n number of times because the loop executes for n times, so the statement  s=s+A[i]; executes n times.

Time taken  =  f(n)=2n+3
f(n)=n

Space: 
Variable used: 
A -- n words
n -- 1
s -- 1
i -- 1 
S(n)= n

"""Example 2 -Addition of Matrix (Nested Loop)"""

Algorithm Add(A,B,n)
{
    for (i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            C[i,j]=A[i,j]+B[i,j]
        }
    }
}

Explanation:
first for loop takes n+1 time and all the statements inside it take n time: 
Algorithm Add(A,B,n)
{
    for (i=0;i<n;i++)              n+1
    {
        for(j=0;j<n;j++)           n
        {
            C[i,j]=A[i,j]+B[i,j]   n
        }
    }
}
The second loop also takes n+1 time and the statement inside it takes n time:
Algorithm Add(A,B,n)
{
    for (i=0;i<n;i++)              n+1
    {
        for(j=0;j<n;j++)           n * (n+1)
        {
            C[i,j]=A[i,j]+B[i,j]   n * n
        }
    }
}
f(n)=2n^2 + 2n + 1
f(n)=n^2

Space:
Variables:
A- n^2
B-n^2
C-n^2
n-1
i-1
j-1

S(n)=n^2

