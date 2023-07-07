# COSC481W-Team3-FinalProject
Final semester-long project for Senior capstone, COSC-481W
This was a web app employee scheduler made for a local McDonald's franchise as part of our senior project.
It has a PHP backend with an HTML and CSS frontend as well as an email server written in Node.js.

**User manual:** 
The McDonald’s Employee Portal provides two different login screens: one for regular crew members and managers, and one for the General Manager and any managers with scheduling powers (Managers are able to switch crew/admin responsibilities at any time). Both also have access to pages to reset their password. To log out, simply close out the page.

**Crew Members and Managers:**
If this is the first time using the portal, make sure to follow the link sent in your email OR follow the link from the login page that says, first-time user. This will allow you to enter a password to be able to access the portal successfully.
If it is not the first login, use the login screen labeled as Login to Employee Portal. Provide your employee id number and password to be able to get access to the portal. Once logged in, you’ll be on the home page of the portal. There are three different actions you can take. 

**View Published Schedules:**
After clicking on this button, you are able to select between the current week and next week by means of a drop-down menu. If there are no posted schedules for this week, nothing will be displayed. If the posted schedule has the wrong dates, the GM should be notified. To return to the Home Page, click on the button at the top of the page.

**Change Availability:**
After clicking on this button, you are able to change your availability. Simply input the start time and end time for every day of the week (0:00 am for not available), and then press submit before returning to the home page.

**Request Time Off:**
After clicking on this button, you are able to request time off. Be sure to select the date range, and the reason why. If this isn’t submitted 2 weeks in advance, it will not be accepted. Again, submit before returning to the home page.

**General Manager and Scheduling Managers:**
Use the login screen labeled as Login to Manager Portal. Provide your employee id number and password to be able to get access to the portal. Once logged in, you’ll be in the home page of the portal. There are four different actions you can take. 

**Manage Employees:**
After clicking on this button, you will be able to view all current employees. You are able to modify any information about them along with their “Admin” status. By being an administrator, they will be able to access the manager portal to change schedules. You are also able to add new employees, by providing all information for them and clicking submit. You are also able to delete employees from the database.

**Edit or Publish Schedules:**
After clicking on this button, you are able to select between the current week and next week by means of a drop down menu. If there are no posted schedules for this week, nothing will be displayed. These must be constantly updated by you, simply choose a picture to publish. Next week’s will not transfer to the current week, you must do that promptly at the end of the week.

**View All Employees Availability:**
After clicking on this button, you are able to view all availability requests. Acknowledge requests after viewing them if you do not need them to catch your attention again.

**View Time Off Requests:**
After clicking on this button, you are vew all time off requests. To view the full request, click on the request you wish to see. Requests need to be approved or denied. Submit before returning to the home page.

**Implementation manual:** 
* **Problem statement:**
The McDonald’s at the current location where one of our team members work needed a new way to distribute schedules, and deal with availability and time off requests. The current app they use is not user friendly and very finicky to use. So we provided a possible solution to this problem.
System requirements:
The system’s biggest requirement was that it needs to be user friendly. It needs a simple UI that anyone can use. Aim for a home page that has a minimal amount of buttons to other pages. These other pages must link back to the home page only. Also, there must be a manager login for admins that can edit and view sensitive information, and a regular login for crew members.
It also must be able to be translated to other languages, since this McDonald’s is culturally diverse. There’s probably a google extension that can be used. It must also be easily accessible, so a website would be the best route.
Must be able to have a secure database since there will be sensitive information stored.
Must have a secure login, and not store login information.
Employees:
View published schedules - A page specifically with this purpose. Up to 2 weeks are visible. Drop down menu to choose from. It will simply be displaying an image.
Submit availability changes - A page for availability requests. Ideally, modify all 7 days of the week at once.
Time off requests - A page for time off requests. Must not go through if it is not two weeks in advance. All fields must be filled out: start date, end date, reason for request.
Admins:
Manage Employees - Manager is able to see all employees on this page. All employee information is able to be edited. Employees can be changed from crew to admin and vice versa on this page. Manager can add an employee here, by adding all information (name, id, phone number, email, admin status, etc). Employees can also be deleted.
Publish and update schedules - A page for this purpose. Manager can choose which week it is from a drop down menu. Must update an image.
Acknowledge availability changes - A page for this purpose. Manager can acknowledge requests to send a notification out to employees.
Approve/deny time off requests - A page for this purpose. Manager must be able to approve or deny requests. This action sends a notification to the respective employee.

