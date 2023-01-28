# Lab Report 1 - Junxian Liu

As part of our first lab, we were tasked with installing VSCode, the process of remotely connecting, and trying some basic commands in our terminal window.

### Installing VSCode
We first tasked with installing VSCode which required us to go to this [link](https://code.visualstudio.com/) and following the instructions prompted to us
to install the application onto our computer. After successfully downloading VSCode, you should open up the application and be promoted with the following
image: <br>

<img width="1440" alt="Screen Shot 2023-01-13 at 11 04 45 AM" src="https://user-images.githubusercontent.com/81266551/212401852-7feaade8-aab2-4fd6-b0c1-4a15d072c4eb.png"><br>

### Remotely Connecting
The next task we had was learning how to remotely connect to our CSE 15L account on our own computers. For Windows computer, they had an extra task of
downloading Git onto their computer prior but since I am on a Mac, it was already installed. In addition, we had to go to this [link](https://sdacs.ucsd.edu/~icc/index.phpto)
find our CSE 15L accounts that we were supposed to connect to. Once we found our account and reset the password for it, we were ready to remotely connect 
to it on our own computer. In our terminal on VSCode, we would type in the following: <br> `$ ssh cs15lwi23zz@ieng6.ucsd.edu` with the "zz" replaced
with the letters of our own account. Lastly, we would be prompted to type in the password that we set for this account. Successful completetion
of this task would like this: <br>

<img width="1440" alt="Screen Shot 2023-01-13 at 11 06 27 AM" src="https://user-images.githubusercontent.com/81266551/212404749-d21ded52-b7f0-40e1-9ce9-012f4bccbf56.png"><br>

### Trying Some Commands
The last task for this lab report would be trying commands after successfully connecting remotely to our CSE 15L account. By typing in commands like: <br>
`cd ~` <br>
`cat /home/linux/ieng6/cs15lwi23/public/hello.txt`<br>
`ls -a` <br>
into our terminal window, we would get certain outputs. 
Successfully completing this task would look like this: <br>

<img width="1440" alt="Screen Shot 2023-01-13 at 11 07 29 AM" src="https://user-images.githubusercontent.com/81266551/212405338-aa21f09b-2982-4dac-a52d-8b2f0ba391fd.png"><br>

Looking at the outputs, running the command `cat /home/linux/ieng6/cs15lwi23/public/hello.txt` would print the contents of the file `hello.txt` that's located in our remote server onto the terminal window. Additionally, running the other command would run in terms of the directory and files located within the remote server that we are connected to. If we were to run these commands when we're not logged onto our remote server, the outputs would be completely different. 

