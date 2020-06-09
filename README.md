
# Practice with Bayes

![]() ![]()


Thomas Bayes           |  Bayes Theorum
:-------------------------:|:-------------------------:
![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Thomas_Bayes.gif/225px-Thomas_Bayes.gif)  |  ![](https://lh3.googleusercontent.com/proxy/0s1DMC6OW-58QzKUEEuVuhM3vW7aZivHikobieoN1vgMxSB-1qNbKdvcOsLd7G6UJE0iMKPPYYUeo1dgSHoT6HZtibPGrJXF3_NAjrI5uZPv2YJWJHmzPdZaq_uUnZs)


```python
# Run this cell unchanged.
from test import Test
test = Test()
```

# #1

<u><b>Define a function called ```bayes``` that receive 3 parameters:</b></u>
1. b_given_a
2. a
3. b

And returns the probability for A|B


```python
# Your code here
def bayes():
    pass
```

# #2

**You receive an email and your spam detector has classified the email as spam.** 

Assume that: 
- 5% of emails you receive are spam 
- The spam detector correctly identifies spam 99% of the time
- Emails are incorrectly marked as spam 0.2% of the time. 

*Hint*

>P(B) = P(B|A) × P(A) + P(B|not A) × P(not A) = P(Detected) = P(Detected|Spam) × P(Spam) + P(Detected|not Spam) × P(not Spam)

<u><b>What is the probability the email is spam?</b></u>


```python
# Your code here
b_given_a = None
a = None
b = None
a_given_b = bayes(b_given_a, a, b)
```

*Run the cell below to check your answer*
>(Do not round your answer)


```python
test.run_test(a_given_b, 'spam')
```

# #3

It's a typically hot morning in June in Durham.  You look outside and see some dark clouds rolling in.  Is it going to rain?

Historically, there is a 30% chance of rain on any given day in June.  Furthermore, on days when it does in fact rain, 95% of the time there are dark clouds that roll in during the morning.   But, on days when it does not rain, 25% of the time there are dark clouds that roll in during the morning.

Given that there are dark clouds rolling in, what is the chance that it will rain?


```python
# Your code here
b_given_a = None
a = None
b = None
a_given_b = bayes(b_given_a, a, b)
```

*Run the cell below to check your answer*


```python
test.run_test(a_given_b, 'rain')
```

# #4

You are on a jury considering a paternity suit.  The mother has blood type O, and the alleged father has blood type AB.

A blood test shows that the child has blood type B.   What is the chance that the alleged father is in fact the real father, given that the child has blood type B?

Here's some information we need to solve the problem.  According to genetics, there is a 50% chance that this child will have blood type B if this alleged father is the real father, and based on rates of B genes in the population, there is a 9% chance that this child would have blood type B if this alleged father is not the real father.

Based on other evidence (e.g., testimonials, physical evidence, records) presented before the DNA test, you believe there is a 75% chance that the alleged father is the real father.  This assessment is your prior belief.  Now, we need to use Bayes Rule to update it for the results of the child's blood test.


```python
# Your code here
b_given_a = None
a = None
b = None
a_given_b = bayes(b_given_a, a, b)
```

*Run the cell below to check your answer*


```python
test.run_test(a_given_b, 'father')
```
