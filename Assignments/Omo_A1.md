# Assignment 1 


## 1. Number of Subjects 
### A
did git pull to get new files
### B. How many times were individuals 8 and 22 sampled?




### C. Write a script that takes the file name and the individual ID and returns the number of times that individual was sampled. Paste your script in a code box with your answer (and explain what it does). Also include the script itself. You can use Unix or python for this.



### D. Write a script that returns a delimited table (e.g. comma-separated or tab-separated) with the number of times each individual was sampled, and saves it as Num_samples.csv. The beginning of your file should look similar to this:


## 3. Twelve days of Christmas
```python
days = [
    "First", "Second", "Third", "Fourth",
    "Fifth", "Sixth", "Seventh", "Eighth",
    "Ninth", "Tenth", "Eleventh", "Twelfth"
]
gifts = [
    "A Partridge in a Pear Tree",
    "Two Turtle Doves, and",
    "Three French Hens",
    "Four Colly Birds",
    "Five Gold Rings",
    "Six Geese-a-Laying",
    "Seven Swans-a-Swimming",
    "Eight Maids-a-Milking",
    "Nine Ldaies Dancing",
    "Ten Lords-a-Leaping",
    "Eleven Pipers Piping",
    "Twelve Drummers Drumming"
]


# Outer Loop 
for i in range(12):
    print("On the", days[i], "day of Christmas my true love gave to me:")
    # Inner Loop 
    for j in range(i, -1, -1):
        if j == 1:
            print(gifts[j] + ", and")
        else:
            print(gifts[j])

    print()

```
