# project1CS3377
# Author: Nguyen Do (npd220001), CS 3377 003
# Project name: Date_Extractinator_9000 (i made that up sorry)
  This program extracts date from the user's input of a text file. The script name is project1.sh
  Before starting the program.
  Please read the instruction below:
# INSTRUCTIONS
  1. Type in bash project1.sh
  2. A prompt will appear on the console "Hello! This program detects all dates in a text file. Enter a file name: "
     - Enter the file name that you want to extract the dates from. (Type in the exact file that you want to have the dates to appear and have that file ready! Ex: input.txt). Press Enter.
  3. Another prompt will appear on the console "Now enter a file name that you want the dates to appear in: "
     - Enter the file name that you want to show the dates on. (Type in the exact file that you want to have the dates to appear and have that file ready! Ex: output.txt). Press Enter.
  4. After Step 3, nothing should appear in the console. The dates will show on the output file you have selected in Step 3. The program extracts all of the possible date formats (to my knowledge) from your input file and the output file displays these dates. Beneath you have the date count, showing how many dates appear in the file.
# MAIN CONCEPTS
  The stars of the script are regular expressions and the grep command. 
  This program is designed to extract date formats that I have seen in my life. However, I have also accumulated many more new formats that I also included in my code.
  The regular expressions contain a range of date formats, from "04/12/2005" to "April 12th, 2005" to "the Twelfth of April, 2005". These are considered the maximums of the dates (having the day, month, and year). Sometimes a component is optional, so I've learned the basic uses of special characters and add changes on top of these regular expressions.This allows me to save more time in writing more redundant regular expressions that may interfere with similar ones, and it also makes the code more readable.
  The grep command is very useful in capturing multiple of the regular expressions at once. I also learned to use grep -Eo that prints the specified patterns of regular expressions as opposed to printing the entire line including the date. grep also helps in counting the dates as I combine it with the "wc" keyword to count the occurrences of dates.
# MOTIVATION
  The goal of this project is for me to gain practice in regular expressions and grep. Before this project, I have only worked with grep once and was new in regular expressions. However, I learned so much about many ways you can shape regular expressions and creativity also becomes its fullest. One indirect impact is that I grow more fond of Unix and that I was able to explore more commands that can make this project work.
# COMMENTS
 In the code there are comments and pseudocodes. The pseudocodes help explain the overall function of the program. The comments explain each component of the program and each format of the regex.
# SAMPLE INPUT FILE
  I was born on April 12th, 2005. I was born in Vietnam. I first ate cheese on January 20th, 2010.
# SAMPLE OUTPUT
  On Console: "Hello! This program detects all dates in a text file. Enter a file name: " *enters story.txt*
  On Console: ""Now enter a file name that you want the dates to appear in: " *enters output.txt*
  On output.txt: "April 12th, 2005
                  January 20th, 2010
                  Hello! you have 2 dates."
# ENDNOTE
  Thank you for spending time reading the README. I hope the program works! It is a great project to test my knowledge and boundary in grep and regular expressions.
