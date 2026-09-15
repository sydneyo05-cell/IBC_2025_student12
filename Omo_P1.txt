
# Week 3 Practical

## Markdown Homework

# W1 Practical

# W1 Practical

## 1. Navigate to your home directory

```bash
cd ~
```

## 2. Navigate to the directory that contains work for another class using a relative pathway

```bash
cd ~/IntroBiolComp-2026/Python
```

## 3. Navigate to the Data Files directory within Python

### a. First get into Python

```bash
cd Users
cd IntroBiolComp-2026
cd Python
```

### b. Now in Python

```bash
cd DataFiles
```

## 4. Navigate to sandbox within Unix

### a. Go back to IntroBiolComp-2026

```bash
cd ../..
```

### b. Now go to Unix

```bash
cd Unix
```

## 5. Navigate to the DataFiles directory in IntroBiolComp-2026/Python

```bash
cd DataFiles
```

## 6. How many lines are in the file BeeSpecies.txt?

```bash
wc -l BeeSpecies.txt
```

**Answer:** 19,509 lines

## 7. Without leaving the current directory, count the number of words in the CodonTable.tsv file in the IntroBiolComp-2026/Unix/DataFiles directory

```bash
wc -l CodonTable.tsv
```

## 8. What is the last codon reported in this file?

```bash
tail -n 1 CodonTable.tsv
```

**Answer:** TT Phe F
