<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

## Tickets and Ticket Lifecycle – Step-by-Step Guide



### 1. Log In to osTicket (Admin/Analyst & End User)

1. Open the **Admin/Analyst login page**:  
   `http://localhost/osTicket/scp/login.php`
2. Log in as an admin/agent (e.g., **jane** or another admin).
3. Open a separate browser tab/window and go to the **End User Portal**:  
   `http://localhost/osTicket`

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/93181b20-d4da-45a6-9c6b-e0a694ee9fa1" />

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/b23745a3-d41c-449f-a676-99f36fb9af85" />



### 2. End User Creates Ticket #1 – Online/Mobile Banking Down

1. In the **End User Portal**, click **Open a New Ticket**.
2. Fill out a ticket such as:  
   - **Issue**: "Entire mobile/online banking system is down"
3. Submit the ticket.

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/5b25d2de-f155-490b-91f1-5a9a9378a130" />


### 3. Agent (john) Views Ticket #1 Properties

1. Log in (or switch) to **Agent Panel**.
2. Go to **Tickets** and open the ticket about the mobile/online banking outage.
3. Observe and note the ticket properties:
   - Priority  
   - Department  
   - SLA  
   - Assigned To  

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/abfde9c8-fdf0-432b-b974-7f27b3759ae0" />



### 4. Agent (john) Sets Ticket #1 Properties

1. While viewing Ticket #1 as **john**:
   - Set **SLA** to **Sev-A (1 hour, 24/7)**.
   - Set **Department** to **Online Banking Department**.
2. Save or update the ticket.

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/f8b31786-f5a3-4286-b6a3-bf725ded2dfa" />


### 5. Work Ticket #1 to Completion as jane

1. Log in or switch to **Agent Panel** as **jane** (or the admin with full access).
2. Open Ticket #1.
3. Add replies/work notes as needed.
4. Change the ticket status to **Resolved/Closed** (or equivalent).
5. Save the ticket.

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/eb49ad3d-817c-4153-818a-fc62a4a5ae48" />
<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/8ab7136c-1481-4b4f-8cb1-b78d89534a76" />




### 6. End User Creates Ticket #2 – Adobe Upgrade/Broken

1. In the **End User Portal**, create another ticket:
   - **Issue**: "Accounting department needs Adobe upgrade, broken"
2. Submit the ticket.

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/efaa8bfe-727a-4af7-88e5-5cfd52bd133e" />

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/9ddd2816-ac1a-48a0-8508-31f9de470b7a" />



### 7. Agent (john) Sets Ticket #2 Properties & Completes

1. As **john**, go to **Tickets** and open Ticket #2.
2. Observe its initial properties:
   - Priority  
   - Department  
   - SLA  
   - Assigned To  
3. Update Ticket #2:
   - **SLA**: Set to **Sev-C (8 hours, Business Hours)**.
   - **Assigned To**: Set to **John Doe**.
4. Work the ticket to completion:
   - Add responses/notes.
   - Mark the ticket **Resolved/Closed**.

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/c10da986-5f45-45a1-8a8c-d33b41bd5f08" />

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/fdbe3939-3b90-415b-93e3-64b056ecc305" />

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/cb474e9e-8f19-4634-a23a-389ad0075b4a" />



### 8. End User Creates Ticket #3 – CFO Laptop Won’t Turn On

1. In the **End User Portal**, create a third ticket:
   - **Issue**: "CFO’s laptop will no longer turn on"
2. Submit the ticket.

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/03fd231c-25f3-464b-afb4-56fe5949e2cf" />

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/07e918eb-2a09-4aaf-b511-cda082d53396" />



### 9. Agent (john) Sets Ticket #3 Properties & Completes

1. As **john**, go to **Tickets** and open Ticket #3.
2. Observe its properties:
   - Priority  
   - Department  
   - SLA  
   - Assigned To  
3. Update Ticket #3:
   - **SLA**: Set to **Sev-B (4 hours, 24/7)**.
   - **Department**: **Support**.
4. Work Ticket #3 to completion:
   - Add responses.
   - Mark as **Resolved/Closed**.

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/3224b616-13c6-4939-b496-515afd51517c" />

<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/99678cba-48b0-4e7e-97ca-e63f7cbcbf3c" />
 
<img width="1792" height="1120" alt="image" src="https://github.com/user-attachments/assets/ba240345-af38-4fca-a295-71e4d33a20b8" />



### 10. Note on Email Notifications (Ticket Updates)

> In most ticketing systems (including osTicket if configured with email), each ticket update can send an **email notification** to the end user. Users can reply to that email and their response is added to the ticket automatically.



### 11. Real-World Ticket Intake (Conceptual Step)

> In real environments, tickets may be created via:
> - Phone calls  
> - Chat apps  
> - Email  
> - Web forms  
> - In-person requests  
>
> Even if you fix something on the spot, it is best practice to **create tickets for everything you do** for tracking and metrics.



### 12. Practice & Repetition

> To build confidence and technical intuition:
> - Practice creating, modifying, escalating, and resolving tickets.
> - Experiment with different SLAs, departments, and permissions.


