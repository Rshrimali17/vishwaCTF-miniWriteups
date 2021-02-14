![Screenshot](challenge.png)

So we are given the following website:
https://shreeraj-shivale.github.io/challenge-1/
![Screenshot](welcome.png)

Now, as we can see in the name of the question, this somehow seems to be related to robots.txt, so after opening the robots.txt file for this website we get the following:

++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>+++++++++++++++.>+++++++++++++++.--------------.+++++++++++++.<<+++++++++++++++.>++++++++++++.++++++.--.>----.++++++.<<+++++++++++++.<++++++++++++++++++++++.++++++++++.++++++++++.>++++++++++.>++++.>-.<--------.>-------..+++.++++++++.<<----------.<++++++++++++++++++++++.>-----------.>..>----.<+++++.-----.<-.>+++++++.>+.<+++++.-.

So this seems like a brainfuck cipher which you can decryot at https://www.dcode.fr/brainfuck-language

After decoding it, we get this:
User-agent: *4
Disallow:J/aasfa.html

SO this tells us that something is hidden at aasfa.html

![Screenshot](2ndpg.png)

So this ensures that we are going in the right direction!!
Now, as we can see in the website, of all the text, affine and based are both in Italics... so the flag (bo1ln_1d_gw3_bodp3a) below in red could be some sort of affine cipher which can be decoded at https://www.dcode.fr/affine-cipher
Finally, after decoding it, we get the flag as you can see below


vishwaCTF{an1me_1s_th3_answ3r}
