Download Link: https://assignmentchef.com/product/solved-cse240-homework8-you-are-given-a-partially-completed-project
<br>
<h1></h1>

<ol>

 <li>You are given a partially completed project containing:</li>

</ol>




<ul>

 <li><u>header file:</u></li>

</ul>

book.h             (contains the class ‘Book’)




<ul>

 <li><u>C++ files:</u></li>

</ul>

book.cpp          (contains the class function definitions)

hw08q1.cpp    (contains the program to work on array of ‘Book’ objects)




If you use VS, then create an empty C++ project. Then add the header file and CPP files, respectively, into your project as shown in the following screenshot:










If you use ASU General g++, then simply put the .h and .cpp files in one folder and compile with this command:

<em>g++ book.cpp  hw08q1.cpp  -o  out </em>Execute with:

<em>./out </em>




Follow the instructions given in the comments of the hw08q1.cpp and book.cpp files to complete the missing parts of the project so that the program executes properly. You should first complete book.cpp and then go on to hw08q1.cpp. NOTE: In the homework, list means an array (not a linked list).










This is a menu-driven program that uses the following options:

<ol>

 <li>Add a new book. The book details (title, ID, aisle , bookType) are given as function arguments. You should add the book only if the book is not already present in the array and there is space in the array to add a new book.</li>

 <li>Display the all book’s information. See expected output below.</li>

 <li>Display only the books whose ID falls within a range (in descending order)</li>

 <li>Display the book with the longest title among the books whose bookType contain a specific substring. Ask the user for a substring. This function is used to demonstrate garbage collection.</li>

</ol>




You should start completing the program beginning from Q1. Question numbers are given on line 29 in hw08q1.cpp. (Q1 – Q2 in book.cpp and Q3 – Q6 in hw08q1.cpp)




Expected outputs:




<strong><u>addBook( ):</u></strong>

<ul>

 <li>This function adds a new book with the details given in function arguments.</li>

 <li>Add the book in ‘b’ (array of objects) only if there is remaining capacity in the array and if the book does not already exist in the list (title or ID)</li>

 <li>This function returns 1 if the book is added successfully, else it returns 0 for the cases mentioned above.</li>

 <li>Assume user enters ID and aisle in 0 – any positive integer range.</li>

</ul>




<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong><u>displayBooks( ):</u></strong>

<ul>

 <li>This function displays the list of books.</li>

 <li>Parse the object array ‘b’ and display the details of all books in the array. See expected output given in question file.</li>

 <li>You can call the class function ‘displayBook()’ here. Note that these are two different functions.</li>

</ul>

<strong> </strong>

<strong> </strong>

<strong><u>sort( ):</u></strong>

<ul>

 <li>This function sorts the books in descending order of ID, and then display the books within a given range.</li>

 <li>You need to get lower bound and higher bound from user after printing a prompt.</li>

</ul>




<strong> </strong>




<strong><u>bookTypeWithSpecificString( ):</u></strong>

<ul>

 <li>This function displays a book with the longest title among the books whose bookType contain a specific substring.</li>

 <li>You should find the book as follows:

  <ol>

   <li>By traversing all books, you should find the books whose bookType include a specific substring.</li>

   <li>After step 1, you should find the book whose title is the longest. You may use ‘titleLength’ and ‘index’ variable.</li>

   <li>After step 2, copy the details of the book to ‘bookWithLengthyTitle’ object created using ‘new’ and display the book’s details using ‘bookWithLengthyTitle’ object.</li>

   <li>Finally delete the ‘ bookWithLengthyTitle ‘ object.</li>

  </ol></li>

</ul>

<strong> </strong>

<strong> </strong>

<strong> </strong>