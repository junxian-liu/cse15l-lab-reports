# Lab Report 3 - Junxian Liu

The command that I will be looking further into is `grep`. <br>

### grep -R
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
 it also prints out the path to the file that contains the term.  <br>
 
 ### grep -A
 
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
 after the line with the term so there is context provided of how the term is being used. <br>
