
Microsoft Entra ID & Azure Labs

Welcome to my Microsoft Entra ID and Azure Labs repository! 🎉


This repository contains step-by-step, beginner-friendly labs and tutorials designed to help you learn and practice Microsoft Entra ID (Azure AD) and related Azure features in a hands-on environment. Each lab is carefully structured to guide you through real-world scenarios, with screenshots, instructions, and notes to make learning simple and practical.


What You’ll Find Here
Hands-on labs: Step-by-step exercises that cover key Entra ID and Azure concepts.
Screenshots & visual guides: Clear instructions with visuals to help you follow along.
Beginner-friendly instructions: Labs assume minimal prior experience, perfect for learners starting their journey in cloud identity and access management.
Best practices: Guidance on lab setup, configuration, and testing in a safe environment.


Example Lab Topics
Creating and organizing users in Microsoft Entra ID
Managing groups and roles
Basic Azure AD settings and security features
Assigning permissions without requiring paid licenses


Lab 1 — Creating & Organizing Users in Microsoft Entra ID (No License Required)


🔍 Objective


Create cloud-only users and security groups in Microsoft Entra ID to simulate a basic enterprise directory. Learn basic Entra ID navigation, user creation, and group management without needing a paid license.

🛠️ Skills Demonstrated
Azure Portal navigation
Entra ID cloud-only user creation
Security group management
Basic cloud identity administration


🔧 Step-by-Step Instructions
Step 1 — Sign In to Microsoft Entra ID

Go to: https://entra.microsoft.com

Sign in with your Microsoft account

You will land on the Microsoft Entra admin center

<img width="1517" height="887" alt="Screenshot 2025-11-29 185752" src="https://github.com/user-attachments/assets/9ac92328-a70e-40d6-98d5-e381fea82b81" />

Entra Admin Home Dashboard showing:

Left navigation menu

Your tenant name at the top right

Step 2 — Navigate to Users

On the left menu, click Microsoft Entra ID

Click Users

Click All users



Step 3 — Create a New User

At the top → click + New user

Select Create new user

Fill in:

User principal name: test.user1@yourdomain.onmicrosoft.com

Display name: Test User 1

Leave password set to Auto-generate

Click Review + create

Click Create

<img width="1511" height="822" alt="Screenshot 2025-11-29 185841" src="https://github.com/user-attachments/assets/cc0a9b00-ed9a-42b2-95ec-feefb26d5060" />

Step 4 — Confirm User Was Created

After creation, Azure will show the user profile page

Check:

Display name

User principal name

Object ID


<img width="1044" height="401" alt="Screenshot 2025-11-29 185932" src="https://github.com/user-attachments/assets/fd2be4ed-6b56-4713-842f-ca7f5a31457e" />



User profile page with all fields visible

Step 5 — Create 2 More Users

Repeat Step 3 for:



User 2

Display name: HR Admin

UPN: hr.admin@yourdomain.onmicrosoft.com

User 3

Display name: IT Support

UPN: it.support@yourdomain.onmicrosoft.com


<img width="1533" height="899" alt="Screenshot 2025-11-29 190536" src="https://github.com/user-attachments/assets/b7ca146a-bf91-4380-b6e2-cc4caa5249cd" />

All Users page showing all 3 users

Step 6 — Create a Security Group

On left menu, click Groups

Click + New group

Group type: Security

Group name: IT-Support-Team

Group description: Group for Level 1 technicians

Choose Assigned as Membership type

Click Create

<img width="1533" height="859" alt="Screenshot 2025-11-29 190653" src="https://github.com/user-attachments/assets/5d790037-29cf-4e56-bf0d-42c02fd04c92" />

Step 7 — Add Members to Group

After creating, click the group

Click Members

Click + Add members

Select:

IT Support

HR Admin (optional)

Click Select

<img width="1516" height="877" alt="Screenshot 2025-11-29 191014" src="https://github.com/user-attachments/assets/82608293-50aa-413d-91ec-cecb96bcfa1e" />

Group page showing the list of added members

Step 8 — Final Confirmation

Navigate to:

Groups → IT-Support-Team → Members

Verify the correct users are added


Entra Admin Center dashboard

All Users page (before user creation)

Create User form

User profile page

All Users page (after all 3 users created)

Create Group form

Group Members page showing added users

<img width="1519" height="861" alt="Screenshot 2025-11-29 191131" src="https://github.com/user-attachments/assets/379a435e-da90-404f-a53a-cb25d0d20bbe" />

📝 Concept Notes
Cloud-Only Users: Users created directly in Entra ID, not synchronized from on-premises AD

User Principal Name (UPN): Sign-in name formatted like an email address

Display Name: User-friendly name displayed in portal

Security Groups: Collections of users to manage access and permissions efficiently

Membership Types: Assigned (manual) vs Dynamic (rule-based)

Best Practice: Always validate user and group details after creation

✅ Validation Checklist
Entra Admin Center dashboard captured

Three cloud-only users created: Test User 1, HR Admin, IT Support

Security group IT-Support-Team created

Users added to the group correctly

All screenshots captured for GitHub portfolio



✅ 
LAB 2 — Assign Administrative Roles in Microsoft Entra ID (No License Required)
🎯 
Objective:
Assign least-privilege administrative roles to specific cloud users in Microsoft Entra ID and verify the assignments to demonstrate basic identity access management (IAM) capabilities.

🛠️ 
Step-by-Step Instructions
Step 1 — Sign In to Microsoft Entra Admin Center
Go to: https://entra.microsoft.com
Sign in
Click Microsoft Entra ID in the left menu

<img width="1525" height="880" alt="11-30" src="https://github.com/user-attachments/assets/3dd3b0ef-1713-4d24-8cca-2d2bcfc7c16f" />


Step 2 — Open Roles and Administrators
In the left menu → click Roles and administrators
View the list of built-in administrative roles

<img width="1527" height="869" alt="Screenshot 2025-11-30 141706" src="https://github.com/user-attachments/assets/c06c00d4-1ba1-499a-8545-76e48bf2bb8a" />


Step 3 — Open Password Administrator Role
Search or scroll to Password Administrator
Click it


<img width="1528" height="879" alt="Screenshot 2025-11-30 142648" src="https://github.com/user-attachments/assets/76df2edd-2999-465a-ae93-e687f39c460b" />


Step 4 — Assign the Role to HR Admin
Inside the role → click Add assignments
Search for → HR Admin
Select the user → click Add

<img width="1529" height="863" alt="Screenshot 2025-11-30 142735" src="https://github.com/user-attachments/assets/e97914eb-5f89-460e-8cce-b0161cb1a1aa" />




Step 5 — Confirm HR Admin Has the Role
Click the Assignments tab
HR Admin should appear


<img width="1520" height="872" alt="Screenshot 2025-11-30 142807" src="https://github.com/user-attachments/assets/95f91963-b579-4ec7-ac6c-84d89155f819" />



Step 6 — Assign Helpdesk Administrator to IT Support
Go back to Roles and administrators
Click Helpdesk Administrator
Click Add assignments
Select IT Support
Click Add

<img width="1519" height="868" alt="Screenshot 2025-11-30 142947" src="https://github.com/user-attachments/assets/b43a4127-c91a-4e51-a7c2-824abc7898ee" />


Step 7 — Verify Assigned Roles on Each User
Go to: Users → All Users
For HR Admin:
Click HR Admin
Click Assigned roles
Should show → Password Administrator
For IT Support:
Click IT Support
Click Assigned roles
Should show → Helpdesk Administrator

<img width="1533" height="869" alt="Screenshot 2025-11-30 143048" src="https://github.com/user-attachments/assets/1aea1ccb-7b95-47cc-aa11-4670a159078f" />

<img width="1533" height="871" alt="Screenshot 2025-11-30 143117" src="https://github.com/user-attachments/assets/7f65ca3c-df51-4371-8d25-8cece6e1c06c" />

📘 
Concept Notes (Important)
🔹 Role-Based Access Control (RBAC)
Allows organizations to assign specific permissions to users based on job needs.
🔹 Why Not Use Global Administrator?
It’s extremely powerful and risky. Cyber attackers target this role first.
🔹 Why “Least Privilege” Matters
Only give the permissions needed to complete a job.

This limits:
Accidental changes
Unauthorized access
Attack surface
Tenant compromise risk

🔹 Real-World Example
Helpdesk staff shouldn’t be able to create new admins.
HR should reset passwords but not manage apps or devices.

✔️ 
Validation Checklist (Must Complete All Items)

🔵 Portal Screenshots
Entra Overview screenshot
Roles & Administrators list

🟣 Role Screenshots
Password Administrator overview
HR Admin added to Password Administrator
Helpdesk Administrator overview
IT Support added to Helpdesk Administrator

🟢 User Verification Screenshots
HR Admin → Assigned roles shows Password Administrator
IT Support → Assigned roles shows Helpdesk Administrator





LAB 3 — Manage Security Groups & Add New Groups in Entra ID


🎯 
Objective
In this lab, you will:
Review and document an existing group (IT-Support-Team)
Create an additional new Security Group
Add users to both groups
Capture proper screenshots for your GitHub portfolio
(No licensing required.)

🛠️ 
Step-by-Step Lab Instructions
STEP 1 — Open Groups in Entra ID
Sign in to the Azure Portal
Search Microsoft Entra ID
Click Groups


All Groups page showing your group list including IT-Support-Team

STEP 2 — Document Your Existing Group (IT-Support-Team)
Click your IT-Support-Team group and capture:
A. Overview Tab
Shows: Group name, Group type, Object ID, Description

<img width="1526" height="862" alt="Screenshot 2025-11-30 150435" src="https://github.com/user-attachments/assets/f59e71e3-7346-4ba3-bc0d-dfc0096d34d9" />


Group → Overview tab
B. Members Tab
Shows who is in the group
Group → Members tab (even if empty)
C. Owners Tab
Shows if the group has an owner

<img width="1510" height="863" alt="Screenshot 2025-11-30 150652" src="https://github.com/user-attachments/assets/13c34d14-b7bf-4119-94de-7254641d2f40" />

Group → Owners tab

STEP 3 — Create a New Security Group
Group Name: HR-Restricted
Group Type: Security
Description: Restricted access group for HR data
Membership type: Assigned

Steps:
Go back to Groups
Click + New Group
Configure fields:
Group type: Security
Group name: HR-Restricted
Membership type: Assigned
Description: Restricted access group
Click Create

<img width="1529" height="863" alt="Screenshot 2025-11-30 150925" src="https://github.com/user-attachments/assets/f1bb386b-3695-476a-945b-8530e00a1c93" />


STEP 4 — Add Members to Both Groups
A. Add Users to IT-Support-Team
Open IT-Support-Team
Go to Members
Click + Add members
Add 1–3 users you created in Lab 1
Click Select

<img width="1517" height="857" alt="Screenshot 2025-11-30 151145" src="https://github.com/user-attachments/assets/dd6c73a0-c114-4725-a30e-9683bb87f9fd" />


“Members” page showing the added users
B. Add Members to HR-Restricted
Open HR-Restricted group
Go to Members
Click + Add Members
Select different users OR the same ones
Click Select

<img width="1518" height="857" alt="Screenshot 2025-11-30 204257" src="https://github.com/user-attachments/assets/6351386b-a00e-4d9f-ac14-b466365ab6c4" />


HR-Restricted → Members page
STEP 5 — Capture Final Documentation for Both Groups
For each group, screenshot:
Overview tab
Members tab
Owners tab (even if empty)



IT-Support-Team:
Groups list showing the group
Overview
Members
Owners
<img width="1525" height="859" alt="Screenshot 2025-11-30 151343" src="https://github.com/user-attachments/assets/54298c95-8ebc-4454-ad8d-53932cdf5b19" />

<img width="1524" height="860" alt="Screenshot 2025-11-30 151402" src="https://github.com/user-attachments/assets/666c4cee-c616-4456-8d20-37c9d7efe779" />

<img width="1314" height="738" alt="Screenshot 2025-11-30 151444" src="https://github.com/user-attachments/assets/c48dabc1-e9c1-411e-8dfa-a3f10bd453dc" />


HR-Restricted:
New group creation screen
Overview
Members
Owners
<img width="1526" height="923" alt="Screenshot 2025-11-30 151516" src="https://github.com/user-attachments/assets/35f80735-145d-4bf3-b656-61b7dd3e2a25" />

<img width="1526" height="868" alt="Screenshot 2025-11-30 151531" src="https://github.com/user-attachments/assets/17428128-f0c9-4dd0-9140-0ff1955c3620" />

<img width="1521" height="865" alt="Screenshot 2025-11-30 151547" src="https://github.com/user-attachments/assets/f6ecabf6-3226-4fae-b46c-8d4ba11a577f" />

📘 
Concept Notes (Place before checklist)


🔹 What Are Security Groups?
Security Groups manage user access across Microsoft 365 and Azure resources. Examples:
Assign Teams permissions
Grant access to SharePoint sites
Apply Conditional Access policies
Add users to app roles

🔹 Why Use Assigned Groups?
Assigned groups are manually controlled, easy to manage, and require no license.

🔹 Why Create Multiple Groups?
Good identity management separates users by roles:
IT group → technical access
HR group → sensitive data access

This demonstrates least privilege and role-based access control (RBAC)

✔️ 
Validation Checklist
You should have:
Existing group IT-Support-Team fully documented
New group HR-Restricted created
Both groups have at least 1 member

Screenshots of:
Groups list
Overview pages
Members pages
Owners pages
Clear naming + role separation explained




