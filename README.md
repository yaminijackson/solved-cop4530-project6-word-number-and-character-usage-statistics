Download Link: https://assignmentchef.com/product/solved-cop4530-project6-word-number-and-character-usage-statistics
<br>
Practice selecting and making use of appropriate STL containers and algorithms to perform tasks.

<strong>Statement of Work:</strong> Implement a program that collects the statistics of word, number, and character usage in a file (redirected as the standard input).

<strong>Requirements:</strong>

<ol>

 <li>Write a program that will read input (from standard input) until end of input is reached (“end of file”), which will count the number of times each word, number, and character appears in the input.</li>

</ol>

<ol>

 <li style="list-style-type: none;">

  <ul>

   <li>A word is defined as a consecutive sequence of letters (‘a’..’z’ or ‘A’..’Z’).</li>

   <li>Words are case insensitive (“AA”, “Aa”, “aA”, and “aa” are the same).</li>

   <li>A number is defined as any consecutive sequence of digits (‘0’..’9′).</li>

   <li>Note that both words and numbers can be of length of 1, that is, contain one letter or one digit, respectively.</li>

   <li>Different sequences represent different numbers. For example, number “001” is different from number “1”.</li>

   <li>Words are separated by any non-letter characters.</li>

   <li>Numbers are separated by any non-digit characters.</li>

  </ul></li>

</ol>

Output specifications:

<ol>

 <li style="list-style-type: none;">

  <ul>

   <li>Your program should track the number of times each word, number, and character appears.</li>

   <li>The program should then output the ten most used characters, the ten most used numbers, and the ten most used words, along with the number of times each of these characters/numbers/words are used.</li>

   <li>Since words are case insensitive, the program should only output the words in lower case.</li>

   <li>The characters, numbers and words should be printed in descending order based on the number of times they are used.</li>

   <li>Breaking ties (for the “Top Tens”):

    <ul>

     <li>When two characters occur the same number of times, the character with the smaller ASCII value should be considered as being used more frequently.</li>

     <li>When two words (or numbers) occur the same number of times, the word (or number) that occurs earlier in the input should be considered as being used more frequently.</li>

    </ul></li>

  </ul></li>

</ol>

<ol start="2">

 <li>An example executable code of the program is provided to you (see below). You should make the outputs of your program match this sample executable. When printing characters, use ‘t’ for tab and ‘
’ for newline. All other characters should be printed normally.</li>

 <li>Write a makefile for your project that compiles an executable called x</li>

 <li>Make use of any appropriate C++ STL containers and algorithms. You should also use C++ string class instead of default c-strings. Here are a few good reference links for the library lookups:</li>

</ol>

<ol>

 <li style="list-style-type: none;">

  <ul>

   <li><a href="http://www.cplusplus.com/reference/stl/">C++ STL Containers</a></li>

   <li><a href="http://www.cplusplus.com/reference/string/string/">C++ string class library</a></li>

  </ul></li>

</ol>

Note that you should select whatever container(s) will make YOUR program’s algorithms the most efficient in terms of growth rate (i.e. “Big-O complexity analysis”).

<ol start="5">

 <li>In a file called txt, write up your analysis of the complexity analysis of the important algorithms and procedures in your program. Note that your analyses will be based on not only the code YOU write, but also on the STL containers you choose for managing your data. Your analyses need to include analysis of at least (but not limited to) each of these necessary tasks:</li>

</ol>

<ol>

 <li style="list-style-type: none;">

  <ul>

   <li>Reading the input set</li>

   <li>Storing the characters / words / numbers in your chosen containers, and setting their tracking values</li>

   <li>Looking up the final tracking info on your character / word / number frequencies</li>

   <li>Deciding on (and accessing for output) your “Top Ten” most frequent list for each case</li>

   <li>Any other important algorithm/tasks you perform to complete the job</li>

  </ul></li>

</ol>

<ol start="6">

 <li>While not a program requirement for submission, it is <em>recommended</em> that you verify your analysis of your program elements by testing larger input sets and also by measuring the actual run time speed of those test runs. You can do this in a program easily by using the ctime library and capturing the returns from the clock() function before and after an algorithm, then subtract the two clock times to see the difference. Conver to seconds by dividing by the constant CLOCKS_PER_SEC. On linprog, you can look up more details at the manual page for clock (man clock).</li>

</ol>

<strong>Example executable, some test cases</strong>

Download a set of 4 sample test files at <a href="https://www.cs.fsu.edu/~myers/cop4530/hw/hw6files/tests6.tar">this link</a>. This is a tar file containing 4 test files (test0, test1, test2, test3). You will need to unpack this tar file in your project directory.

When you create your own executable, you’ll need to re-direct any test files as the standard input to your program, like this:

proj6.x &lt; test0

The provided example executable can be run from linprog, at the location ~myers/dsprog/proj6.x . So, for example, you can run the same test file as in the example above with:

~myers/dsprog/proj6.x &lt; test0




<strong>ABET Assessment</strong>

<strong>This is our assignment that will satisfy the ABET assessment requirement that students in this course are able to do algorithm complexity analysis on chosen solutions to problems.</strong>

