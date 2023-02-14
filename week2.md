# Lab Report 2 - Servers and Bugs (Week 3)

## Part 1

Code for String Server
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String output = "";
    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return output;
        } 
        else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                output = output + "\n" + parameters[1];
                return output;
            }
            return "404 Not Found!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
![Image](https://jorryns.github.io/cse15l-lab-reports/StringServer1.png)

The methods in my code called are handleRequest and StringServer, handleRequest is called when the url path ends in / and contains /add-message, which takes the string query and adds it to the output string called output. The above screenshot shows the string "Hello" being added the output string. The below screenshot shows "How are you" being added to the existing output string, therefore printing both Hello and How are you on two different lines.

![Image](https://jorryns.github.io/cse15l-lab-reports/StringServer2.png)

The methods in my code called are the same handleRequest and StringServer, handleRequest is called when the url path ends in / and contains /add-message, which takes the string query and adds it on to the existing output string called output with a new line seperating the previous query string from this one. 

**Note** Not demonstrated is the error catching involved if the string does not contain add-message which returns 404 not foudnd
## Part 2
```
import static org.junit.Assert.*;
import org.junit.*;

public class test{
  @Test
  public void testReverseInPlace(){
    //failure inducing input
    int[] input = {1,2,3,4,5,6,7,8,9,10};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[]{10,9,8,7,6,5,4,3,2,1}, input);
    //non failure inducing input
    int[] input2 = {3};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{3}, input2);
  }
}

```


![Image](https://jorryns.github.io/cse15l-lab-reports/week2output.jpg)
**Output**
Symptom is for the failure inducing input at element 5 the output is 6 when it was expected to be 5. The symptom for the non-failure inducing input is that the output may be right however it is because of luck. The element just stayed in place and happened to be correct.

Original Code:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
Fixed Code:
```
static void reverseInPlace(int[] arr){
  for(int i =0; i<arr.length/2; i+=1){
  int temp = arr[i];
  arr[i] = arr[arr.length - i - 1];
  arr[arr.length-i-1] = temp;
  }
}
```

This fixes the issue because the bug was the array would only swap the first half of elements because once it hit the 5th element it would go and copy the wrong element. I fixed this by making a temp value to store the original value that is meant to be copied, switching two values at once, and only traversing half way through the array.


## Part 3

Something from the second lab that I learned that I thought was super useful to know was how to create a run a server. This was especially cool when we ran the server on the remote UCSD computer because it was demonstrating the practices needed to host a "local" webserver something that I have been very interesting in learning about. The query method was also cool to learn about, though I can't see any personal practical applications of it yet, however I will be curious to see some widespread applications of them in current webservers.
