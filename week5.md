# Lab Report 5

## find

```
find -empty 
```

The -empty argument finds all the empty files and directories

For Example:

**empty in parent directory**

![image](https://user-images.githubusercontent.com/122568624/224904558-e6efb9a8-9fbe-4a52-bf5f-526e5ab40134.png)

**empty in folder**

![image](https://user-images.githubusercontent.com/122568624/224905311-78e1487f-1fe2-4cf3-a41e-ee79fac801d7.png)

Source: https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/

```
find -name nameOfFile
```
The -name argument specifies the name (or a pattern with wildcards) of the file(s) you want to find. The -iname option is case-insensitive.

For example:

**-name on branches**

![image](https://user-images.githubusercontent.com/122568624/224904914-72e4f9d8-442e-4803-a238-b406ee833473.png)

**-name on test-data**

![image](https://user-images.githubusercontent.com/122568624/224905070-e04804a6-5891-4919-8b0d-d34622d63b47.png)


Source: ChatGPT
```
find -newer file 
```
Search for files that were modified/created after ‘file’.

For example: 

**looking for file created after hi.txt when theres only 1**

![image](https://user-images.githubusercontent.com/122568624/224906486-c35bd35f-4dc1-4da7-948d-fab6392bd9c4.png)

**looking for file created after the newest file**

![image](https://user-images.githubusercontent.com/122568624/224906550-e1bc9410-d287-4ec6-812c-5fbd933d33ce.png)

Source: https://www.geeksforgeeks.org/find-command-in-linux-with-examples/

```
find -type f or find -type d
```

The -type test is an efficient way of finding files and directories. The -type test lets you filter the result of the find command by either files or directories.
For example:

**-type d**

![image](https://user-images.githubusercontent.com/122568624/224906149-e6a10164-5b3b-478b-9fee-650765dfd910.png)

**-type f**

![image](https://user-images.githubusercontent.com/122568624/224906230-bae0b43c-d7d9-4ee8-a717-74a517c4b7af.png)

Source: (https://adamtheautomator.com/bash-find/)
