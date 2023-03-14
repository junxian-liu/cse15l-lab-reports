# Lab Report 5 - Junxian Liu

For this lab report, I'll be continuing the task from [lab report 3](https://junxian-liu.github.io/cse15l-lab-reports/LabReport3.html) which 
was on researching different commands and ways to use `grep`. <br>
So in this lab report, I'll explore a few more ways we could use `grep`.

## grep "word or phrase"
 
 Input:<br>
 `grep "hawaii" written_2/*/*/*` <br>
 Output: <br>
 `grep: written_2/non-fiction/OUP/Abernathy: Is a directory
  grep: written_2/non-fiction/OUP/Berk: Is a directory
  grep: written_2/non-fiction/OUP/Castro: Is a directory
  grep: written_2/non-fiction/OUP/Fletcher: Is a directory
  grep: written_2/non-fiction/OUP/Kauffman: Is a directory
  grep: written_2/non-fiction/OUP/Rybczynski: Is a directory
  written_2/travel_guides/berlitz1/HandRHawaii.txt:        <www.hawaiianvillage.hilton.com>. Waikiki’s largest resort
  written_2/travel_guides/berlitz1/HandRHawaii.txt:        <www.royal-hawaiian.com>. Waikiki’s “Pink Palace,” built by the
  written_2/travel_guides/berlitz1/HandRHawaii.txt:        <www.volcano-hawaii.com>. Brian and Lisha Crawford are the kings`
 <br>
 
 This command simply searchs for the specific word or phase in all the files of the directory.<br>
 This would be useful if you just wanted to determine if a word is found in the directory and where the word located. 
 <br><br> <br><br> <br><br> <br><br> <br><br> <br><br>
 
 ## grep -l "word or phrase"
 
 Input:<br>
 `grep -l "hawaii" written_2/*/*/*` <br>
 Output: <br>
 `grep: written_2/non-fiction/OUP/Abernathy: Is a directory
  grep: written_2/non-fiction/OUP/Berk: Is a directory
  grep: written_2/non-fiction/OUP/Castro: Is a directory
  grep: written_2/non-fiction/OUP/Fletcher: Is a directory
  grep: written_2/non-fiction/OUP/Kauffman: Is a directory
  grep: written_2/non-fiction/OUP/Rybczynski: Is a directory
  written_2/travel_guides/berlitz1/HandRHawaii.txt`
 <br>
 
 Similar this command simply searchs for the specific word or phase in all the files of the directory like the previous command we talked about.
 However for this command, it only displays the file of where the word or phrase is located, not the actual line it's in.<br>
 This would be useful if you just wanted to know which files the words in but not the exact location and how it's being used. <br>
 
 With more research, I have displayed here two more useful ways we could use the `grep` command to look through a directory and files. 
 While `grep` is mainly used to find and locate phrases in a directory, there are a few ways it can be used to maniupulate and filter texts. 
