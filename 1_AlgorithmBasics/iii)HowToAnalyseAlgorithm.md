Basis of Analysis:
1. Time
2. Space
3. Network Concumption
4. Power Consumption
5. CPU Registers (in system level programs)

For Broader and easy terms, we consider time and space in most cases.

For time analysis, lets say each simple statement takes 1 unit of time to execute.

"""Example 1"""
Lets take a simple swap algorithm

Algorithm Swap(a,b)
{
    temp=a;    --- 1
    a=b;       --- 1
    b=temp;    --- 1
}

Time: 
Since each statement now takes one unit of time, the total time function becomes:
f(n)= 1+1+1= 3
f(n)=3  which is constant. 

Space: 
variables used:
a - 1 word
b - 1 word
temp - 1 word
S(n)=3 words (we say words here because the data type of the variables is unknown)

