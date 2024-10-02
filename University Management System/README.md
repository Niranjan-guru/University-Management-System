
# University Management System

This Project is developed based on Java 11 (Swing) and Ant Framework. This System provides a simple user interface with a login system allowed only for ADMIN. 

Please feel free to Share any changes or updates in this Project.
One more MySQL is used as the DBMS in this project.!!!


## Dependencies Required

Please donwload the required dependencies before executing the Project...

Dependencies are:-
   
   1. mysqlconnector.jdbc jar (https://dev.mysql.com/downloads/connector/j/#:~:text=MySQL%20Connector/J%20is%20the%20official%20JDBC%20driver%20for)
   2. rs2xml jar (https://github.com/kenzo44/rs2xml.jar/blob/master/rs2xml.jar) 
   3. jcalendar-tz jar (https://github.com/gmonu/Library-Management-System/blob/master/src/Jar/jcalendar-tz-1.3.3-4.jar)
   [P.S. To donwload, click onto the link given above, and press "View Raw" option it will be automatically donwloaded]

## Support

For support, email niranjanbalaguru63@gmail.com or Ping me at https://www.linkedin.com/in/niranjan-balaguru-0bb84a23b/.




## Authors

- [@guru-niranjan](https://github.com/Niranjan-guru)


## Tech Stack

**Client:** Swing Java, AWT, ANT Framework.

**Server:** MySQL Database Server

**IDE:** NetBeans, MySQL Workbench 8.0 CE

# Installation & Execution

📥 **Import the Project**

```bash
git clone https://github.com/Niranjan-guru/University-Management-System
```
🎉 Clone the repository and navigate to the project folder. 

You will find a **Dependencies** folder containing the required dependencies.

🛠️ **Setup MySQL Database**

Open your **MySQL Workbench** and follow the steps below:

Create a new server connection to localhost.

Create and configure the database:

```sql
-- Create the database and select it
CREATE DATABASE universitymanagementsystem;
USE universitymanagementsystem;

-- Create and populate login table
CREATE TABLE login(admin VARCHAR(20), password VARCHAR(20));
INSERT INTO login VALUES('<your_username>', '<your_password>');

-- Create student table
CREATE TABLE student(
  name VARCHAR(20), fname VARCHAR(20), rollno VARCHAR(20), dob VARCHAR(20), 
  address VARCHAR(20), phone VARCHAR(20), email VARCHAR(20), class_x VARCHAR(20), 
  class_xii VARCHAR(20), aadhar VARCHAR(20), course VARCHAR(20), branch VARCHAR(20)
);

-- Create teacher table
CREATE TABLE teacher(
  name VARCHAR(20), fname VARCHAR(20), empId VARCHAR(20), dob VARCHAR(20), 
  address VARCHAR(20), phone VARCHAR(20), email VARCHAR(20), class_x VARCHAR(20), 
  class_xii VARCHAR(20), aadhar VARCHAR(20), education VARCHAR(20), department VARCHAR(20)
);

-- Create leave tables for students and teachers
CREATE TABLE studentleave(rollno VARCHAR(20), date VARCHAR(20), duration VARCHAR(20));
CREATE TABLE teacherleave(empId VARCHAR(20), date VARCHAR(20), duration VARCHAR(20));

-- Create fee structure table
CREATE TABLE fee(
  course VARCHAR(20), semester1 VARCHAR(20), semester2 VARCHAR(20), semester3 VARCHAR(20), 
  semester4 VARCHAR(20), semester5 VARCHAR(20), semester6 VARCHAR(20), semester7 VARCHAR(20), 
  semester8 VARCHAR(20)
);
INSERT INTO fee VALUES('BTech', 430000, 430000, 430000, 430000, 430000, 430000, 430000, 430000);

-- Create other required tables
CREATE TABLE collegefee(roll VARCHAR(20), course VARCHAR(20), branch VARCHAR(20), semester VARCHAR(20), total VARCHAR(20));
CREATE TABLE subject(rollno VARCHAR(20), semester VARCHAR(20), subject1 VARCHAR(20), subject2 VARCHAR(20), subject3 VARCHAR(20), subject4 VARCHAR(20), subject5 VARCHAR(20));
CREATE TABLE marks(rollno VARCHAR(20), semester VARCHAR(20), subject1 VARCHAR(20), subject2 VARCHAR(20), subject3 VARCHAR(20), subject4 VARCHAR(20), subject5 VARCHAR(20));
📝 Tip: You can copy and paste the entire set of commands into your MySQL Workbench for quick execution! (Or run them one by one if you prefer).
```

🎨 **Icons & Customization**

All necessary icons are available in the icons folder. If you'd like to replace any icon:

Simply swap the image but keep the same file name to avoid errors.
If you face any issues with icons not displaying, feel free to reach out! 📧

🚦 **Ready to Run!**

After completing all the steps, you're all set to run the project. 🎉

Start the execution from the Splash.java file.
Enter the username and password that you inserted into the login table earlier.

✨ **Enjoy managing your university system!** ✨


## Screenshots

![Login Page]("C:\Users\Niranjan\OneDrive\University Management System\Screenshots\About.png")

![Fees Payment Page]("C:\Users\Niranjan\OneDrive\University Management System\Screenshots\About.png")

![About Page]("C:\Users\Niranjan\OneDrive\University Management System\Screenshots\About.png")

![MarkDetails Page]("C:\Users\Niranjan\OneDrive\University Management System\Screenshots\About.png")

![Menu Page]("C:\Users\Niranjan\OneDrive\University Management System\Screenshots\About.png")

![StudentDetails Page]("C:\Users\Niranjan\OneDrive\University Management System\Screenshots\About.png")

![StudentLeave Page]("C:\Users\Niranjan\OneDrive\University Management System\Screenshots\About.png")

