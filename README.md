# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
 Step 1: Import sys module to use command line arguments.
 Step 2: Use the open() by getting the file name with "sys.argv[1]" which means the first index of given argument
 Step 3: Iterate the content of the file using for loop.
 Step 4: Split the contents into each line using .split() function.
 Step 5: Iterate the list of lines and increment the value of variable (word) each time.
 Step 6: Run the program by giving "python prgm.py EX12.txt" on the terminal.


## PROGRAM:

```
#Developed By: ABINAYA S
#Register No: 212222230002
import sys
count = {}
with open(sys.argv[1], 'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word] = 1
            else:
                count[word] += 1
print(count)
f.close()
```
### OUTPUT:
#### File content:
![Screenshot 2023-06-08 113331](https://github.com/ROHITJAIND/command-line-arguments-to-count-word/assets/118707073/07302a96-9557-4806-8236-4381000c3715)

### OUTPUT:
![Screenshot 2023-06-08 113438](https://github.com/ROHITJAIND/command-line-arguments-to-count-word/assets/118707073/24d5bb6b-e206-4cd3-ba56-97b7837aa52e)


## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
