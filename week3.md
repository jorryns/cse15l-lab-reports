# Lab Report 3

## grep

```
grep -r "string" /path
```

The -r argument stands for recursive and recursively reads all files under the directory for "string". The output returns the file with the string. For example:

![Image](https://jorryns.github.io/cse15l-lab-reports/lab3.3.jpg)

Source:https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/

```
greep -c string /file
```
The -c argument counts the amount of times that the string is found in each file
For example:

![Image](https://jorryns.github.io/cse15l-lab-reports/lab3.1.png)

Source: https://phoenixnap.com/kb/grep-command-linux-unix-examples#:~:text=The%20grep%20command%20prints%20entire,%2C%20add%20the%20%2Dx%20option.&text=The%20output%20shows%20only%20the%20lines%20with%20the%20exact%20match.
```
grep -n 'word' /file/path
```
The -n command displays the matched lines and their line numbers. For example: 

![Image](https://jorryns.github.io/cse15l-lab-reports/lab3.2.png)

Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/

```
grep -rl "word" path
```

The -rl command displays the files that the string is in by recursively searching and then listing the file. For example  

```
-rl 'Lucayans' written_2
```
displays the Bahamas file in the command line.

```
written_2/travel_guides/berlitz2/Bahamas-History.txt
```

Source: Chatgpt
