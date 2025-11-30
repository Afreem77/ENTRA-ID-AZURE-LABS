
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

<img width="1511" height="822" alt="Screenshot 2025-11-29 185841" src="https://github.com/user-attachments/assets/cc0a9b00-ed9a-42b2-95ec-feefb26d5060" />





Screenshot the Create user form BEFORE clicking Review + create

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



Screenshot the New group form before clicking Create

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



