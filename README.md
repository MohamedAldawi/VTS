# Vacation Tracking System
- The Vacation Tracking System (VTS) is designed to empower individual employees by enabling them to efficiently manage their vacation time, sick leave, and personal time off, without requiring an in-depth understanding of company policies or local facility-specific leave regulations. This concept is introduced in the book [Object-Oriented Analysis and Design with Applications, Third Edition](https://www.oreilly.com/library/view/object-oriented-analysis-and/9780201895513/)
- I crafted the system's workflow and providing a comprehensive definition of its use cases, which included the creation of detailed Flow, State, and ERD diagrams.

# Index
- [System Overview](#System-Overview)
- [System Features](#System-Features)
- [Use Case Diagram](#Use-Case-Diagram)
- [Use Cases](#Use-Cases)
- [Time Management Use Case](#Time-Management-Use-Case)
- [Workflow - Main flow](#Workflow---Main-flow)

# System Overview  
  This system holds the promise of significant time and cost savings, primarily within the HR department. It essentially removes the manual, individual time request process and replaces it with a rule-based   validation system. HR personnel will retain their responsibilities for inputting and updating employee vacation data in the system, but they will no longer serve as intermediaries in the request and       
  validation process for each individual time request.

# System Features
1. A rule-based system for the validation and verification of leave time requests.
2. Grant access to requests from the previous calendar year and permit requests to be made up to a year and a half in advance.
3. Email notifications to request manager approval and inform employees of changes in request status.
4. Enable HR and system administration personnel to override actions restricted by rules, with logging of those overrides.
5. Empower managers to directly allocate personal leave time within system-defined limits.

# Use Case Diagram
<p align="center">
 <img src="../main/images/use_case_diagram.png" alt="use_case_diagram"/>
    <br>
    <em>Figure 1.1 Use Case Diagram </em>
</p>

# Use Cases
- **$\textcolor{red}{Time \ Management: This \ use \ case \ explains \ how \ employees \ can \ request \ and \ review \ their \ vacation \ time \ requests.}$**
-	**Request Approval:** This use case outlines how a manager handles vacation time requests from their subordinates.
-	**Grant Additional Time:** This use case describes how a manager can allocate extra leave time, such as comp time, to their subordinates.
-	**Modify Employee Records:** This use case details how an HR employee can make changes to an employee's information in the system. This includes setting leave time allowances and maximum manager-awarded time.
-	**Location Management:** This use case explains how an HR employee administers location records and their associated regulations.
-	**Leave Category Management:** This use case outlines how an HR employee oversees leave categories and their corresponding regulations.
-	**Override Leave Records:** This use case specifies how an HR employee has the authority to override rejections of leave time requests made by the system's rules.
-	**System Logs Backup:** This use case describes how the system administrator creates backups of the system's logs.

# Time Management Use Case
- **Description:** The employee intends to create a new request for vacation time.
- **Actor:** Employee
- **Preconditions:** The employee is authenticated and identified as an employee of the company with privileges to manage his or her own vacation time.
- **Postconditions:** Email notification is sent to manager while the request is created. 
- **Basic flow:**
    1.	The employee accesses the VTS through a link to the web portal.
    2.	The VTS retrieves the employee's vacation information for the past 6 months and up to 18 months in the future.
    3.	The employee selects a category with available vacation time.
    4.	The VTS guides the employee to specify the requested date(s) and hours using a visual calendar.
    5.	The employee provides additional details and submits the request.
    6.	If there are errors, the web page displays them for correction.
    7.	The employee can edit or cancel the request.
    8.	If the request is complete and valid, it is sent for manager approval, triggering an email to the manager.
    9.	The request enters a pending approval state.
    10.	The manager receives the email and accesses the VTS.
    11.	The manager may need to provide authentication credentials.
    12.	The manager reviews pending requests and approves or denies them individually.
    13.	The VTS prompts the manager to provide reasons for disapproval.
    14.	The employee is notified of the decision, and the manager can continue managing requests or exit the VTS.
 
# Workflow - Main flow
<p align="center">
 <img src="../main/images/use_case_activity.png" alt="workflow"/>
    <br>
    <em>Figure 1.2 Workflow </em>
</p>
