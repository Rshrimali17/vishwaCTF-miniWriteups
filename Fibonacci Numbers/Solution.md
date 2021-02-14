## Fibonacci Numbers

Title : Fibonacci Numbers

Category : Reverse Engineering

Description : Fibonacci numbers are (0 1) 1 2 3 5 8 13 21 34 55 89 ... Can you uncover the mystery between these numbers and the given txt file? ... 

Hints : None

Files : Fibonacci.txt

Points : 100

Solves : 15

Flags : vishwaCTF{f1b0_f1b0_f1b0}

## Solution

1. We see that the Fibonacci.txt starts with 'vis'. What a coincidence, Our flag also starts with the same - vishwaCTF{...}
2. Also, the 5th character is 'h'. Could be the 'h' in vishwaCTF{...}
3. Also, the 8th character is 'w'. Could be the 'w' in vishwaCTF{...}
4. Also, the 13th character is 'a'. Could be the 'a' in vishwaCTF{...}
4. So, we can think a bit and then see that the difference in the places of these characters may represent the Fibonacci Series.
5. v:1, i:2, s:3, h:5, w:8, a:13, ......
6. i-v:1, s-i:1, h-s:2, w-h: 3, a-w:5, ......
7. Voila, we did get the Fibonacci Series, starting from 1. But remember from the description? Fibonacci Series doesnt change no matter whether it starts from 0 or 1.
8. Now, we needto think of a way to extract all the characters even at a large number of places. Because, the 10th number in Fibonacci is = 55 and 20th = 6765, and so on. Therefore, we cannot manually track the positions.
9. So, we need to write a code for it. 
10. The logic will be, we start from the very first position in the text, take that character at that position : v. Then we add the Fibonnaci Number(1) in our position and get : i. Then we add next Fibonnaci Number(1) in position where we got 'i', and we get 's'. Then we add next Fibonacci Number(2) in position of 'i' and get : h. And so on....
11. So, we should write a loop for this. The loop will start from first position.
    Store the character at that place.
    If it is the first loop :
        Set current Fibonnaci Number as 1. And add it to the position.
    Else
        Add the next Fibonacci Number to the position.
    Go to that Position.
    Repeat till end of all text.
12. See the stored characters, it will be the flag.

I have explained the whole logic here. Now go write the code for this in your favorite language.

<hr>

P.S. : You can copy all the text in an array itself if you dont wanna handle File Reading. All languages are capable of handling Character Arrays/String of millions of length.