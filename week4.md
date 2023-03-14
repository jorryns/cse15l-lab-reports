# Lab Report 4
## Step 1
To Login to your user account
1. **Type** ssh cs15lwi23___@ieng6.ucsd.edu
2. press `<enter>`

![image](https://user-images.githubusercontent.com/122568624/224612924-a6f74e86-ec0b-45d7-8c25-b05e7f64adaf.png)

## Step 2
To clone repository 
1. **Type** git clone git@github.com:jorryns/lab7.git (or whatever your ssh link is for the lab)
2. press `<enter>`

![image](https://user-images.githubusercontent.com/122568624/224616292-8ea5179d-6948-4b7c-b88e-ee1bee7ec680.png)

## Step 3
To run tests
1. **Type** cd lab7
2. `<ctrl+c>` javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java `<ctrl+v>`
3. press `<enter>`
4. `<ctrl+c>` java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests `<ctrl+v>`
5. press `<enter>`

![image](https://user-images.githubusercontent.com/122568624/224617311-4991e61e-5bca-494c-b7ba-c6b47e4c0c4a.png)


## Step 4
To edit out the error on line 46 which is to change to 1 into a 2
1. **Type** nano
2. press `<down>` 45 times
3. press `<right>` 6 times
4. press `<backspace>` 
5. **Type** 2
6. press `<enter>`
7. `<ctrl-o>`
8. `<ctrl-x>`
9. **press** y
10. press `<enter>`

![image](https://user-images.githubusercontent.com/122568624/224816989-1e4eed96-004b-49be-ac62-ac40ac9b842e.png)

## Step 5 
To run the tests again in order to ensure they work
 1. `<ctrl+c>` javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java `<ctrl+v>`
 2. press `<enter>`
 3. `<ctrl+c>` java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests `<ctrl+v>`
 4. press `<enter>`

![image](https://user-images.githubusercontent.com/122568624/224817703-3935cc92-0f52-4fd5-8ced-a1ea642aaaf9.png)

## Step 6
To push to git
1. **Type** git add ListExamples.java
2. press `<enter>`
3. **Type** git push
4. press `<enter>`

![image](https://user-images.githubusercontent.com/122568624/224820775-0292361d-5d7b-4279-b69c-c44cb11d153a.png)


