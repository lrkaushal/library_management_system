## Library Management System

#### The objective of this project is to learn Swing and jdbc.

### The Library Management system provides following functionalities:

* Login
* Add a book
* Search a Book based on Book Title
* Search Books based on Category
* Search Books based on Author
* List All Books along with author information
* Issue Book to Student
* List Books issued to Student based on USN number 
* List books which are to be returned for current date

### Working

* A user can add book by providing the following information, title, ISBN (Book Number), category and Author information (Author Name and Phone Number).
* Book search can be based on book title, or category or Author, when a book is found, entire information has to be printed on the screen. Partial searches to be supported (for example, if user searches by ‘ja’, ‘Java Complete Reference’, ‘Head First Java’ books) should be displayed.
* A user can list all books present in the library and also the books issued to the students using their USN number.
* A book can be issued to a student by first selecting a book from list of books and then selecting the student from the list of partial or complete search result. Also the date of issue is saved while issuing and return date is calculated (i.e. 7 days from issue date).
* Also if the book is not in library, the user should be informed about the unavailability of the book.


### Database Design

Book Table  | -
----------- | ------------------
Book ISBN	| Primary key
Book Title	| Varchar
Category	| Varchar
No of Books	| int

</br>

Author Table	| -
------------ 	| ----------------------	 
Author Name	 	| Varchar
Author Mail Id	| Varchar
Book ISBN		| Foreign KEY, References Book

</br>

Student Table | -
------------- | --------------------
USN			  | Varchar, Primary Key
Name		  | Varchar

</br>

Book ISSUE Table | -
---------------	 | --------------------------------
Issue ID		 | Auto Increment, Primary Key
USN				 | Foreign Key, References Student
Issued Date		 | Date
Return Date		 | Date
Book ISBN		 | Foreign Key, References Book 

</br>

ADMIN Table		| -
--------------- | --------------------
Admin Id		| Varchar, Primary key
Password		| Varchar

</br>
</br>


### Screenshots

* Login Screen

![login1](https://github.com/lrkaushal/library_management_system/assets/73939193/ad1401f2-1b14-4fe4-8e45-8012d6ee7a7c)


</br>
</br>


* Add new Book

![add_book](https://github.com/lrkaushal/library_management_system/assets/73939193/3c25ffc6-58b9-4317-a894-050c3944b1f0)

</br>
</br>

* Search Book

![search_book](https://github.com/lrkaushal/library_management_system/assets/73939193/5f7cf4f0-0f1b-46e2-9ac2-e9d96a0497a9)


</br>
</br>

* List all Books

![list_all_books](https://github.com/lrkaushal/library_management_system/assets/73939193/03127f74-600b-4f9e-b4e0-a80cbdd8dbac)


</br>
</br>

* Issue Book-1

![issue_book](https://github.com/lrkaushal/library_management_system/assets/73939193/f4580489-a667-41af-bdaa-6bafceb3bc9a)


</br>
</br>

* Issue Book-2



</br>
</br>

* List Issued Books



</br>
</br>

* List Books to be returned on current Date

![book_to_return](https://github.com/lrkaushal/library_management_system/assets/73939193/58d938f5-b040-46fe-9c3d-9b607c5353d3)


</br>
</br>

### Tools and Technology used

*	Programming language → java 8
*	Netbeans IDE
*	MariaDB(MySqL)  

### Reference Link: 
[How to create a cardLayout with netbeans GUI Builder](https://stackoverflow.com/questions/21898425/how-to-use-cardlayout-with-netbeans-gui-builder)

### Demo
* Install MariaDB and follow the steps given in [this] file.
* Now download this project and go to [dist folder](https://github.com/git-akshat/Library-Management/tree/master/dist)
* Double click on LibraryManagement.jar and here you go :)
