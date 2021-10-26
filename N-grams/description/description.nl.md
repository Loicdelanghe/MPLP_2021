N-grams are an important aspect in computational linguistics. The n-grams of a sentence are defined as a contiguous sequence of n items from that sentence, where n can be any number from two up to the total amount of words in that sentence. This still all might sound quite abstract, so consider the following example:

**The fox jumped over the lazy dog**

A list of the tri-grams (where n = 3) would look like this:

the quick red
quick red fox
red fox jumps
fox jumps over
jumps over the
over the lazy
the lazy brown
lazy brown dog

In principle, creating n-grams boils down to finding all combinations of up to n words in a sentence, while respecting the original order of the sentence.

Having acquired this information, can you write a python script that generates the bigrams(n = 2) of an input sentence? The output of your script should be a list containing a tuple for each word combination. 

### Example

**Invoer:**

    The fox jumped over the lazy dog

**Uitvoer:**

    [("the", "fox"),("fox", "jumped"),("jumped", "over"),("over", "the"),("the", "lazy"),("lazy", "dog")] 



