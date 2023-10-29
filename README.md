# Vacation Tracking System
- The Vacation Tracking System (VTS) is designed to empower individual employees by enabling them to efficiently manage their vacation time, sick leave, and personal time off, without requiring an in-depth understanding of company policies or local facility-specific leave regulations. This concept is introduced in the book [Object-Oriented Analysis and Design with Applications, Third Edition](https://www.oreilly.com/library/view/object-oriented-analysis-and/9780201895513/)
- I crafted the system's workflow and providing a comprehensive definition of its use cases, which included the creation of detailed Flow, State, and ERD diagrams.

# Index
- [System Overview](#System-Overview)
- [System Features](#System-Features)
- [Use Case Diagram](#Use-Case-Diagram)
- [Use Cases](#Use-Cases)

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
-	**Time Management:** This use case explains how employees can request and review their vacation time requests.
-	**Request Approval:** This use case outlines how a manager handles vacation time requests from their subordinates.
-	**Grant Additional Time:** This use case describes how a manager can allocate extra leave time, such as comp time, to their subordinates.
-	**Modify Employee Records:** This use case details how an HR employee can make changes to an employee's information in the system. This includes setting leave time allowances and maximum manager-awarded time.
-	**Location Management:** This use case explains how an HR employee administers location records and their associated regulations.
-	**Leave Category Management:** This use case outlines how an HR employee oversees leave categories and their corresponding regulations.
-	**Override Leave Records:** This use case specifies how an HR employee has the authority to override rejections of leave time requests made by the system's rules.
-	**System Logs Backup:** This use case describes how the system administrator creates backups of the system's logs.

```diff
- @@Time Management: This use case explains how employees can request and review their vacation time requests.@@

```
