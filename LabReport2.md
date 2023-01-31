# Lab Report 2 - Junxian Liu

For our second and third lab, we worked with servers as well as debugging files. 

## StringServer
<img width="920" alt="Screen Shot 2023-01-30 at 5 06 11 PM" src="https://user-images.githubusercontent.com/81266551/215632728-5ae976ae-b0ae-4dc4-8362-f802ecf00a20.png">
- Java code for StringServer <br><br>

<img width="444" alt="Screen Shot 2023-01-30 at 4 45 36 PM" src="https://user-images.githubusercontent.com/81266551/215630039-fca1387c-1bdf-4e31-9b7b-28df80599e50.png">
First add-message request with the string `Hello` <br>
For this request, the `handleRequest(URI url)` method was called with the argument `http://localhost:4000/add-message?s=Hello` being passed through. 
`String[]` was also updated in regards to the url that was passed into the method. The variables `concatenate` and `request` would be updated respectfully as well. <br><br>

<img width="423" alt="Screen Shot 2023-01-30 at 4 45 46 PM" src="https://user-images.githubusercontent.com/81266551/215630045-5004a22e-e3bd-4d1d-ab45-098d07a6a422.png">
- Second add-message request with the string `World` <br><br>
<img width="385" alt="Screen Shot 2023-01-30 at 4 45 55 PM" src="https://user-images.githubusercontent.com/81266551/215630050-18b34fcd-9a7e-40c9-9d48-5d26fcb6dbb8.png">
- Results when we only type the root path <br><br>
