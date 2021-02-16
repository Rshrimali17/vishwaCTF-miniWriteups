## hackerman

Title : hackerman

Category : General Skills

Description : This is a challenge to test your basic programming skills.

Pseudo code:

Set X = 1

Set Y = 1

Set previous answer = 1

answer = X * Y + previous answer + 3

After that => X + 1 and Y + 1 ('answer' becomes 'previous answer') and repeat this till you have X = 525.

The final answer is the value of 'answer' when X = 525. Fill it in below.

Example:

5 = 1 * 1 + 1 + 3

12 = 2 * 2 + 5 + 3

24 = 3 * 3 + 12 + 3

Hints : None

Files : None

Points : 100

Solves : 49

Flags : vishwaCTF{48373851}

## Writeup

After converting the pseudo code into a python code and running it gives us the flag
x=1
y=x 
p=1 
A=0 
while x<=525:
    A=x*y+p+3
    x=x+1
    y=y+1
    p=A 
    print(A)
    
flag : vishwaCTF{48373851}