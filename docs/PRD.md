# Project Requirements Document (PRD)

## Tamil Brahmin Community Family Tree Web Application

---

# 1. Project Overview

## Project Name

**Tamil Brahmin Family Tree Portal**

## Project Objective

The objective of this application is to build a secure, private, community-only family tree platform for Tamil Brahmin families. The platform will allow members to voluntarily register their details, create interconnected family trees, and preserve lineage information digitally.

The system must support:

* Thousands of members
* Admin-controlled approvals
* Editable family records
* Multi-generation family tree visualization
* Community lineage verification
* Collaborative family updates with approval workflow

The application should be mobile-friendly, simple for elderly users, and scalable for long-term community use.

---

# 2. User Roles

## 2.1 Admin Role

Admins will have complete control over:

* Member approvals
* Family tree approvals
* Edit approvals
* Colour tagging of members
* Data corrections
* Duplicate handling
* Family tree moderation
* Viewing all submissions and changes

---

## 2.2 Member Role

Approved members can:

* Register and login
* Submit/edit profile details
* View all approved family trees
* Suggest edits to any family member
* Submit relationship corrections
* Upload photographs
* Search family trees

However:

* No changes become live immediately
* Every new entry or modification requires Admin approval

---

# 3. Registration Requirements

# IMPORTANT RULE

## ALL QUESTIONS ARE OPTIONAL

The system must NOT force users to fill any field.

Every field in registration must remain optional.

Members should be able to:

* Submit partial information
* Save incomplete information
* Return later and edit/update details BEFORE approval

---

# 4. Registration Form Fields

The registration form shall contain the following optional fields:

| Field No | Field Name                                      |
| -------- | ----------------------------------------------- |
| 1        | Full Name                                       |
| 2        | Nick Name                                       |
| 3        | Mobile Number                                   |
| 4        | Email Address                                   |
| 5        | Present Address                                 |
| 6        | Native Place                                    |
| 7        | Year of Birth (Only Year, NOT full DOB)         |
| 8        | Father's Name                                   |
| 9        | Mother's Name                                   |
| 10       | Is Father a Tamil Brahmin? (Yes/No)             |
| 11       | If No, Please Mention Father's Community        |
| 12       | Is Mother a Tamil Brahmin? (Yes/No)             |
| 13       | If No, Please Mention Mother's Community        |
| 14       | Whether Married? (Yes/No)                       |
| 15       | If Married, Is Spouse a Tamil Brahmin? (Yes/No) |
| 16       | If No, Please Mention Spouse Community          |
| 17       | Your Gothram                                    |
| 18       | Gothram of Spouse Before Marriage               |
| 19       | Upload Photo of Self                            |
| 20       | Any Other Remarks                               |

---

# 5. Registration Workflow

## Step 1 — Member Registration

User creates account using:

* Mobile number OR email
* Password/OTP authentication

---

## Step 2 — Optional Data Entry

User fills any number of optional fields.

No mandatory validation except:

* Basic format validation for email/mobile if entered

---

## Step 3 — Draft Save Capability

Before admin approval:

* User can revisit profile
* Edit data
* Resubmit information
* Upload/change photo
* Add/remove details

Status shown as:

* Draft
* Pending Approval

---

## Step 4 — Admin Review

Admin reviews:

* Authenticity
* Duplicate possibility
* Community relevance
* Family linkage possibility

Admin actions:

* Approve
* Reject
* Request clarification

---

## Step 5 — Family Tree Generation

After approval:

* Member becomes publicly visible to all approved members
* System generates family tree node
* Unique Family Tree Code is assigned

---

# 6. Unique Member Code System

Each approved member shall receive:

## Unique Family Tree ID

Example:

* TB000001
* TB000002

Rules:

* Auto-generated
* Permanent
* Unique
* Searchable

This code should appear:

* In profile
* In family tree
* In admin dashboard
* In search results

---

# 7. Family Tree Requirements

# 7.1 Automatic Tree Creation

After approval:

* Member node gets created automatically

The tree should support:

* Father linkage
* Mother linkage
* Spouse linkage
* Children linkage
* Multi-generation expansion

---

# 7.2 Visible Information in Tree

The family tree node should display:

* Name
* Year of Birth
* Native Place
* Gothram
* Profile Photo (optional)

No sensitive data like:

* Mobile number
* Address
* Email

should appear publicly unless allowed by admin settings.

---

# 7.3 Tree Visualization

The tree should support:

* Expand/collapse
* Zoom in/out
* Mobile touch support
* Horizontal & vertical layout
* Large family structures

---

# 8. Colour Coding System

Admins should be able to assign different colours to specific members or nodes in the family tree.

Purpose:

* Identify lineage categories
* Identify verified branches
* Mark special family status
* Distinguish submitted data conditions

Examples:

* Green → Verified lineage
* Yellow → Pending clarification
* Blue → Special branch
* Red → Review required

Requirements:

* Admin-configurable
* Colour visible in tree nodes
* Multiple colour options

---

# 9. Edit & Approval Workflow

# CRITICAL REQUIREMENT

## NO DIRECT LIVE EDITS

After approval:

* No member can directly modify live family tree data

---

# 9.1 Edit Request System

Any approved member can:

* Suggest edits
* Add relationships
* Correct names
* Upload additional data
* Suggest lineage changes

---

# 9.2 Pending Approval Queue

Every edit request must enter:

* Admin Review Queue

Only after admin approval:

* Changes become visible live

---

# 9.3 Change Tracking

System must store:

* Old value
* New value
* Submitted by
* Date/time
* Approval status
* Admin remarks

---

# 10. Member Contribution System

Any approved member should be allowed to:

* Suggest corrections for any family member
* Add missing relationships
* Suggest parent-child connections
* Add missing spouse information
* Upload historical details

But:

* Nothing becomes public without admin approval

---

# 11. Admin Dashboard Requirements

## Dashboard Features

Admins should be able to:

### Member Management

* Approve/reject registrations
* Suspend members
* Edit profiles
* Merge duplicate members

---

### Approval Queue

* Pending registrations
* Pending edits
* Pending relationship requests
* Pending photo approvals

---

### Family Tree Controls

* Manual linkage correction
* Colour assignment
* Relationship approval
* Tree restructuring

---

### Search & Filters

Search by:

* Name
* Native place
* Gothram
* Member code
* Family branch

---

# 12. Search Requirements

Approved members can search by:

* Name
* Nick name
* Native place
* Gothram
* Family code
* Father name
* Mother name

---

# 13. Privacy Requirements

## Public Visibility Rules

Only approved members can view family trees.

Guest/public users should NOT access:

* Trees
* Member data
* Search

---

## Hidden Data

The following should NOT be publicly visible:

* Mobile number
* Email
* Address
* Remarks
* Pending submissions

Unless specifically permitted by admin policy.

---

# 14. Technical Requirements

## Frontend

* Mobile-first responsive design
* Simple UI for elderly users
* Large fonts/buttons

Suggested:

* React.js
* Tailwind CSS

---

## Backend

Suggested:

* Node.js + Express

OR

* Firebase backend

---

## Database

Suggested:

* PostgreSQL

OR

* MongoDB

---

## Authentication

* OTP login
  OR
* Email/password login

---

# 15. Database Structure (High Level)

## Main Tables

### Users

Stores:

* Account details
* Login credentials
* Approval status

---

### MemberProfiles

Stores:

* Personal details
* Gothram
* Native place
* Community information

---

### FamilyRelationships

Stores:

* Parent-child links
* Spouse links
* Relationship mapping

---

### PendingChanges

Stores:

* Requested edits
* Approval status
* Audit trail

---

### AdminActions

Stores:

* Admin approvals
* Rejections
* Colour assignments

---

# 16. Audit & Security Requirements

System must log:

* Registrations
* Edits
* Approval actions
* Relationship changes
* Login activity

Security requirements:

* HTTPS only
* Encrypted passwords
* Role-based access
* Protection against unauthorized edits

---

# 17. Scalability Requirements

The application should support:

* Thousands of members
* Large interconnected trees
* High mobile usage
* Future Android app integration

---

# 18. Future Enhancements (Phase 2)

Potential future modules:

* Matrimony integration
* Community events
* Temple mapping
* Heritage records
* Family photo archives
* AI duplicate detection
* Elder verification system

---

# 19. MVP (Minimum Viable Product)

## Version 1 Must Include

### Member Features

* Registration/login
* Optional profile form
* Family tree generation
* Edit request submission
* Search

---

### Admin Features

* Approval system
* Edit moderation
* Colour coding
* Tree management

---

### Technical Features

* Mobile responsive UI
* Secure authentication
* Unique member codes
* Audit logging

---

# 20. Final Core Principles

The system must prioritize:

1. Community privacy
2. Admin-controlled accuracy
3. Easy contribution from members
4. Historical lineage preservation
5. Non-destructive edit workflow
6. Mobile-first usability
7. Scalability for future generations
