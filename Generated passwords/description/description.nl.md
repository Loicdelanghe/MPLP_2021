Computer generated passwords are becoming more and more popular due to the ever-growing capabilities of malicious software and hacking algorithms. The fact that characters are randomly picked from a list means that computer generated passwords are much harder to crack (as with every character that is added to the password, the number of possible passwords increase exponentially). For this exercise, make a python script that randomly generates passwords. As a rule, a good password should have at least: 1 capital letter, 1 symbol, 1 number (1 to 9) and should be 10 characters long. Tip: you can use a nested dictionary to store all possible password characters.

Python has a built-in module that allows you to pick a random item from a list (make sure you don't forget to import it at the beginning of your script!):


<pre><code>
Import random

L = [1,2,3,4,5]
random_number = random.choice(L)

</code></pre>


As an additional challenge: let's make an algorithm that takes some user input. Dodona will automatically provide you with an integer number. The number can be called at the beginning of your script in this way:

<pre><code>
Numbers_in_pwd = int(input())

</code></pre>

Make sure that your password contains as many numbers as the input integer specifies e.g if the input is 3, your password should contain at least 3 numbers. 


### Example

**Invoer:**

    2

**Uitvoer:**

    Fr:frk28ol



