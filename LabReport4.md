# Lab Report 4 - Junxian Liu
For this lab report, we'll be looking at the tasks that we did as part of a competition during our lab. These tasks required us to 
clone a repository from github account, run tests on the file, debug the files, and then commit the changes we made to github. 

### Step 4 - Log into ieng6
<img width="501" alt="Screenshot 2023-02-27 at 1 54 26 PM" src="https://user-images.githubusercontent.com/81266551/221694615-53184426-12f0-4348-9bb5-0aff798339e1.png">
<br>
This task was fairly simple as it just required us to log into our ieng6 account which is something we have done many times before. 
To log in, we would type `ssh` followed with our ieng6 account. Then when prompted to enter our password, we would then enter our password there. If everything is correct, you would get a message saying you succesffully logged into your account. <br><br><br><br><br><br><br><br><br>

### Step 5 - Clone your fork of the repository from your Github account
<img width="610" alt="Screenshot 2023-02-25 at 5 11 29 PM" src="https://user-images.githubusercontent.com/81266551/221488429-d651c0aa-acbc-4b1e-ad9e-417763cb7a2a.png">
<br>
To start this task, we had to fork the repository tp provided to us in the writeup of the tasks to our personal Github account. From there we had to clone
that repository into our ieng6 account. To achieve this, we type `git clone` followed by the link of the Github link of our repository. If successful, 
we would get the message that it's cloning into our directory.

### Step 6 - Run the tests, demonstrating that they fail
<img width="967" alt="Screenshot 2023-02-26 at 10 19 24 PM" src="https://user-images.githubusercontent.com/81266551/221489140-e008fd3e-da53-42cb-af97-40fa9a62f880.png">
<br>
To start this task, we had to type `cd lab7` to get into the lab7 directory. Once we're done with that, we have compile and run the tests to see
if they pass or not. To do that we typed `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` to compile all java files in the directory 
then `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` to run the tests. After running that last
command, the next message we should see is whether or not the tests passed, and if they failed, the failure message. As for us, we confirmed that the tests failed. <br><br><br><br><br><br><br><br><br><br><br><br><br><br>

### Step 7 - Edit the code file to fix the failing test
<img width="443" alt="Screenshot 2023-02-25 at 5 21 05 PM" src="https://user-images.githubusercontent.com/81266551/221496092-bea41ff8-1285-46da-aafe-aef8cab19528.png">
<img width="652" alt="Screenshot 2023-02-25 at 5 21 29 PM" src="https://user-images.githubusercontent.com/81266551/221496108-07072ed7-817c-42d8-a852-3d48a86fd984.png">
<br>
To complete this task, we had to edit the `ListExamples.java` file so it would pasts the tests. So to do that we had to first type 
 `nano ListExamples.java` so we could get into the file to edit. Then in the screen where we edit the file, I pressed the down key until I got to 
43 because that's where I found the error to be located. Once I got down to line 43, I pressed the right key to edit the `index1` and changed it to
`index2`. Now that everything is updated, we had to write it to the file and confirm the edits. To do so I typed `^O` to write out the edits and 
`<enter>` to confirm the edits. To exit out of nano, I typed `^X`. 

### Step 8 - Run the tests, demonstrating that they now succeed
<img width="963" alt="Screenshot 2023-02-26 at 9 57 51 PM" src="https://user-images.githubusercontent.com/81266551/221496206-d74114b1-c59d-42f7-9c2e-92ca195d7845.png">
<br>
Just like step 6, we had to recompile our code then run the tests again to check if they succeed now. Since we already typed the javac and java paths, 
I just had to type the up keys several times to go back in my history to where I typed it. Once I got back to the line where I typed it, I typed
`<enter>` to reenter the command. Doing that for both javac and java, we see get confirmation that now our `ListExamples.java` file passed the tests. 

### Step 9 - Commit and push the resulting change to your Github account
<img width="526" alt="Screenshot 2023-02-26 at 10 03 11 PM" src="https://user-images.githubusercontent.com/81266551/221496292-dcbd513a-4675-406c-b288-b5e3f95ec342.png">
<br> 
To commit and push the edits to our Github account, we first typed `git add ListExamples.java` as the edits to that file are the ones we want to
commit. After preparing those edits to be committed, I then typed `git commit -m "Updated"` to commit the edits to my Github account. That command commited the changed with the message of "Updated".

