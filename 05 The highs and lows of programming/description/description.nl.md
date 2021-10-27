Write a python script that finds the maximum and minimum integer values in a list and print them out in a tuple. It seems that in my absent-mindedness I have left some string and dictionary objects in the lists, which means the built-in max() and min() functions will not work. Count the numbers of dictionaries and strings in the list and print the final number out nicely, as seen below. 

Dodona will automatically provide input lists for your script. However since Dodona is quite particular when it comes to input and evaluation of python scripts you should start your script with:

<pre><code>
L = eval(input())

</code></pre>



### Example

**Input:**

    [52, 96, 2, "Apples", 1]

**Output:**

    Number of strings in the list: 1 
    Number of dictionaries in the list: 0
    (1, 96)



