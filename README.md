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

📸 *Screenshot: Admin/Analyst login page (`/scp/login.php`)*  
📸 *Screenshot: End User Portal home page (`/osTicket`)*


### 2. End User Creates Ticket #1 – Online/Mobile Banking Down

1. In the **End User Portal**, click **Open a New Ticket**.
2. Fill out a ticket such as:  
   - **Issue**: "Entire mobile/online banking system is down"
3. Submit the ticket.

📸 *Screenshot: New Ticket form filled out for mobile/online banking outage*  
📸 *Screenshot: Ticket confirmation page for Ticket #1*


### 3. Agent (john) Views Ticket #1 Properties

1. Log in (or switch) to **Agent Panel** as **john**.
2. Go to **Tickets** and open the ticket about the mobile/online banking outage.
3. Observe and note the ticket properties:
   - Priority  
   - Department  
   - SLA  
   - Assigned To  

📸 *Screenshot: Ticket #1 details as viewed by john (before changes)*


### 4. Agent (john) Sets Ticket #1 Properties

1. While viewing Ticket #1 as **john**:
   - Set **SLA** to **Sev-A (1 hour, 24/7)**.
   - Set **Department** to **Online Banking Department**.
2. Save or update the ticket.

📸 *Screenshot: Editing Ticket #1 to set SLA = Sev-A and Department = Online Banking*  
📸 *Screenshot: Updated Ticket #1 properties after saving*


### 5. Attempt to View Ticket #1 Again as john

1. As **john**, navigate back to the **Tickets** list.
2. Try to view Ticket #1 again.
3. Observe whether john can:
   - Still see the ticket.
   - Still change its properties or if access is restricted.

📸 *Screenshot: Tickets list from john’s perspective*  
📸 *Screenshot: Any error or restricted view for Ticket #1 as john (if applicable)*


### 6. Work Ticket #1 to Completion as jane

1. Log in or switch to **Agent Panel** as **jane** (or the admin with full access).
2. Open Ticket #1.
3. Add replies/work notes as needed.
4. Change the ticket status to **Resolved/Closed** (or equivalent).
5. Save the ticket.

📸 *Screenshot: Ticket #1 being worked on by jane*  
📸 *Screenshot: Ticket #1 in a completed/closed state*


### 7. End User Creates Ticket #2 – Adobe Upgrade/Broken

1. In the **End User Portal**, create another ticket:
   - **Issue**: "Accounting department needs Adobe upgrade, broken"
2. Submit the ticket.

📸 *Screenshot: New Ticket form for Adobe upgrade issue (Ticket #2)*  
📸 *Screenshot: Ticket #2 confirmation page*


### 8. Agent (john) Sets Ticket #2 Properties & Completes

1. As **john**, go to **Tickets** and open Ticket #2.
2. Observe its initial properties:
   - Priority  
   - Department  
   - SLA  
   - Assigned To  
3. Update Ticket #2:
   - **SLA**: Set to **Sev-B (4 hours, 24/7)**.
   - **Department**: Set to **Support**.
4. Work the ticket to completion:
   - Add responses/notes.
   - Mark the ticket **Resolved/Closed**.

📸 *Screenshot: Ticket #2 before property changes*  
📸 *Screenshot: Ticket #2 after setting SLA/Department*  
📸 *Screenshot: Ticket #2 in completed/closed state*


### 9. End User Creates Ticket #3 – CFO Laptop Won’t Turn On

1. In the **End User Portal**, create a third ticket:
   - **Issue**: "CFO’s laptop will no longer turn on"
2. Submit the ticket.

📸 *Screenshot: New Ticket form for CFO laptop issue (Ticket #3)*  
📸 *Screenshot: Ticket #3 confirmation page*


### 10. Agent (john) Sets Ticket #3 Properties & Completes

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

📸 *Screenshot: Ticket #3 before changes*  
📸 *Screenshot: Ticket #3 after setting SLA/Department*  
📸 *Screenshot: Ticket #3 in a completed/closed state*


### 11. Escalate Tickets – Apply Sev-A (SysAdmins Last)

1. For all existing tickets, adjust properties so they are escalated to **Sev-A** where required.
2. Specifically, set the ticket associated with **SysAdmins** to **Sev-A (1 hour, 24/7)** **last**.
3. Observe how changing SLA or department to SysAdmins affects visibility or accessibility (for example, john may lose access if he does not have rights to SysAdmins).

📸 *Screenshot: List of tickets while updating SLAs (Sev-A/Sev-B)*  
📸 *Screenshot: Ticket associated with SysAdmins after escalation*  
📸 *Screenshot: Inaccessible ticket view or error for john (if applicable)*


### 12. Regain Access by Granting View Rights to SysAdmins

1. Log in as an admin with configuration access (e.g., **jane**).
2. Go to the **Admin Panel → Agents → Departments → SysAdmins**.
3. Adjust permissions to grant yourself (or the relevant agent) **view access** to the **SysAdmins** department.
4. Save changes.

📸 *Screenshot: SysAdmins department permissions configuration*  
📸 *Screenshot: Agent/role assignment showing View access for SysAdmins*


### 13. Observe the Escalated Ticket Again as Agent

1. Switch back to the **Agent Panel** as the agent who now has SysAdmins view access.
2. Locate and open the previously escalated ticket.
3. Observe that:
   - You can now **see** the ticket.
   - In many cases, escalated tickets might be **restricted from further changes** (read-only / limited edits depending on configuration).

📸 *Screenshot: Escalated ticket now visible to agent*  
📸 *Screenshot: Ticket showing limited or read-only controls (if applicable)*


### 14. Solve All Remaining Tickets

1. For all open tickets:
   - Ensure appropriate SLA, Department, and Assignment are set.
   - Add final notes or resolution comments.
   - Set tickets to **Resolved/Closed** status.
2. Confirm there are no unresolved tickets left.

📸 *Screenshot: Ticket list showing all tickets in a resolved/closed state*


### 15. Note on Email Notifications (Ticket Updates)

> In most ticketing systems (including osTicket if configured with email), each ticket update can send an **email notification** to the end user. Users can reply to that email and their response is added to the ticket automatically.

📸 *Screenshot (optional): Email settings section in Admin Panel (if configured)*


### 16. Real-World Ticket Intake (Conceptual Step)

> In real environments, tickets may be created via:
> - Phone calls  
> - Chat apps  
> - Email  
> - Web forms  
> - In-person requests  
>
> Even if you fix something on the spot, it is best practice to **create tickets for everything you do** for tracking and metrics.

(You can optionally add notes or diagrams here instead of screenshots.)


### 17. Practice & Repetition

> To build confidence and technical intuition:
> - Repeat this lab several times.
> - Practice creating, modifying, escalating, and resolving tickets.
> - Experiment with different SLAs, departments, and permissions.

📸 *Screenshot (optional): Re-doing the lab or summary view of multiple test tickets*
