<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket Ticket Lifecycle: From Intake to Resolution  

This tutorial outlines the **lifecycle of a help desk ticket** within the open-source ticketing system **osTicket**. It covers ticket creation, assignment, resolution, and escalation while demonstrating real-world help desk operations.  

---

## Environments & Technologies Used  
- **osTicket** – Open-source help desk ticketing system  
- **IIS Web Server** – Hosts the osTicket application  
- **PHP** – Required for osTicket functionality  
- **MySQL** – Database management system for ticket storage  
- **HeidiSQL** – Database administration tool  

## Operating Systems Used  
- **Windows 10** (or Windows Server for production environments)  

---

## Ticket Lifecycle Stages  

### 1. Access osTicket  
- **Admin/Analyst Login Page:** [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)  
- **End User Portal:** [http://localhost/osTicket](http://localhost/osTicket)  

---

## Lifecycle Stages  

### **Stage 1: Ticket Creation (Intake)**  
- **Scenario:** The **end user** submits a ticket using the osTicket web portal.  
- **Example Ticket:** *Entire mobile/online banking system is down.*  

### **Stage 2: Ticket Assignment & Categorization**  
As a **Help Desk Agent (John)**:  
- Observe ticket properties:  
  - **Priority:** Unassigned  
  - **Department:** Unassigned  
  - **SLA:** Unassigned  
  - **Assigned To:** Unassigned  
- Set ticket properties:  
  - **Priority:** **Sev-A (1 hour, 24/7)**  
  - **Department:** **Online Banking Department**  
- Attempt to re-observe the ticket as "John" – Can you still view or change it?  

### **Stage 3: Ticket Resolution**  
As **Help Desk Agent (Jane)**:  
- Work the ticket to completion.  

### **Stage 4: Another Ticket Submission**  
As an **End User**, create a new ticket:  
- **Issue:** *Accounting department needs Adobe upgrade, broken.*  
- As **Help Desk Agent (John)**: Observe the ticket’s properties and update:  
  - **Priority:** **Sev-B (4 hours, 24/7)**  
  - **Department:** **Support**  
  - **Modify Department Hierarchy:**  
    - Change **SysAdmins** to a **Top-Level Department**  
    - **DELETE** the **Maintenance Department** (not archive)  
- Work the ticket to completion as **John**.  

### **Stage 5: Ticket Escalation**  
As an **End User**, create a third ticket:  
- **Issue:** *CFO’s laptop will no longer turn on.*  
- As **Help Desk Agent (John)**, set properties:  
  - **Priority:** **Sev-B (4 hours, 24/7)**  
  - **Department:** **Support**  
- Work the ticket to completion as **John**.  

### **Stage 6: Permission Restrictions**  
- Set **Sev-A** priority for the **SysAdmins Department** on a ticket.  
- Observe that **John** can no longer access the ticket.  
- As **Admin**, switch to the **Admin Panel** and assign yourself **View-access** to SysAdmins.  
- Switch back to **Agent Panel** – now observe the **escalated ticket**.  
- Notice that you can **view the ticket but no longer make changes**.  

### **Stage 7: Finalizing & Ticket Closure**  
- Solve all remaining tickets.  
- Explain that most ticketing systems (including osTicket) **send email notifications** to users when updates are made.  
- Users can respond via email, and replies are logged in the ticket.  

---

## **Real-World Ticket Intake**  
- Tickets can be submitted in various ways:  
  - **Phone calls, chat apps, emails, web forms, or in-person requests.**  
- In IT support, people often ask for help **without submitting a ticket**.  
- It’s okay to fix things on the spot, but **always create tickets** for documentation and metrics tracking.  

---

## **Finishing Up & Additional Practice**  
- **osTicket offers more features** beyond this lab – explore them!  
- **Experiment with the email functionality** for ticket updates.  
- **Repeat this lab multiple times** until you can complete it from memory.  
- **Building Technical Intuition:**  
  - **Repetition builds confidence.**  
  - **Understanding ticket management** is crucial for IT help desk roles.  

---

### 🎉 **Congratulations! You’ve completed the osTicket Ticket Lifecycle Lab!** 🎉 

