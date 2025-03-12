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

## Access osTicket  

- **Admin/Analyst Login Page:** [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)  
- **End User Portal:** [http://localhost/osTicket](http://localhost/osTicket)  

---

## Ticket Lifecycle Stages  

### **Stage 1: Ticket Creation (Intake)**  
- **Scenario:** As an **end user**, submit a ticket using the osTicket web portal.  
- **Example Ticket:** *Entire mobile/online banking system is down.*  

![image](https://github.com/user-attachments/assets/edcc8a39-0103-4be3-a91b-3aa74130c0c6)

![image](https://github.com/user-attachments/assets/d3b5489e-8f31-4f1c-a1ed-e4057eec2113)


### **Stage 2: Ticket Assignment & Categorization**  
As a **Help Desk Agent (John)**:  
- Observe ticket properties:  
  - Priority  
  - Department 
  - SLA  
  - Assigned To
 
![image](https://github.com/user-attachments/assets/50d449ad-8c62-44e2-8676-6be9c493cc7e)


- Set ticket properties:  
  - **SLA Plan:** i.e. Sev-A (1 hour, 24/7)  
  - **Department:** i.e. Assign to "Online Banking Department"    

![image](https://github.com/user-attachments/assets/f8e206fa-28bf-4cee-9ce0-b816aa023e6c)

![image](https://github.com/user-attachments/assets/d74d36fa-c8a5-4d87-8cba-53b9e026b627)


### **Stage 3: Ticket Resolution**  
As **Help Desk Agent (Jane)** from the Online Banking Department:  
- Work the ticket to completion.

![image](https://github.com/user-attachments/assets/65dfea42-fce3-4672-8b65-836a4650d01a)

### **Stage 4: Finalizing & Ticket Closure**  
- Solve all remaining tickets.  
- Explain that most ticketing systems (including osTicket) **send email notifications** to users when updates are made.  
- Users can respond via email, and replies are logged in the ticket.

![image](https://github.com/user-attachments/assets/004b9bb3-fd42-482d-bbc4-ff5517104ea6)

---

## More Practice  
As an **End User**, create a new ticket:  
- **Issue:** *Accounting department needs Adobe upgrade, broken.*  
- As **Help Desk Agent (John)**: Observe the ticket’s properties and update:  
  - Priority: Sev-B (4 hours, 24/7)  
  - Department: Support    
- Work the ticket to completion as **John**.  

As an **End User**, create a third ticket:  
- **Issue:** *CFO’s laptop will no longer turn on.*  
- As **Help Desk Agent (John)**, set properties:  
  - Priority: Sev-B (4 hours, 24/7)  
  - Department: Support  
- Work the ticket to completion as **John**.  

---

## **Real-World Ticket Intake**  
- Tickets can be submitted in various ways:  
  - Phone calls, chat apps, emails, web forms, or in-person requests.  
- In IT support, people often ask for help **without submitting a ticket**.  
- It’s okay to fix things on the spot, but **always create tickets** for documentation and metrics tracking.  

---

## **Finishing Up & Additional Practice**  
- osTicket offers more features beyond this lab – explore them!  
- Experiment with the email functionality for ticket updates.  
- Repeat this lab multiple times until you can complete it from memory.  
- Building Technical Intuition:  
  - Repetition builds confidence.  
  - Understanding ticket management is crucial for IT help desk roles.  

---

### 🎉 Congratulations! You’ve completed the osTicket Ticket Lifecycle Lab! 🎉 
