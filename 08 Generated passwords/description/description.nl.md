Computer generated passwords are becoming more and more popular due to the ever-growing capabilities of malicious software and hacking algorithms. The fact that characters are randomly picked from a list means that computer generated passwords are much harder to crack (as with every character that is added to the password, the number of possible passwords increase exponentially). For this exercise, make a python script that randomly generates passwords. As a rule, a good password should have at least: 1 capital letter, 1 symbol ("&", "!", "?", ":", ";"), 1 number (1 to 9) and should be 10 characters long. Tip: you can use a nested dictionary to store all possible password characters.

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


Because the response to this exercise is randomly generated and it has a lot of components to check, we have use a special evaluation function. Before sending in your response copy and paste the code below at the end of your script. Then, change the variable names 'Password_variable' and 'integer' in the first lines of this code to the variable where your password is stored and the Numbers_in_pwd variable respectively. 

<pre><code>

Password_variable = #your generated password comes here
integer_input = #the Numbers_in_pwd variable comes here



def costumeval(generated_output,expected_output):
    parsed = list(generated_output)
    symbol_list = ["&", "!", "?", ":", ";"]
    capital_check = False
    symbol_check = False
    cnt_numbers = 0

    for i in parsed:
        if i.isupper() == True:
            capital_check = True
        else:
            pass

    for i in parsed:
        if i in symbol_list:
            symbol_check = True
        else:
            pass

    for item in parsed:
        try:
            converted_int = int(item)
            cnt_numbers+=1
        except:
            ValueError

    if cnt_numbers == expected_output and capital_check == True and symbol_check == True and len(generated_output) == 10:
        return "Ok"
    else:
        return False


print(costumeval(Password_variable,integer_input))

</code></pre>







### Example

**Input:**

    2

**Output:**

    Fr:frk28ol



