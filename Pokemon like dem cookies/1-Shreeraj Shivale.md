## Pokemon like dem cookies

Title : Pokemon like dem cookies

Category : Web

Description : Pikachu is trying to say something to Ash... Can you help help him understand?
https://shreeraj-shivale.github.io/webchallenge/

P.S. : Turn up the volume and feel free to explore the website and have fun with it :)  

Hints : None

Files : None

Points : 150

Solves : 28

Flags : vishwaCTF{gotta_catch_em_all}

## Solution

![Screenshot](challenge.png)
  

So we are given the following website: 
https://shreeraj-shivale.github.io/webchallenge/

So, as we can see, the website contains the term cookies, so lets just check the cookies

Yup, it contains a cookie called as flag with following value:
pi pi pi pi pi pi pi pi pi pi pika pipi pi pipi pi pi pi pipi pi pi pi pi pi pi pi pipi pi pi pi pi pi pi pi pi pi pi pichu pichu pichu pichu ka chu pipi pipi pipi pipi pi pi pi pikachu pi pi pi pi pi pi pi pi pikachu pi pi pi pi pi pikachu pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu ka ka pikachu pi pi pi pi pikachu ka ka pikachu pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pi pi pi pi pi pikachu ka ka ka ka ka ka ka ka ka pikachu pi pi pi pi pi pi pikachu pi pi pi pi pi pi pi pi pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pi pi pikachu pi pi pi pi pi pi pi pi pi pi pi pikachu pikachu 

This seems like pikalang cipher which can be decoded here 

https://www.dcode.fr/pikalang-language

After decoding it, we get the flag!!

vishwaCTF{gotta_catch_em_all}
