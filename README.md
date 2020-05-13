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
curl "https://en.wikipedia.org/wiki/List_of_unusual_deaths"
```

- To return the page and output to a file named **data.txt**

```
curl "https://en.wikipedia.org/wiki/List_of_unusual_deaths" -O data.txt
```

