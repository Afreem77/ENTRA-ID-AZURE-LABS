
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


<img width="1517" height="887" alt="Screenshot 2025-11-29 185752" src="https://github.com/user-attachments/assets/354be15d-240f-401d-87fa-f58c5244409d" />



Entra Admin Home Dashboard showing:

Left navigation menu

Your tenant name at the top right

Step 2 — Navigate to Users

On the left menu, click Microsoft Entra ID

Click Users

Click All users


<img width="1511" height="822" alt="Screenshot 2025-11-29 185841" src="https://github.com/user-attachments/assets/dbd27554-9c59-4c6c-ae65-d4f747932842" />



“All users” page open, even if empty (show the table).

Step 3 — Create a New User

At the top → click + New user

Select Create new user

Fill in:

User principal name: test.user1@yourdomain.onmicrosoft.com

Display name: Test User 1

Leave password set to Auto-generate

Click Review + create

Click Create


<img width="1044" height="401" alt="Screenshot 2025-11-29 185932" src="https://github.com/user-attachments/assets/fa15b458-a22e-4951-862f-fe976c317392" />


Screenshot the Create user form BEFORE clicking Review + create

Step 4 — Confirm User Was Created

After creation, Azure will show the user profile page

Check:

Display name

User principal name

Object ID



<img width="1533" height="899" alt="Screenshot 2025-11-29 190536" src="https://github.com/user-attachments/assets/7f22b606-2344-4d5a-b466-3ba4d60b3ff7" />


User profile page with all fields visible

Step 5 — Create 2 More Users

Repeat Step 3 for:



User 2

Display name: HR Admin

UPN: hr.admin@yourdomain.onmicrosoft.com



User 3

Display name: IT Support

UPN: it.support@yourdomain.onmicrosoft.com



<img width="1533" height="859" alt="Screenshot 2025-11-29 190653" src="https://github.com/user-attachments/assets/5506dcba-c8ee-4dbb-92c9-abc7ee358f1d" />


All Users page showing all 3 users

Step 6 — Create a Security Group

On left menu, click Groups

Click + New group

Group type: Security

Group name: IT-Support-Team

Group description: Group for Level 1 technicians

Choose Assigned as Membership type

Click Create



<img width="1516" height="877" alt="Screenshot 2025-11-29 191014" src="https://github.com/user-attachments/assets/ff961d8f-b615-447e-a7ad-0be19050031c" />


Screenshot the New group form before clicking Create

Step 7 — Add Members to Group

After creating, click the group

Click Members

Click + Add members

Select:

IT Support

HR Admin (optional)

Click Select



<img width="1519" height="861" alt="Screenshot 2025-11-29 191131" src="https://github.com/user-attachments/assets/8546317d-b4e4-4790-9fa6-36d82d592308" />


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



