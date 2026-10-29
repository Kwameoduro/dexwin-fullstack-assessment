# Bugs for TaskFlow App

## TF001: Subsequent Project Selection fails to show associated task in UI
Description: On the taskflow application, selecting another project after a project is selected fails to show the associated tasks.


### Test Data
First Selected project = Website Redesign

Second Selected Project = Marketing Site Q3 

### Test Environment
Application URL = https://scary-spider-67x59gr97xwcr77p-5173.app.github.dev/

OS: Windows 11

### Reproduction Steps
1. Open the application URL in your search box.
2. Select a project (Website Redesign Project) and observe the associated tasks.
3. Select another project (Marketing Site Q3) and observe it associated tasks.

### Expected Results
After observing the associated tasks of the Website Redesign Project, clicking on the marketing site q3 should display the its associated tasks as well.

### Actual Result
The tasks page stays the same and does not show the tasks associated with the Marketing Site Q3 project.


### Severity
Critical (This is crtitical because the available tasks should show for every associated project. Also, it is a major functionality.)

### Priority
High


### Evidence
<img width="890" height="440" alt="bug 2" src="https://github.com/user-attachments/assets/1117b72b-07b2-44ce-98a7-1659c9fdc176" />
<img width="932" height="454" alt="bug 1" src="https://github.com/user-attachments/assets/9e83895d-10f6-4eb2-835c-b032e67b4810" />



## TF002: The is no notification and Update in the UI when changing the Status of tasks.
Description: On the taskflow application, changing the the status of a task from Complete to another status does not show any notification and changed state in the UI after clicking on the status change button. And the user might not know 
if the transition is done or not.

### Precondition
A project is already selected.

### Test Data
First Selected project = Website Redesign

### Test Environment
Application URL = https://scary-spider-67x59gr97xwcr77p-5173.app.github.dev/

OS: Windows 11

### Reproduction Steps
1. Open the application URL in your search box.
2. Select a project (Website Redesign Project) and observe the associated tasks.
3. Proceed to the tasks on on the board and click on either Complete or Reopen and observe what happens.

### Expected Results
Afte clicking, the status should change. Either from complete to reopen or reopen to complete associated with a notification.

### Actual Result
The status stays the same and you will never know if the transition or change has happened or not.

### Severity
Critical (This is crtitical because the user has to know if the change has occured or not in real time)

### Priority
High

### Evidence

<img width="883" height="434" alt="bug 3" src="https://github.com/user-attachments/assets/0ddbea29-8103-40a9-a635-a28832365ec5" />



## TF003: No Routing is done in the Backend when reselecting another project
Description: On the taskflow application, after selecting another project, there is no routing in the backend and hence the it stays on the same page even though another project is clicked.

### Precondition
A project is already selected.

### Test Data
First Selected project = Website Redesign

### Test Environment
Application URL = https://scary-spider-67x59gr97xwcr77p-5173.app.github.dev/

Postman or Inspection Tool.

OS: Windows 11

### Reproduction Steps
1. Open the application URL in your search box.
2. Select a project (Website Redesign Project) and observe the associated tasks.
3. Open your inpection tool and switch to the network tab.
4. Click on another project and observe what will happen in the network tab

### Expected Results
After clicking on another project, the network tab should show the routing is done.

### Actual Result
The network tab stays the same. Nothing shows in there.

### Severity
Critical (This is crtitical because no routing shows so the user is still on the same page and the same tasks shows even though a different project is chosen.)

### Priority
High




