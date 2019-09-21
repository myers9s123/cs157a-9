# Project Requirement Document

## Project Description
College Web Portal is a project designed to organize college classes in an efficient manner and make picking the right class easier for students. Every start of the semester, a lot of students find enrolling the right classes very challenging. Newer students might feel lost when picking the right instructor for a course. We also observed some students went to multiple sessions for the same class hoping to get an add code. 

The current enrollment system at San Jose State University does not display any information regarding the instructor. Also, there is no way for students to view how many seats available in a particular course on the enrollment page. Currently, students would have to visit another site and look up these information themselves. College Web Portal is a solution to this problem. It will display all the necessary information within the same domain, allowing easy access to information. Also, it will provide a better user experience for administrators to manage listed classes. For example, it can automatically generate a list of open classes so the department can notify students which classes are available.

College Web Portal would be a web-based application. It’s targeted users are students, professors, and school administrators. The main difference of College Web Portal and current MySJSU portal is College Web Portal provides extra information about the professors. This feature is very convenient to the students. Students do not have to open the SJSU page of faculty and the RateMyProfessor website to learn more about the background of their professors. Learning the background of professors prior to enrolling into their classes help students to make the correct decisions. Students that are thirsty for the knowledge of a particular field could choose the professors that are experts in that area.


## System Environment
### Hardware
Development will be done on local machines running MacOS, Linux and Windows operating systems.

### Software
The web framework for this project is Django, which will run on the Apache web server. Python is the main programming language. For the database portion, MySQL RDBMS will be used. The client side will be web based and include the use of HTML, CSS and Javascript. Bootstrap framework will be implemented to simplify the process of CSS styling.

## Functional Requirements

### User Access
Users will access the web application through a web browser and will authenticate via student ID and password. The system will support three main types of access, each with different levels of read and write capability to data entities. The three types of access are student, professor and administrator. 

### Functions

#### Authentication
Each user of the system will authenticate to gain access to their protected account data.

#### Account Settings
Each user has the ability to update their account settings such as password and communication preferences.

#### Course Search
Each user is able to search through the database of available courses and view the details of each course such as the instructor, pre-requisites, location on campus, general course description, dates when the course will be held and number of available seats.

#### Course Actions
Student users are able to add, drop and waitlist courses.

#### Course Records
Student users are able to view a list of past courses that they have taken and view details including the grade that they obtained.

#### Professor Search
Each user is able to browse current professors of the university by department and also search professors by keyword. They may also view public profiles of each professor.

#### Professor Profile
Instructors are able to manage their public profile and update details such as their profile picture, background, credentials, office hours and contact information.

#### Course Administration
Administrators of the web application such as school faculty are able to manage available courses including searching available courses, creating new courses, editing existing courses and deleting courses.

#### User Administration
Administrators are able to manage student/professor/admin accounts including searching, viewing, editing and deleting accounts.

#### Campus Administration
Administrators are able to manage campus data such as registered buildings on campus, rooms, capacity limits and available areas of study (subjects).


## Non Functional Issues

#### GUI Tools
GUI tools include the use of the web browser inspector and console in order to finely tune the user interface. Developers will use code editors of their choice including vim, VSCode and PyCharm. The Bootstrap web library will be used to promote swift development of the client side GUI and to give a professional presentation to the web pages.

#### Access Control
Access control will be handled by Django’s built in user authentication and groups systems. Students will have access to course search, professor search, account settings and the ability to manage their course sections. Professors will have access to manage their public profile, account settings, course search and professor search. Administrators will have access to manage available courses, manage course waitlists, manage registered professors, update the school’s available campus buildings/rooms, manage student accounts and manage account settings.

#### Security
College Web Portal is going to ensure the security of each user through open source authentication APIs. This prevents unauthorized user to access the data of the other users in the system. Administrators could monitor the users to observe any strange activities.

#### Scalability
The main target of College Web Portal is SJSU students and faculties. However, if it performs well and gets good feedback from SJSU, it could be promoted to other campuses. This happens because most campuses have the same problems too.
