# Notes

## Creating a Project

- First I have created a new sub-folder within the folder named 44517 and I have named the sub-folder as **shell-data-processing** by using the command:

```
mkdir shell-data-processing
```

- Then, I have changed the directory to **shell-data-processing** by using the command:

```
cd shell-data-processing
```
- You shall now be within the folder **shell-data-processing**. Any operations performed will now occur within the folder **shell-data-procssing**.

- Now in order to create an empty new item named ***README.md*** and ***.gitignore*** , I shall be using the commands as described below:

```
ni README.md
ni .gitignore
```
- In order to list the contents that are present in the current working library, I will be using the command:

```
ls 
```

- Closing the PowerShell
```
Press Alt+Space c
```


## Curl Commands Used

- To return the text page

```
curl command "https://en.wikipedia.org/wiki/List_of_unusual_deaths"
```

- To return the page and output to a file named **data.txt**

```
curl "[url](https://en.wikipedia.org/wiki/List_of_unusual_deaths)" -O data.txt
```

## Bash Commands Used
### Commands used to find most common words,sorted 

- In order to convert each space present in the file **data.txt** into line-feed(like \n or making the test to enter into next line) and each line to be converted into individual words

```
tr ' ' '\12' < data.txt
```

- The **data.txt** file thus modified will now undergo the sorting process in an ascending order by using the command as displayed below

```
tr ' ' '\12' < data.txt | sort
```

- The **data.txt** file thus sorted will now undergo piping of the sorted output to uniq -c to count

```
tr ' ' '\12' < data.txt | sort | uniq -c
```

- Now, we will pipe the reduced output to sort with -nr flag by using the command

```
tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr
```

- In order to re-direct the processed output to **result.txt**

```
tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt
```
