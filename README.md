![The Infinite Loopers](https://i.imgur.com/3qSxZjk.png)
### Team L02_11
#### Abhay Vaidya, Felix Chen, Julian Barker, Ruyin (Olivia) Zhang, Tito Ku

WeBWorK is a proof-of-concept Java desktop application for courses that incorporate multiple-choice quizzes and assignments.

#### Features include:
- Assignment Creation with unlimited number of multiple-choice questions
- Assignment editing
- Multiple tries to complete assignments
- Viewing and exporting assignment results
- Assignment remark system
- Course feedback system


### WeBWorK Welcome Page
![webwork_login_page](https://user-images.githubusercontent.com/12486014/33279148-910ea0ce-d36b-11e7-89aa-b4e7bc09fc7f.png)

### Admin Instructor Registration Information
![admin_prof_info](https://user-images.githubusercontent.com/12486014/33287182-e15222bc-d385-11e7-8497-944a01007753.png)

### Non-Admin Instructor Registration Information
![general_prof_info](https://user-images.githubusercontent.com/12486014/33287204-f4332e80-d385-11e7-8a65-4a75dbf41351.png)

### Student Registration Information
![student_info](https://user-images.githubusercontent.com/12486014/33287221-04cbbbc2-d386-11e7-81bb-43f3b6e3e16e.png)

### Instructor Dashboard
![instructor_listing](https://user-images.githubusercontent.com/12486014/33287244-136a5fda-d386-11e7-8838-807431896c73.png)

### Assignment Creation
![assignment_creation](https://user-images.githubusercontent.com/12486014/33287260-26d5ff66-d386-11e7-9ed7-68c38d7ef642.png)

### Assignment Editing
![editing](https://user-images.githubusercontent.com/12486014/33287281-35bfdda8-d386-11e7-8408-8d49a4f1ea15.png)

### Student Dashboard
![student_dashboard](https://user-images.githubusercontent.com/12486014/33287304-4f7666d6-d386-11e7-88ca-22b13f89da6a.png)

### Assignment Completion
![assignment_completion](https://user-images.githubusercontent.com/12486014/33287329-5f6352c0-d386-11e7-894e-3b7823347e25.png)

### Submission Summary
![submission_summary](https://user-images.githubusercontent.com/12486014/33279216-d09bd590-d36b-11e7-8ada-e9d9296bd0a5.png)

### View Assignment Results
![view_result](https://user-images.githubusercontent.com/12486014/33287356-70ab448e-d386-11e7-9649-8986d3e34e92.png)

### Export Assignment Marks
![export_marks](https://user-images.githubusercontent.com/12486014/33287391-7d13a6da-d386-11e7-8e61-97d35f23d1f1.png)

### Remark Submission
![student_remark](https://user-images.githubusercontent.com/12486014/33287399-86529cce-d386-11e7-8ae1-139942bd5d95.png)

### Instructor Receiving Remark Submission
![instructor_remak_email](https://user-images.githubusercontent.com/12486014/33287472-c6abcfc0-d386-11e7-8687-02e63405c527.png)

### Instructor Remarking an Assignment
![instructor_remark](https://user-images.githubusercontent.com/12486014/33287498-dc7a03a8-d386-11e7-955b-1318125aca29.png)

### Student Receiving Remark Completion
![grade_adjusted_email](https://user-images.githubusercontent.com/12486014/33287515-e6d4dbb6-d386-11e7-9bb7-d59c2c9df42a.png)

### Student Submitting Course Feedback
![student_feedback](https://user-images.githubusercontent.com/12486014/33287531-fa85c8dc-d386-11e7-86f8-6546763acba8.png)

### Instructor Viewing Course Feedback
![view_feedback](https://user-images.githubusercontent.com/12486014/33279435-8595dd74-d36c-11e7-8542-c43326646996.png)


### User Instructions
##### Setup
- Due to the usage of an external library, JavaMail, if the program is being run through an IDE, the user must reconfigure their Java build path to access the library. The API is found as 5 jar files in the **_lib_** folder in the project and you must add them to your build path.
- Go to `ApplicationDriver.java` under the `controllers` package
- Run `ApplicationDriver.java` and you will see a login/register interface

#### **INSTRUCTOR'S MANUAL**
##### Register
- For first-time users, you must register your account by typing in your valid email address and password
- You will have to check the **_Instructor_** checkbox before clicking **_Register_**
- You will be presented with a screen to ask you input your first name, last name and passcode to finish your registration 
- As an instructor, you will need to provide a valid passcode for the course in order to register as an instructor successfully. If you are the first instructor, you are considered the admin and will be required to set the passcode for all other instructors.
- You will see a popup window notifying you of a successful registration after you have entered all the information properly and submit.

##### Login
- After you have registered successfully, you will be able to log in to the instructor dashboard using the same email address and password that you registered with (it is not necessary to check the instructor box)

##### Creating a Problem Set
- Open the assignment creation panel by clicking the **_+ Add Assignment_** button at the top right corner
- Select a due date of the assignment by clicking the drop-down box on the left top
- Enter the assignment number you are going to create
- Manually enter each problem corresponding multiple choice options
- Preset the solution for each question by clicking the corresponding radio button for the correct multiple choice option
- After you have entered all the required information for the question, you can click **_Add this Problem_** to add the problem to the problem set
- If you have not entered all the required information before clicking **_Add this Problem_**, you will get a popup notification to ask you fulfill all the required text
- Repeatedly do the steps above until you have added all the problems to the problem set for the current assignment 
- Click the **_Create_** button after you have entered all your problems to finish creating the assignment
- As an instructor, you can release and unrelease assignments by clicking the labeled buttons corresponding to the appropriate assignments

##### Assignment Editing
- Click **_Edit_** button on the dashboard beside the assignment that you wish to edit
- Use the drop-down menu to select the question you want to modify
- Once selected, you can edit the problem, the multiple choices, and its solution on the panel directly. Click **_Save Edited Problem_** once you are done editing.  
- If you wish to delete a question, select the question you wish to delete from the drop-down menu, then click **_Remove problem_**
- If you wish to add a new question to this assignment, you need to click **_Clear_** to clear all the default text in the boxes first. Enter the new assignment question, multiple choice options and its solution to the corresponding text fields and then click **_Add new problem_**.
- After you have completed all necessary changes to the assignment, you need to click **_Save_** to save all your changes. After you click **_Save_**, the application will take you back to the dashboard.
- Now your edited assignment will return be listed as **_Unreleased_**. You may now click **_Release_** to release the assignment to the students once more.

##### Grade Analysis & Retrieval
- The class average of each closed assignment is displayed on the dashboard automatically after the assignment due date has passed. You can check out the class average under the _Closed_ assignments session.
- If you would like to export a copy of an excel spreadsheet which includes all the students' performances for a given assignment, click **_Export Mark_** for the assignment data you would like to review. A file-chooser window will open after clicking **_Export Mark_**, you can save the copy of the document to anywhere on your computer by choosing a directory. The new assignment details result file will replace the old file if the file has already existed in the directory you chose. 
- If you would like to get a summary of the performance of an individual student, you can search for their results by clicking **_Search Student_**. After clicking **_Search Student_**, it will open a search panel where you need to enter the student number into the text field and then click **_Search_**. All the marks that this student has achieved in the past assignments will be displayed on the display panel. 

##### Remarks
- All the remark requests would be sent to your email directly through this application system once the student clicks the remark button on their student panel. Check your emails to view all the remark requests.
- If you want to approve a remark request, you can go to your dashboard and click the **_Remark_** button. Enter the student number and the assignment number which you are handling, and the student's final mark to the text box. Click **_Adjust Mark_** to save the changes to the database and the application system will send an email to notify the student of the change of his/her mark automatically. Click **_Cancel_** if you would like to go back to the dashboard. 

##### Feedback
- You can view student feedback by clicking the **_View Feedback_** button at the top corner of the dashboard. 

#### **STUDENT'S MANUAL**
##### Register
- Enter your valid student email address and password, click **_Register_**.
- You will see a screen to ask you to input your first name, last name and student number to complete your registration process.
- You will see a pop-up window says **_Registration Successful_** after you have entered all the information properly when you register.

##### Login
- After you have registered successfully, you will be able to log in to the student dashboard using the same email address and password that you registered with

##### Completing Assignments
- Click **_Open_** on the assignment you want to start
- Answer each question by selecting a multiple choice option
- Click **_Save and Close_** if you have not finished the assignment
- Click **_Submit and Grade_** to grade your assignment and get your mark
- If you click **_Save and Close_**, the application will auto-fill your previous saved answers for each question and set it as the default option when you open the assignment again next time.

##### Auto-marking & Submission Summary
- The application will auto grade your assignment after you click **_Submit and Grade_**. There will be a submission summary to notify you which questions you have got right and which questions you have got wrong for the current submission. Your final mark of this assignment will get adjusted if your current try is better than the highest mark you have got in the history. 
- You can view each assignment submission summary after the deadline for the assignment passed. Find your **_Closed_** assignments and click the **_Result_** button on the assignment result you want to review. You will be able to see your final mark, average mark, number of tries, and time spent as feedback. Click **_Done_** after reviewing it and the application would take you back to the dashboard.

##### Remarks
- Click the **_Remark_** button beside the assignment you wish to get remarked
- Explain why you want a remark in the message box and then click **_Submit_** to request a remark
- The remark will be sent to instructors directly by email and you will be notified if your grade has been changed

##### Feedback
- You can communicate with your professors or TAs by sending them feedback messages. The **_Give Feedback_** button is at the right corner of the dashboard. Click **_Give Feedback_** button to write a feedback message.

###### Note: GitHub may have problems displaying some of our documents. For this reason, it is recommended you download the document instead of using GitHub's preview to view it.
