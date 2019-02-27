# EECS 201 HW 6
uniqname:  bgribov

## Question 1
``` 1
^ represents the begining of the string, meaning that the string start with whatever is after the symbol
```

## Question 2
``` 2
$ represents the end of the string, meaning the string ends right with that was before the symbol
```

## Question 3
``` 3
. takes the place of a letter. For example .at could produce bat, cat, sat, and so on. 
```

## Question 4
``` 4
grep -c ^...$ cracklib-small
```

## Question 5
``` 5
grep -c ^[a-z][a-z][a-z]$ cracklib-small
```

## Question 6
``` 6
for vowel in a e i o u; do echo -e "$(grep -c ^$vowel cracklib-small) \t $vowel"; done | sort -rn
For each vowel, a, e, i, o, u prit out the number of words in cracklib-small that start with that vowel and then print the vowel (after a tab). When you print this print it in reverse numerical order (biggest to smallest)
```

## Question 7
``` 7
sort <(cat american-english british-english) | uniq -u | wc -l
```

## Question 8
``` 8
sort <(cat american-english cracklib-small) | uniq -d | wc -l
```

## Question 9
``` 9
This command is searching for all strings in the file that (-v) excludes the lines that begin with a sapce and then a *.
```

## Question 10
``` 10
Git grep doesn't search untracked files as when I made a file with a name that should be found with the command git grep did not locate it. 
```

## Question 11
``` 11
It searches files that haven't been comitted but are staged. I made a file then did git add and when I ran git grep it showed up eventhough I had not comitted it yet. 
```
