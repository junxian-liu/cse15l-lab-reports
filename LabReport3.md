# Lab Report 3 - Junxian Liu

The command that I will be looking further into is `grep`. <br>

## grep -R
Input:<br>
`grep -R france written_2` <br>
Output:<br>
`written_2/travel_guides/berlitz1/WhereToFrance.txt: Maison de la France Web site (<www.franceguide.com>) is also a` <br>

Input: <br>
`grep -R hawaii written_2` <br>
Output:<br>
`written_2/travel_guides/berlitz1/HandRHawaii.txt: <www.hawaiianvillage.hilton.com>. Waikiki’s largest resort
 written_2/travel_guides/berlitz1/HandRHawaii.txt: <www.royal-hawaiian.com>. Waikiki’s “Pink Palace,” built by the
 written_2/travel_guides/berlitz1/HandRHawaii.txt: <www.volcano-hawaii.com>. Brian and Lisha Crawford are the kings`<br>
 
 <br>
 -R prints the searched pattern in the given directory recursively in all the files. <br>
 This command could be useful to search for a specific term inside of your directory. Not only does it print out the statement containing the term, 
 it also prints out the path to the file that contains the term. 
 
## grep -A
 
 Input:<br>
 `grep -A1 hawaii written_2/*/*/*` <br>
 Output: <br>
 `written_2/travel_guides/berlitz1/HandRHawaii.txt:        <www.hawaiianvillage.hilton.com>. Waikiki’s largest resort
  written_2/travel_guides/berlitz1/HandRHawaii.txt-        covers 22 beachfront acres of gardens, lagoons, waterfalls, coconut`
 <br>
  
 Input: <br>
 `grep -A1 france written_2/*/*/*` <br>
 Output: <br>
 `written_2/travel_guides/berlitz1/WhereToFrance.txt:        Maison de la France Web site (<www.franceguide.com>) is also a
  written_2/travel_guides/berlitz1/WhereToFrance.txt-        good starting place; the section called Discover the Regions of France`<br>
 
  <br>
 -A prints the searched line and n lines after the result<br>
 This could be useful for when trying to find a specific term in the diretory. In addition to that, this command also prints out the line
 after the line with the term so there is context provided of how the term is being used. 
 
## grep -i
 
 Input:<br>
 `grep -i shinjuku-dori  written_2/*/*/*`<br>
 Output: <br>
 `written_2/travel_guides/berlitz1/WhereToJapan.txt:        A longish walk along Shinjuku-dori from the station will` <br>
 
 Input:<br>
 `grep -i oahu written_2/*/*/*` <br>
 Output:<br>
 `written_2/travel_guides/berlitz1/HandRHawaii.txt:        Oahu (Including Honolulu)
  written_2/travel_guides/berlitz1/HandRHawaii.txt:        on the west side of Oahu, expertly managed by JW Marriott, Ihilani is`<br>
  
  <br>
  
  Similar to -A and -R, -i searches the directory and finds lines that contains the specified phrase. If found, it prints out the location and the 
  line of the text containing the word. This is useful if you want to find all occurences of a certain word in a diretory. 
  
## grep -c
  
  Input: <br>
  `grep -c "hawaii" written_2/*/*/*/*` <br>
  Output: <br>
  `written_2/non-fiction/OUP/Abernathy/ch1.txt:0
   written_2/non-fiction/OUP/Abernathy/ch14.txt:0
   written_2/non-fiction/OUP/Abernathy/ch15.txt:0` <br>
  Input: <br>
  `grep -c "france" written_2/*/*/*`<br>
  Output: <br>
  `written_2/travel_guides/berlitz1/HandRHawaii.txt:0
   written_2/travel_guides/berlitz1/HandRHongKong.txt:0
   written_2/travel_guides/berlitz1/HandRIbiza.txt:0` <br>
   
   <br>
   Unlike -A, -R, and -i, -c prints an output of a count of the number of matching lines with the phrase within the directory.
   It's useful when wanting to know how many times a word appears in each file without having to look through the text files individually.
<br>

## Sources
[Source 1](https://www.computerhope.com/unix/ugrep.htm) <br>
[Source 2](https://www.geeksforgeeks.org/grep-command-in-unixlinux/) <br>
For both of these sources, I did a simple google search for different grep commands I could use in the terminal. Through looking through a few articles, 
I found both of these sites quite useful in understanding how different commands worked so I went with them. aklxalksndasd
