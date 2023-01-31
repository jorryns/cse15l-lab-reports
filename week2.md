# Lab Report 2 - Servers and Bugs (Week 3)

## Part 1

## Part 2
```
import static org.junit.Assert.*;
import org.junit.*;

public class test{
  @Test
  public void testReverseInPlace(){
    #failure inducing input
    int[] input = {1,2,3,4,5,6,7,8,9,10};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[]{10,9,8,7,6,5,4,3,2,1}, input);
    #non failure inducing input
    int[] input2 = {3};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{3}, input2);
  }
}

```

## Part 3
