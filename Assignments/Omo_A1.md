# Assignment 1 


## 1. Number of Subjects 
### A
did git pull to get new files
### B. How many times were individuals 8 and 22 sampled?
 



### C. Write a script that takes the file name and the individual ID and returns the number of times that individual was sampled. Paste your script in a code box with your answer (and explain what it does). Also include the script itself. You can use Unix or python for this.



### D. Write a script that returns a delimited table (e.g. comma-separated or tab-separated) with the number of times each individual was sampled, and saves it as Num_samples.csv. The beginning of your file should look similar to this:

## 2. Mining The Origin of Species

### A. Use the curl command to download a text version of The Origin from https://www.gutenberg.org/cache/epub/1228/pg1228.txt. Use the -o flag to name your file (otherwise the whole file will be dumped to the screen).
``` bash

!curl -o OriginOfSpecies.txt https://www.gutenberg.org/cache/epub/1228/pg1228.txt
``` 

### B. The current view on the origin of new species is that reproductive isolation plays a key role. How many times are the words "sterility" and "isolation" mentioned in the book? Hint: don't forget to make your search case-insensitive.
``` bash
# the -i makes it case-insensitive and the -o prints each line individually 
grep -oi "sterility" OriginOfSpecies.txt | wc -l.
``` 

output = 97
``` bash

grep -oi "isolation" OriginOfSpecies.txt | wc -l
``` 

output = 12
### C. To get a better idea of the context in which Darwin mentioned these words, search for the 3 lines before and after each occurrence of the key words in point B, and save your results to a text file. Save one file for each key word.


### D. A good way to explore broad patterns of word usage is a diagram called a word cloud (also known as a tag cloud).


### E. Based on your word clouds, do you agree with the idea that Darwin did not address the processes that lead to the formation of new species?



## 3. Twelve days of Christmas
```python
# all the days from the file
days = [  "First", "Second", "Third", "Fourth",
    "Fifth", "Sixth", "Seventh", "Eighth",
    "Ninth", "Tenth", "Eleventh", "Twelfth"]
# all the gifts from the file 
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
# this is for the i in the range of the 12 days it will print the day and the song lyrics
for i in range(12):
    print("On the", days[i], "day of Christmas my true love gave to me:")
    # Inner Loop - this loops back from the current day (i) to the past days to include a list of all the gifts

    for j in range(i, -1, -1):
        print(gifts[j])

    print ()

```
Output 
```python

On the First day of Christmas my true love gave to me:
A Partridge in a Pear Tree

On the Second day of Christmas my true love gave to me:
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Third day of Christmas my true love gave to me:
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Fourth day of Christmas my true love gave to me:
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Fifth day of Christmas my true love gave to me:
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Sixth day of Christmas my true love gave to me:
Six Geese-a-Laying
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Seventh day of Christmas my true love gave to me:
Seven Swans-a-Swimming
Six Geese-a-Laying
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Eighth day of Christmas my true love gave to me:
Eight Maids-a-Milking
Seven Swans-a-Swimming
Six Geese-a-Laying
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Ninth day of Christmas my true love gave to me:
Nine Ldaies Dancing
Eight Maids-a-Milking
Seven Swans-a-Swimming
Six Geese-a-Laying
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Tenth day of Christmas my true love gave to me:
Ten Lords-a-Leaping
Nine Ldaies Dancing
Eight Maids-a-Milking
Seven Swans-a-Swimming
Six Geese-a-Laying
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Eleventh day of Christmas my true love gave to me:
Eleven Pipers Piping
Ten Lords-a-Leaping
Nine Ldaies Dancing
Eight Maids-a-Milking
Seven Swans-a-Swimming
Six Geese-a-Laying
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree

On the Twelfth day of Christmas my true love gave to me:
Twelve Drummers Drumming
Eleven Pipers Piping
Ten Lords-a-Leaping
Nine Ldaies Dancing
Eight Maids-a-Milking
Seven Swans-a-Swimming
Six Geese-a-Laying
Five Gold Rings
Four Colly Birds
Three French Hens
Two Turtle Doves, and
A Partridge in a Pear Tree
```
