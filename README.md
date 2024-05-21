<h1>Add and manage users with Linux commands</h1>


<h2>Description</h2>
Use the useradd, usermod, userdel, and chown commands to manage user access in the Linux Bash shell.


<h2>Environments Used </h2>

- <b>Linux</b>
- <b>Bash Shell</b>

<h2>Scenario:</h2>

In this scenario, a new employee with the username researcher9 joins an organization. You have to add them to the system and continue to manage their access during their time with the organization.

Here’s how you’ll do this task: 

<b>First</b>, you’ll add a new employee to the system and then to their primary group. 

<b>Second</b>, you’ll make this employee the owner of a file related to a particular project. 

<b>Third</b>, you’ll add the new employee to a supplementary group. Finally, you’ll delete the employee from the system.


<h2>Tutorial walk-through:</h2>

<h3>Task 1. Add a new user</h3>

A new employee has joined the Research department. In this task, you must add them to the system. The username assigned to them is researcher9.

1. Write a command to add a user called researcher9 to the system.

<img src="https://i.imgur.com/sqIUi9B.png" height="80%" width="80%"/>
   
Next, you need to add the new user to the research_team group.

2. Use the usermod command and -g option to add researcher9 to the research_team group as their primary group.

<img src="https://i.imgur.com/bbE5hd6.png" height="80%" width="80%"/>


<h3>Task 2. Assign file ownership</h3>

The new employee, researcher9, will take responsibility for project_r. In this task, you must make them the owner of the project_r.txt file.

The project_r.txt file is located in the /home/researcher2/projects directory, and owned by the researcher2 user.

1. Use the chown command to make researcher9 the owner of /home/researcher2/projects/project_r.txt.

<img src="https://i.imgur.com/CO7UcTa.png" height="80%" width="80%"/>


<h3>Task 3. Add the user to a secondary group</h3>

A couple of months later, this employee's role at the organization has changed, and they are working in both the Research and the Sales departments.

In this task, you must add researcher9 to a secondary group (sales_team). Their primary group is still research_team.

1. Use the usermod command with the -a and -G options to add researcher9 to the sales_team group as a secondary group.

<img src="https://i.imgur.com/o8lcJHo.png" height="80%" width="80%"/>


<h3>Task 4. Delete a user</h3>

A year later, researcher9, decided to leave the company. In this task, you must remove them from the system.

1. Run a command to delete researcher9 from the system:

<img src="https://i.imgur.com/MaYWRmg.png" height="80%" width="80%"/>

This command will output the following message:
   
<img src="https://i.imgur.com/RWzgf8Y.png" height="80%" width="80%"/>

This is expected.

<img src="https://i.imgur.com/b81WtLN.png" height="80%" width="80%"/>

2. Run the following command to delete the researcher9 group that is no longer required:

<img src="https://i.imgur.com/pVTOx7U.png" height="80%" width="80%"/>



<h2>Conclusion</h2>

You now have practical experience in using basic Linux Bash shell commands to

- add a new user
- add a user to a group
- change user permissions on files
- delete a user

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
