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
