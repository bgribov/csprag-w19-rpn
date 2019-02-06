# EECS 201 HW 3
uniqname:  bgribov

## Question 1
``` 1
ls, mkdir, touch don't work 
```

## Question 2
``` 2
Mkdir cannot be done with an empty path because it will exit with error if the path does not exsist. If path does not exsist it will exit with an error behavior. 
```

## Question 3
``` 3
PWD still works! PWD is a built in command on many shells, therefore still works when there is an empty path. Path however is an evironment variable that shows which directories the shell can search to find a command that was typed. Since it is built in and not based on the environment variable, pwd still works with an empty path. 
```

## Question 4
``` 4
$? represents the exit status of the previous command in the script. This was actually helpful for me when I did advanced homework 3 as I used it to check the exit status of the files I ran to see if they ran over time, exited with failure, or success. 
```

## Question 5
``` 5
$1 represents the first argument passed to the script. When running somehting like ./program why this we could gather the why variable which could be an indicator for the program that is running. This could be helpful to access an argument if theres a specific place for each argument to tell the script what the program wants. 
```

## Question 6
``` 6
#!/bin/bash


gcc -o helloworld helloworld.c
./helloworld > hey.txt

if [ "$(cat hey.txt)" == "Hello World!" ]; then
echo "All tests passed"
else
echo "Test failed. Expected output >>Hello World<<, got output >>" $(cat hey.txt) "<<"
fi
```

## Question 7
``` 7
You could modify your bash profile to say: export PATH=$PATH:/and add what you want the path to be!
```

### Question 8
``` 8
Around 3 hours, it took a while to figure out the bash script and the PATH questions confused me a little
```
