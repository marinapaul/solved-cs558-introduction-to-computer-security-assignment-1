Download Link: https://assignmentchef.com/product/solved-cs558-introduction-to-computer-security-assignment-1
<br>
You can use <strong>either C, C++, Java, or Python</strong> to implement this assignment.

In this assignment, you will implement the monoalphabetic cipher (cs558-02.pdf) to encrypt/decrypt files containing only lower-case letters a-z.  <strong>The file contains only 1 line and does not contain spaces, tabs, and newlines.</strong>  You can assume that the file contains less than 10000 characters.  For each plaintext letter, your program should randomly generate a ciphertext letter based on a seed.  <strong>The seed will be hardcoded in your program.</strong> <strong>The seed should be the same in encryption and decryption so that the same mapping (i.e. the same key) will be used in encryption and decryption. </strong> Different plaintext letters should be mapped to different ciphertext letters.  Different mappings will be generated with different seeds. <strong> </strong>

The program has three arguments: inputfile, outputfile, and 1/0

<ul>

 <li>inputfile: input file name</li>

 <li>outputfile: output file name</li>

 <li>1: encryption, 0: decryption</li>

</ul>




E.g. in C, an example command for executing your program is (assume that the name of your executable is mono):

./mono in out 1: encrypt file in and store the result in file out:

./mono out in1 0: decrypt file out and store the result in file in1

After the above two commands, files in and in1 should contain the same content.

Your program (both encryption and decryption) will print the mappings generated between the plaintext letters and the ciphertext letters.  The mappings will be printed using the format a-c1, b-c2, …, z-c26, where ci is the corresponding cyphertext letter, and c1=c2=…=c26.  E.g.

a-b, b-d, e-h, ……

<u>Submission guideline:</u>

Please hand in your <strong>source code</strong> electronically through mycourses.binghamton.edu (<strong>please do not submit .o or executable code</strong>).  Your code should compile and run correctly on bingsuns.binghamton.edu or remote.cs.binghamton.edu.  If you do not have access to remote.cs, please let me know.

<ul>

 <li>Write a <strong>README</strong> file (<strong>text file, do not submit a .doc file</strong>) which contains

  <ul>

   <li>Your name and the email address</li>

   <li>The programming language used</li>

   <li>Whether your code was tested on bingsuns or remote.cs.</li>

   <li>How to compile and execute your program.</li>

   <li>(Optional) Anything special about your submission that you would like take note of.</li>

  </ul></li>

 <li>Place all your files under one directory with a unique name (such as p1-[userid] for assignment 1, e.g. p1pyang).</li>

 <li>Tar the contents of this directory using the following command.</li>

</ul>

<strong>tar –cvf [directory_name].tar [directory_name]</strong>

E.g. tar -cvf p1-pyang.tar p1-pyang/

<ul>

 <li>Use mycourses to upload the tared file you created above.</li>

</ul>