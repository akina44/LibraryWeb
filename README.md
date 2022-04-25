# LibraryWeb
 LibraryWeb
### INTRODUCTION
## 1.1- What is Scrum?
Scrum is an agile framework for developing, delivering, and sustaining complex 
products,[1] with an initial emphasis on software development, although it has been used in 
other fields including research, sales, marketing and advanced technologies.[2] It is designed 
for teams of ten or fewer members, who break their work into goals that can be completed 
within time-boxed iterations, called sprints, no longer than one month and most commonly 
two weeks. The Scrum Team track progress in 15-minute time-boxed daily meetings, called 
daily scrums. At the end of the sprint, the team holds sprint review, to demonstrate the work 
done, and sprint retrospective to improve continuously.
### 1.2-What is Customized Visual Bookshelf from Gutenberg Project?
The aim of the project is to design and implement a user friendly interface for 
searching books from Gutenberg project and collecting the chosen books in a visual bookshelf 
for a specific user of the system. Every user should see his own bookshelf when logs in and he 
should be able to change the books in his/her own shelf by making new searches. Or he/she 
can simply remove one book from his shelf if the book is finished. The system should also 
keep track of the point/page where the user paused reading. Addition to the visualized 
bookshelf, a pop-up screen can be useful to show user which book is paused where.
### 1.2.1-What is Project Gutenberg?
Project Gutenberg is an online library of free eBooks. Project Gutenberg was the first 
provider of free electronic books, or eBooks. Michael Hart, founder of Project Gutenberg, 
invented eBooks in 1971 and his memory continues to inspire the creation of eBooks and 
related content today.
### 1.3-How We Worked? 
We held live meetings on discord at least 3 days a week and at least 2 hours a day since the 
beginning of December. We usually do everything we do together, blend what we do personally and 
create new content together. We tried to help each other in every way even though one of us did not 
understand.
## DEVELOPMENT 
### 2- Specific Requirements
2.1-User Requirements Eliciation: 
1. The System shall allow guests to create an account and become registered users.
2. The system shall allow users to customize their bookshelves by providing options 
to deleting, adding or categorizing books. 
3. The system shall show the book’s cover along with it’s name.
4. The system shall show the last read page of the book to the user.
### 2.2-System Requirements Specification: 
1-Every non-registered user of the system needs to sign-up to use the features.
2-System will take the user to the sign-up screen to allow them to enter their e-mail’s 
and passwords.
3-System will seperate each account with a specific tag to give users privatization and 
customization. 
4-Every registered user of the system will have a functioning Bookshelf.
5-Users will be able to search the books.
6-Users will be able to see the book’s categories, add them to their Bookshelf and 
read.
7-Users will be able to categorize the books on their Bookshelf.
8-Users will be able to delete or discard the books they read from the Bookshelf.
9-Users will be able to search the books from Gutenberg Project’s database.
10-Users will be able to see the books’ name and cover along with an small 
information text.
11-Users will be able to select the file type of the book they added to their library or 
download them.
12-If the users choose to not download and use the system itself, the system will save 
the last page read in the users’ information in the database.
### 2.3-Funtional Requirements: 
1. Login: Allows the user to log into the system.
2. Register: It allows the user to register to the system using the 
information(email,name,password).
3. Book adding: allows the user add book own shelf.
4. Book removing: allows the user remove book from own shelf.
5. Reminder: Remind the user which book is paused. 
6. Searching:System allows the user to search book.
2.4-Non-functional Requirements: 
1. The user must registered on system for reading book.
2. The user have personal book shelf.
3. The user can add and remove book(s) from own shelf.
4. The user can mark the page in the book.
5. The system remind marked page for user.
6. The user can search the books by genre, year of publication, title, author on 
the system.
7. The system should provide loging in the user in 5 seconds.
8. The site should load in 3 seconds.
9. Passwords should never be viewable at the point of entry or at any other 
time.
## 3-Scenarios and Use Cases 
 ### 3.1-Scenario Name: createAnAccount 
Participating Actor Instances: zoe:User, zoe:Guest, site:UserSystem
##### Flow of events:
1. Zoe wants to read books and she enters the site as a guest
2. Zoe sees that she needs to sign-up for using the system
3. Zoe clicks on the “sign-up” button and site redirects her to another page
4. Zoe enters her e-mail, her username and her password
5. Zoe confirms that she has read the “Terms and Conditions”
6. Zoe clicks on the continue button
7. Site redirects her to the main page.
8. Zoe clicks on the “log-in” button
9. Zoe enters the username and password she registered with
10. Zoe starts to use the site
### 3.2-Scenario Name: addBooks 
Participating Actor Instances: adam:User, bookshelf:BookshelfSystem
##### Flow of events:
1. Adam wants to read books and he logs in to his account.
2. Adam is directed to the Bookshelf
3. Adam clicks on the “search” button
4. Adam types book name, author name or book’s category
5. Bookshelf shows the book or books he wants to Adam
6. Adam clicks on the book to add it to his Bookshelf
7. Adam closes the search and returns to the Bookshelf
### 3.3-Scenario Name: removeBooks 
Participating Actor Instances: emily:User, Bookshelf:BookshelfSystem
##### Flow of events:
1. Emily enters the site to organize her Bookshelf
2. Site greets Emily with the information about her last read book
3. Emily closes the window and sees her books
4. Emily sees the books she finished
5. Emily clicks on the books she wants to remove 
6. Emily removes the books one by one from her bookshelf
### 3.4-Use case name: SignUp 
Participating actors: Initiated by Guest
Communicates with User and UserSystem
##### Flow of events:
1. The Guest clicks on the SignUp button to register to the site.
2. The Guest is welcomed by the registration page.
3. The Guest enters their information and confirmes that they read the Terms and 
Conditions.
4. The Guest clicks on the Continue button and the UserSystem redirects them to the 
main page.
5. The Guest clicks on the LogIn button and logs in to the site as a User.
Entry conditions: The Guest must not have opened an account with the same 
information before this request.
##### Exit Conditions:
- UsersSystem rejects the information entered .OR
- UserSystem accepts the information entered.
3.5-Use case name: SearchAndAddBooks 
Participating Actors: Initiated by User
Communicates with BookshelfSystem
##### Flow of events:
1. The User opens the Bookshelf by logging in to the site
2. The User is welcomed with the Bookshelf page
3. The User clicks on the Search button to find book/books
4. The User enters the information they want to find
5. The User is greeted with the book/books based on the information they entered
6. The User clicks on the book/books they want to add and add them one by one
7. The User closes the search screen and returns to the Bookshelf
Entry Conditions: The User must log in to use this function.
Exit Conditions: The User must be at the bookshelf’s capacity. OR
The User must exit the system.
3.6-Use case name: RemoveAndRemindBooks 
Participating Actors: Initiated by User
Communicates with BookshelfSystem
##### Flow of events:
1. The User opens the Bookshelf by logging in to the site
2. The User is welcomed with the Bookshelf page
3. The User is sees a pop-up window with the last page information of the last read
book
4. The User closes the window and continues to the Bookshelf 
5. The User clicks on the book/books they want to remove 
6. The User removes the books one by one
Entry Conditions: There must be books in the Bookshelf
Exit Conditions: All books must be removed. OR
The User must exit the system.
