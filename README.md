# osTicket Lifecycle Examples

Last section for the osTicket. Great work! In this tutorial, we're going to configure create a sample ticket, work on it, and finally complete said ticket to get a general idea on how powerful osTicket is for business enterprises.

<h3>Prologue</h3>
If your Virtual Machine is turned off, login to Azure, turn the VM back on, and login to Remote Desktop with your credentials.

Afterwards, we'll open up osTicket and continue where we left off.

But before we start creating tickets, there's some minor changes that needs to be taken care of first. 

So let's go to the Admin/Analyst Login Page and login with the osTicket admin credentials used in previous sections:
http://localhost/osTicket/scp/login.php 

From there, let's go into the Admin page itself by clicking on the "Admin Panel" located on the top right corner.

<img width="1217" height="463" alt="image" src="https://github.com/user-attachments/assets/c91dd5a5-6640-4906-a9a2-2bcd6cebdba9" />

Next, we'll highlight the Agents tab, and then click Departments as shown.

<img width="1216" height="317" alt="image" src="https://github.com/user-attachments/assets/b867c03a-a959-492c-af3b-a555c8825ee2" />

Once in the Departments page, click the checkbox beside the word "Maintenance", then click "More". A dropdown option will pop up and from there click "Delete" and then click "Yes, Do It!"

<img width="1216" height="509" alt="image" src="https://github.com/user-attachments/assets/0456413d-d5c2-40f9-b103-0e888c2de66a" />

<img width="620" height="266" alt="image" src="https://github.com/user-attachments/assets/36cd2326-d0fe-4a4c-914e-1ec9909942a8" />

The reason for the deletion is because created support tickets would've been auto-assigned to that particular department which is what we don't want due to the priority level that Maintenance had.


Upon deletion, click on "Support / SysAdmins"

<img width="1220" height="518" alt="image" src="https://github.com/user-attachments/assets/be087cd5-adf9-42e2-9cf0-0d99563e41a7" />

Once inside, set the Parent to "Top Level Department", scroll to the bottom of the page, and then click "Save Changes".

<img width="1169" height="486" alt="image" src="https://github.com/user-attachments/assets/407e78d9-1756-4c55-931b-51f36eed0478" />


Now we are fully ready to tackle tickets!


<h3>Create and Work</h3>

Login to osTicket at http://localhost/osTicket/ and create a new ticket as an end-user.

![image](https://github.com/user-attachments/assets/2c46d46e-8077-489a-a06e-e295555aa97c)

Use to same login info that we used to create Karen. From there, follow the screenshot below and then click "Create Ticket" for submission.

<img width="1037" height="928" alt="image" src="https://github.com/user-attachments/assets/06966c74-95e6-431c-9123-e1337459c5fa" />


Next, we're going to login as the Agent John using past credentials in order to see the ticket that was submitted to the system here.

http://localhost/osTicket/scp/login.php 

*Note, if the username for John doesn't work, you may have to use the fake email address associated with the admin.

As you can see, the ticket has been submitted for Admins and Agents to view. Let's click on the ticket itself in red.

<img width="1208" height="380" alt="image" src="https://github.com/user-attachments/assets/aa70dd46-396f-41eb-a71f-8b911e2fe4a9" />


Take a look at the various options we have. We can change the SLA priority level, ticket status, the due date, assign tickets to different teams, etc. so let's start making some edits.

1. First we'll tackle the priority level by changing the Default SLA to Sev-A inside the "SLA Plan" dropdown box and giving it a description, then click Update.

<img width="1202" height="550" alt="image" src="https://github.com/user-attachments/assets/3abe3a31-2e9c-4950-9a0f-e6e7bad1215b" />

<img width="836" height="345" alt="image" src="https://github.com/user-attachments/assets/9da5bf79-7068-4f1c-bc07-114a1cf52430" />

2. Change the Help Topic so that it's less generalized, this of course will vary depending on the organization. So click "Report a Problem" and then we going to change the Help Topic inside the dropdown box from "Report a Problem" to "Report a Problem / Business Critical Outage". Give it a description, and then click Update.

<img width="1210" height="406" alt="image" src="https://github.com/user-attachments/assets/16779fb3-477a-490f-a834-34f206d72336" />

<img width="803" height="311" alt="image" src="https://github.com/user-attachments/assets/ca75a4eb-b6aa-4fd5-85b3-41ae2d56959f" />

3. Let's assign the ticket to a team by clicking on "Unassigned" beside the "Assigned To" area. Click the dropdown box, and then click on "Online Banking" under the "Teams" section inside of the dropdown box. Give it a description, and then click "Assign".

<img width="1209" height="349" alt="image" src="https://github.com/user-attachments/assets/ebb77477-71fa-4677-9a56-c2f5ba9e4af6" />

<img width="796" height="338" alt="image" src="https://github.com/user-attachments/assets/7d6afd9a-a348-4935-9b9d-534fd3d0cce6" />

<img width="810" height="316" alt="image" src="https://github.com/user-attachments/assets/282529d3-9913-40de-b0f8-2041b288e9b8" />


Now, let's log out as John, and log in as Jane so we can assign the ticket just for her to specifically work on.

<img width="1206" height="465" alt="image" src="https://github.com/user-attachments/assets/6121bfa5-1526-48bd-902f-599a7d6daa71" />

Go inside the ticket, and click on "Online Banking" beside the "Assigned To" area. From there, click the dropdown box, click "Jane Doe", give a small description, and then click "Assign".

<img width="1210" height="401" alt="image" src="https://github.com/user-attachments/assets/6ec3d1f8-77fd-45b3-a6c0-6a57b1c2e2bd" />

<img width="1210" height="401" alt="image" src="https://github.com/user-attachments/assets/88fa58e8-ddbf-4a65-b0f0-c01c91b15d8e" />

<img width="810" height="376" alt="image" src="https://github.com/user-attachments/assets/209b3696-5f6f-4ed1-882f-085e19d896e4" />

<img width="816" height="362" alt="image" src="https://github.com/user-attachments/assets/63795c39-10f6-4ec4-894a-94de450c116d" />


<h3>Closing</h3>

We can also reply to Karen, or internally where only the Admin and Agents can see. Feel free to explore and when you're ready let's close the ticket, and then click "Post Reply"


![image](https://github.com/user-attachments/assets/e6852a51-77a4-40d3-92f9-c94ee02ee626)


Let's change the status of the ticket to "Resolved"


<img width="1220" height="353" alt="image" src="https://github.com/user-attachments/assets/c97715d2-4cdd-4346-b7d1-a6d3b6cf0ea1" />


![image](https://github.com/user-attachments/assets/7220e019-9afc-4fb6-a3d0-247a90369235)


Feel free to leave an optional note in the new window if you like and then click "Close".

As shown below, you can see the resolved ticket, and how many tickets have been resolved in a day, week, month, etc. as well

![image](https://github.com/user-attachments/assets/74e96f78-465e-413d-8fd8-1f72449e76bc)



*Creator note* - don't pay attention to the discrepancy of the dates / ticket numbers within the screenshots as there have been some minor changes that I had to do when I realized that I was logged in as the admin the whole time instead of an agent.


With that said, congratulations for making it to the very end of the osTicket guide! Feel free to play around with creating tickets, changing agent settings, and more. Ticketing System is vital for businesses big and small to ensure operations are in working order. By communicating with end users and prioritizing what can impact a business, you will have guaranteed success in this field!



Remember, do not forget to stop the VM!! 

![image](https://github.com/user-attachments/assets/92abfa3a-0dc5-4284-8fde-ab364f9f546d)
