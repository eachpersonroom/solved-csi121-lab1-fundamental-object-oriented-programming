Download Link: https://assignmentchef.com/product/solved-csi121-lab1-fundamental-object-oriented-programming
<br>
<h1></h1>

<ul>

 <li>Familiar with java</li>

 <li>Review fundamental object-oriented programming</li>

</ul>

<strong> </strong>An exercise (The exercise will not be marked. You can jump to the Tasks if you already familiar with Java JDK)

<strong>Step1: Installation of Java JDK, and Text Editor. </strong>

<ol>

 <li>Please use the following link to download and install Java JDK on your laptop. Please make sure you download the correct installation file for your operating system:</li>

</ol>

<a href="https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html">https://www.oracle.com/java/technologies/javase/javase</a><a href="https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html">–</a><a href="https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html">jdk8</a><a href="https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html">–</a><a href="https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html">downloads.html</a>

<ol start="2">

 <li>Please use the following link to download the Text Editor.</li>

</ol>

<ul>

 <li>NotePad++ for Windows user: <a href="https://notepad-plus-plus.org/downloads/">https://notepad</a><a href="https://notepad-plus-plus.org/downloads/">–</a><a href="https://notepad-plus-plus.org/downloads/">plus</a><a href="https://notepad-plus-plus.org/downloads/">–</a><a href="https://notepad-plus-plus.org/downloads/">org/downloads/</a></li>

 <li>TextMate for OS user: <a href="https://macromates.com/download">https://macromates.com/download</a></li>

</ul>

<strong>Step 2: Setup the path to run the JDK tools.  </strong>

The point of setting the environment variable is to let programs know in which directory executables like javac can be found.

<ol>

 <li>Open Advanced System Settings</li>

</ol>

In Windows 10 press Windows key + Pause Key, This will open the System Settings window. Go to Change settings and select the Advanced tab. Alternatively, open “Windows search” – you will find it next to the Windows logo

<ol>

 <li>In the search field type in – advanced system settings 2. Click on the match on top of the list</li>

 <li>Set JAVA_HOME Environment variable</li>

</ol>

In “System Properties window” click “Environment Variables…”

Under “System variables” click the “New…” button and enter JAVA_HOME as “Variable name” and the path to your Java JDK directory under “Variable value”

<ol start="3">

 <li>Update System PATH</li>

 <li>In “Environment Variables” window under “System variables” select Path</li>

 <li>Click on “Edit…”</li>

 <li>In “Edit environment variable” window click “New”</li>

 <li>Type in %JAVA_HOME%bin</li>

 <li>Test your configuration</li>

</ol>

Open a new command prompt and type in:

<h1>1.      echo %JAVA_HOME%</h1>

this will print out the directory JAVA_HOME points to or empty line if the environment variable is not set correctly

Now type in:

<ol>

 <li><strong> javac -version </strong>this will print out the version of the java compiler if the Path variable is set correctly or <em>“javac is not recognized as an internal or external command…”</em> otherwise</li>

</ol>




For Mac, please see the details here: <a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">https://www.java67.com/2015/11/how</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">–</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">to</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">–</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">set</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">–</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">javahome</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">–</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">path</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">–</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">in</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">–</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">mac</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">os</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">–</a><a href="https://www.java67.com/2015/11/how-to-set-javahome-path-in-mac-os-x.html">x.html</a>

<h1>Step 3: Try your first Java program, HelloWorldApp.java</h1>

<ol>

 <li>Open you text editor, create a new file and save it as HelloWorldApp.java;</li>

 <li>Please type the following codes character by character. Don’t copy-paste from this page. Remember that errors are your friend at this stage. Try to encounter common errors as early as possible to learn how to fix them.</li>

</ol>

<h1>class HelloWorldApp{   public static void main(String[] args)   {           // Display “Hello world!”  System.out.println(“Hello world!”);</h1>

<strong>   }</strong>

<strong>}</strong>

<ol start="3">

 <li>Open the command line and goes to the folder where you save your java source code;</li>

 <li>Compile the HelloWorldApp.java file by typing “javac HelloWorldApp.java”. If your code has no error, the executable file “HelloWorldApp.class” will be added in the same folder; If there are mistakes in your code, please follow the hints given by the complier and correct the mistakes (debug) in your text editor and repeat this step;</li>

 <li>Run your program by typing “java HelloWorldApp”, then you will see “Hello World” print on your screen. You can modify the display content of your program once your program can be executed. For each modification, you must save the changes and restart from Step 4.</li>

</ol>

<strong> </strong>

<h1>Tasks</h1>

A course management system contains three class, i.e., the Student class, the Subject class, and the Course class (the primary class).

The Student class is used to keep and maintain the personal information of a student. Its field data shall contain some basic information about a student, such as the student name, DOB, sex, student number and etc. With the Student class, Student objects can be created. The Student class shall also provide some mutator and accessor methods to modify and access the field data of Student objects.

The Subject class is used to keep and maintain a subject’s information. Its field data shall contain the subject name, code, session and year, and a student list. The student list shall contain all students enrolled into the subject, and it can be implemented via an ArrayList of Student objects. The Subject class shall also provide the mutator and accessor methods to modify the subject information. More important, it shall contain methods to modify the student list, i.e., to enrol and withdraw students to the subject.

The Course class is the primary class of the system and is used to manage all subjects and students of a particular course. Its field data shall contain the course name, a student list (i.e., all students enrolled into this course) and a subject list (i.e., all subjects that the course contains). The Course class shall provide some methods to access and modify the course name, and the student and the subject lists.

<h2>Task 1: Class design with UML class diagrams (2 marks)</h2>

Based on the above description, you shall complete the design of the course management system with the three classes and draw UML class diagrams (with the UMLet or other professional tools, no hand drawing) to represent your design. You shall use the correct notations in the UML class diagrams and clearly show the field data, methods and associations between the three classes.

<h2>Task 2: Implementation</h2>

Implement your course management system by using Java. The implementation of all classes shall consistent with your UML diagrams. For the testing purpose, please using the following information and procedure in the <em>main()</em> method.

Course Name: Bachelor of Computer Science

Students (4 students): Amy Bell (Female, 01/01/2001, 100001), Bob Brown (Male, 02/02/2002, 200001), Cindy Ma (Female, 03/03/2001, 100003), and David Hintz (Male, 04/04/2000, 100004)

Subjects (2 subjects): CSIT111 (Programming Fundamentals, Spring 2020), CSIT121 (Object Oriented Design and Programming, Spring 2020)

<ol>

 <li>To create the Bachelor of Computer Science Course object, four Student objects, and two Subject objects;</li>

 <li>To add the four Student objects into the student list of the BCS Course object, and the two Subject objects into the subject list of the BCS Course object;</li>

 <li>To enrol Amy, Bob and Cindy into CSIT111 and David into CSIT121, and display the course enrolment information as follows:</li>

</ol>




<em>————————– </em>

<em>Course Name: Bachelor of Computer Science </em>

<em> </em>

<em>Subject Name: Programming Fundamentals (CSIT111, Spring 2020) Enrolled Students:  </em>

<em>Amy Bell                (100001) </em>

<em>Bob Brown            (100002) </em>

<em>Cindy Ma              (100003) </em>

<em> </em>

<em>Subject Name: Object Oriented Design and Programming (CSIT121, Spring 2020) Enrolled Students: </em>

<em>David Hintz           (100004) </em>

<em>—————————- </em>

<ol start="4">

 <li>To withdraw Cindy from CSIT111 and re-enrol her into CSIT121 instead, and display the course enrolment information as follows:</li>

</ol>

<em>————————– </em>

<em>Course Name: Bachelor of Computer Science </em>

<em> </em>

<em>Subject Name: Programming Fundamentals (CSIT111, Spring 2020) Enrolled Students:  </em>

<em>Amy Bell                (100001) </em>

<em>Bob Brown            (100002) </em>

<em> </em>

<em>Subject Name: Object Oriented Design and Programming (CSIT121, Spring 2020) Enrolled Students: </em>

<em>David Hintz           (100004) </em>

<em>Cindy Ma              (100003) </em>

<em>—————————- </em>




<h2>Task 3: Compilation and Testing</h2>

Compile and test your program and make sure the outputs are same as the requirements.


