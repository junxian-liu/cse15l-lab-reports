# Lab Report 2 - Junxian Liu

For our second and third lab, we worked with servers as well as debugging files. 

## StringServer
<img width="920" alt="Screen Shot 2023-01-30 at 5 06 11 PM" src="https://user-images.githubusercontent.com/81266551/215632728-5ae976ae-b0ae-4dc4-8362-f802ecf00a20.png"><br>
- Java code for StringServer <br><br>

<img width="444" alt="Screen Shot 2023-01-30 at 4 45 36 PM" src="https://user-images.githubusercontent.com/81266551/215630039-fca1387c-1bdf-4e31-9b7b-28df80599e50.png"><br>
First add-message request with the string `Hello` <br>
For this request, the `handleRequest(URI url)` method was called with the argument `http://localhost:4000/add-message?s=Hello` being passed through. 
`String[]` was also updated in regards to the url that was passed into the method. The variables `concatenate` and `request` would be updated respectfully as well. <br><br>

<img width="423" alt="Screen Shot 2023-01-30 at 4 45 46 PM" src="https://user-images.githubusercontent.com/81266551/215630045-5004a22e-e3bd-4d1d-ab45-098d07a6a422.png"><br>
Second add-message request with the string `World` <br>
Also for this request, the `handleRequest(URI url)` method was called with the argument `http://localhost:4000/add-message?s=World` being passed through. 
`String[]` was also updated in regards to the url that was passed into the method. The variables `concatenate` and `request` would also be updated respectfully as well. <br><br>

<img width="385" alt="Screen Shot 2023-01-30 at 4 45 55 PM" src="https://user-images.githubusercontent.com/81266551/215630050-18b34fcd-9a7e-40c9-9d48-5d26fcb6dbb8.png"><br>
- Results when we only type the root path <br><br>

## Bugs from Lab 3
<img width="356" alt="Screen Shot 2023-01-30 at 5 42 36 PM" src="https://user-images.githubusercontent.com/81266551/215637934-4ea4d64e-23b7-4a6c-9b6d-61844f6b3397.png">
- We'll be analyzing this method for it's bugs and the symptoms that come with it. <br><br>

`@Test
  public void testReversedFail(){
    int[] input = {1, 2, 3};
    assertArrayEquals(new int[]{3, 2, 1}, ArrayExamples.reversed(input));
  }
 `<br>
 - As for this Junit test, it would fail with the error: <br><br>
 
 `arrays first differed at element [0]; expected:[3] but was:[0]
 at ArrayTests.testReversedFail(ArrayTests.java:25)
Caused by: java.lang.AssertionError: expected:[3] but was:[0]`<br><br>

`@Test
  public void testReversedTrue(){
    int [] input = {0 ,0 ,0};
    assertArrayEquals(new int[]{0, 0, 0}, ArrayExamples.reversed(input));
  }
 `<br>
 - For this Junit test, with no modifications to the method would pass. <br>

Code before: <br>
`static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
 `<br>
 
Code after: <br>
`static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
 `<br><br>
 In the before code, the method would set the values in the array that we would return, to values of an empty array. So no more matter what array we pass as an argument to the method, the returned array would be an array of empty values. So to fix it, we would set the values of a new array to the array we pass in as a argument in reversed order. Then we would return the reversed new array. <br><br>
 
 ## Things I learned from Lab 2 and 3
 One thing I didn't know but learned during the lab on week 3 was the use of Junit testing and it's application to debugging your code. I found the tool really useful in the aspect that it can test for certain inputs and provide feedback on whether or not those inputs would work and if the code needs to changed. In addition, not only does it work in terms of testing inputs but it can also test your code to ensure that you're getting the outputs that you intend to. If the tests are failing and the output isn't what you want, you know you need to change your code. This tool allows you to code more efficiently.
