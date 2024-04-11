# E-learning-Platform
A Simple E-Learning website made using Flask and HTML.It includes portals for both students and teachers where students can acess or enroll into courses and teachers can create, update or delete courses and check out students enrolled into their courses.

Demo for this project can be checked out here:

https://drive.google.com/file/d/1veNZjlS3QmYlrcxF6jQpOVvBPnuwnXGU/view?usp=drivesdk

You can register/login from the home page. The registration system has a 2 step verification system, where once you enter your details like  Email, password and if you are a teacher or not. Once these details are entered you will get a mail for OTP, which you have to enter in the portal. This was made using Flask-Mail.

Once registered you can login. After login you will be redirected to the respective dashboard, depending on whether you are a student or teacher. You can't access the course details without logging into your accounts.
In Student Dashboard, a student can access course material for the courses they have enrolled and can see relevent details of all the courses

# Attributes of USERS Table:
- Id
- Email
- Password
- Role (teacher or student)
- OTP
# Attributes of COURSES Table:
- Id
- User_id
- Duration
- Price
- Emai_Id(of teacher)
# Attributes of PURCHASES Table:
- Id
- User_Id
- Course_Id
- Student_email

To run this project first create database, and add that in the SQL URI in main.py, create the tables mentioned, check the details and more specification on each attribute in the models.py. Install all libraries within a virtual environment as mentioned in the main.py and then run it. Note: dont forget to change the config details in the app.py to get the notifications on the mail.
