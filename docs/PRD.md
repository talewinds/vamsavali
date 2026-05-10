# Project Requirements Document (PRD)

# Tamil Brahmin Community Family Tree Web Application

---

# 1. Project Overview

## Project Name

**Tamil Brahmin Family Tree Portal**

---

## Project Objective

The objective of this application is to build a secure, private, community-only genealogy and family tree platform for Tamil Brahmin families.

The platform will:

* Preserve lineage and heritage digitally
* Build a unified interconnected community genealogy network
* Allow members to voluntarily contribute family information
* Enable collaborative family tree building
* Support admin-controlled verification and approvals
* Prevent duplicate or disconnected family trees

The application must support:

* Thousands of members
* Multi-generation interconnected families
* Intelligent relationship matching
* Secure approval workflows
* Non-destructive editing
* Mobile-first usability

The system must be simple enough for elderly users and scalable for future generations.

---

# 2. Core System Philosophy

# IMPORTANT ARCHITECTURAL PRINCIPLE

The application shall NOT create isolated individual family trees.

Instead, the application shall maintain:

# ONE UNIFIED COMMUNITY GENEALOGY GRAPH

Each approved member becomes:

* A person/node inside the global community genealogy network

Family relationships connect nodes together dynamically.

This architecture ensures:

* No disconnected duplicate trees
* Better relationship matching
* Easier family merging
* Shared ancestry support
* Long-term scalability

---

# 3. User Roles

---

# 3.1 Admin Role

Admins shall have full authority over:

* Member approvals
* Family linkage approvals
* Duplicate handling
* Family merge approvals
* Edit approvals
* Colour coding
* Relationship restructuring
* Profile corrections
* Tree moderation
* Viewing audit history

Admins shall have the ability to:

* Merge duplicate profiles
* Link disconnected branches
* Approve/reject all changes
* Review intelligent family match suggestions

---

# 3.2 Member Role

Approved members shall be able to:

* Register and login
* Submit/edit personal details
* View approved community family trees
* Suggest edits
* Suggest relationships
* Upload photos
* Search family members
* Suggest missing lineage connections

However:

* No changes shall go live immediately
* Every addition/edit requires admin approval

---

# 4. Registration Requirements

# IMPORTANT RULE

## ALL REGISTRATION QUESTIONS ARE OPTIONAL

The system must NOT force users to fill any field.

Every field in the registration form must remain optional.

Users shall be allowed to:

* Submit partial information
* Save incomplete drafts
* Revisit profile before approval
* Edit/update details before approval

Only minimal validation is required for:

* Mobile number format
* Email format

if entered.

---

# 5. Registration Form Fields

The registration form shall contain the following optional fields:

| No | Field                                           |
| -- | ----------------------------------------------- |
| 1  | Full Name                                       |
| 2  | Nick Name                                       |
| 3  | Mobile Number                                   |
| 4  | Email Address                                   |
| 5  | Present Address                                 |
| 6  | Native Place                                    |
| 7  | Year of Birth (Only Year, NOT Date of Birth)    |
| 8  | Father's Name                                   |
| 9  | Mother's Name                                   |
| 10 | Is Father a Tamil Brahmin? (Yes/No)             |
| 11 | If No, Mention Father's Community               |
| 12 | Is Mother a Tamil Brahmin? (Yes/No)             |
| 13 | If No, Mention Mother's Community               |
| 14 | Whether Married? (Yes/No)                       |
| 15 | If Married, Is Spouse a Tamil Brahmin? (Yes/No) |
| 16 | If No, Mention Spouse Community                 |
| 17 | Your Gothram                                    |
| 18 | Gothram of Spouse Before Marriage               |
| 19 | Upload Photo of Self                            |
| 20 | Any Other Remarks                               |

---

# 6. Registration Workflow

---

# Step 1 — User Registration

User creates account using:

* Mobile number OR email
* Password OR OTP authentication

---

# Step 2 — Optional Data Submission

User may fill:

* Any number of fields
* Partial information
* Draft details

No field is compulsory.

---

# Step 3 — Draft Editing Before Approval

Before approval:

* User can revisit profile
* Edit details
* Add/remove information
* Change uploaded photo
* Save drafts multiple times

Possible statuses:

* Draft
* Pending Approval

---

# Step 4 — Admin Review

Admin reviews:

* Authenticity
* Duplicate possibility
* Community relevance
* Family linkage possibilities

Admin actions:

* Approve
* Reject
* Request clarification
* Request additional details

---

# Step 5 — Member Approval

After approval:

* Member becomes visible to approved community members
* Member becomes part of community genealogy graph
* Unique Family Tree Code is generated

---

# 7. Unique Family Tree Member Code System

Every approved member shall receive a:

# Unique Family Tree Member Code

Example:

* TB000001
* TB000002
* TB000003

---

# Rules

The code must be:

* Auto-generated
* Unique
* Permanent
* Searchable
* Never reused
* Assigned only after approval

---

# Purpose of Unique Code

The code shall help:

* Identify members uniquely
* Avoid duplicate confusion
* Track genealogy relationships
* Simplify admin approvals
* Enable family branch tracking

---

# Code Visibility

The code should appear in:

* Member profile
* Family tree node
* Search results
* Admin dashboard
* Relationship suggestions

---

# IMPORTANT

Even though all members belong to the unified genealogy graph, EACH approved member must still have an independent unique member code.

The code identifies:

* The person/member
  NOT
* A separate isolated family tree.

---

# 8. Intelligent Family Linkage & Merge System

The system shall intelligently search for existing family relationships whenever a new member is approved.

The objective is to:

* Avoid duplicate disconnected family trees
* Connect related family branches
* Build one unified genealogy network

---

# 8.1 Relationship Matching Engine

The system should search using:

* Father name
* Mother name
* Gothram
* Native place
* Spouse details
* Year of birth
* Existing relationships
* Nick names
* Family branch similarities

---

# 8.2 Suggested Relationship Detection

The system may generate suggestions such as:

* Possible brother match
* Possible uncle relationship
* Possible cousin linkage
* Possible duplicate member
* Possible shared ancestor

---

# 8.3 Relationship Confidence Score

The system should assign confidence scores.

Example:

| Match Type             | Confidence |
| ---------------------- | ---------- |
| Same father + gothram  | 95%        |
| Same native place only | 40%        |
| Same spouse lineage    | 75%        |

---

# 8.4 Admin Approval Required

NO automatic merge shall happen.

All relationship merges require:

* Admin review
* Admin approval

Admin may:

* Approve linkage
* Reject linkage
* Keep separate temporarily
* Merge duplicate profiles
* Restructure relationships manually

---

# 8.5 Non-Destructive Merge Rules

The system must NEVER permanently delete genealogy records.

Instead:

* Duplicate records may be archived
* Merge history must be preserved
* Original submissions must remain traceable

---

# 9. Family Tree Requirements

---

# 9.1 Unified Community Tree

The platform shall maintain:

* One interconnected community genealogy graph

Each member becomes:

* A node/person within the network

Relationships may include:

* Father
* Mother
* Son
* Daughter
* Husband
* Wife
* Sibling
* Uncle
* Aunt
* Cousin
* Ancestor branches

---

# 9.2 Family Tree Node Display

Each visible family tree node shall display:

* Full name
* Year of birth
* Native place
* Gothram
* Profile photo (optional)
* Unique member code

Sensitive information shall remain hidden.

---

# 9.3 Hidden Information

The following must NOT appear publicly:

* Mobile number
* Email
* Address
* Remarks
* Pending edits

Unless explicitly allowed by admin policy.

---

# 9.4 Tree Visualization Features

The tree should support:

* Expand/collapse
* Zoom in/out
* Mobile touch support
* Horizontal layout
* Vertical layout
* Large family rendering
* Smooth navigation

---

# 10. Colour Coding System

Admins shall be able to assign colours to specific members or branches.

Purpose:

* Verified lineage identification
* Pending clarification
* Branch grouping
* Special lineage marking
* Research-required marking

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

# 11. Edit & Approval Workflow

# CRITICAL RULE

## NO DIRECT LIVE EDITS

Approved data must NEVER change directly.

---

# 11.1 Edit Request System

Any approved member may:

* Suggest edits
* Correct names
* Suggest relationships
* Add lineage details
* Upload historical information

---

# 11.2 Approval Queue

Every modification must enter:

* Pending Approval Queue

Only after admin approval:

* Changes become visible live

---

# 11.3 Change Tracking

The system must store:

* Old value
* New value
* Submitted by
* Date/time
* Approval status
* Admin remarks

---

# 11.4 Audit History

All changes must remain traceable permanently.

---

# 12. Member Contribution System

Any approved member may:

* Suggest corrections for any family member
* Add missing lineage information
* Suggest parent-child relationships
* Suggest spouse relationships
* Suggest branch merges

However:

* Nothing becomes live without admin approval

---

# 13. Search Requirements

Approved members shall be able to search by:

* Name
* Nick name
* Native place
* Gothram
* Unique member code
* Father name
* Mother name
* Family branch

---

# 14. Admin Dashboard Requirements

---

# 14.1 Member Management

Admins shall be able to:

* Approve/reject members
* Suspend members
* Edit profiles
* Merge duplicates
* Archive profiles

---

# 14.2 Approval Queue

Admin dashboard must display:

* Pending registrations
* Pending edits
* Pending merges
* Pending relationships
* Pending photo approvals

---

# 14.3 Family Tree Controls

Admins shall be able to:

* Manually restructure branches
* Approve merges
* Approve lineage links
* Assign colours
* Correct relationships

---

# 14.4 Search & Filters

Admin search should support:

* Name
* Gothram
* Native place
* Member code
* Branch
* Relationship type

---

# 15. Privacy Requirements

Only approved members may:

* View trees
* Search members
* Explore relationships

Guest/public users must NOT access:

* Member data
* Family trees
* Search system

---

# 16. Technical Requirements

---

# Frontend

Recommended:

* React.js
* Tailwind CSS

Requirements:

* Mobile-first
* Elder-friendly UI
* Large fonts/buttons

---

# Backend

Recommended:

* Node.js + Express

---

# Database

Recommended:

* PostgreSQL

Reason:

* Better relationship handling
* Better genealogy querying
* Better scalability

---

# Authentication

Recommended:

* OTP login
  OR
* Email/password login

---

# 17. Database Structure (High Level)

---

# Main Tables

### Users

Stores:

* Authentication data
* Approval status
* Roles

---

### MemberProfiles

Stores:

* Personal profile information
* Gothram
* Native place
* Community details

---

### FamilyRelationships

Stores:

* Parent-child relationships
* Spouse relationships
* Branch linkage

---

### PendingChanges

Stores:

* Proposed edits
* Approval workflow
* Change history

---

### MergeSuggestions

Stores:

* Possible relationship matches
* Confidence scores
* Admin decisions

---

### AdminActions

Stores:

* Approvals
* Rejections
* Colour assignments
* Merge decisions

---

# 18. Security & Audit Requirements

The system must log:

* Registrations
* Logins
* Edits
* Relationship changes
* Merge approvals
* Admin actions

Security requirements:

* HTTPS only
* Encrypted passwords
* Role-based access
* Secure APIs
* Unauthorized edit prevention

---

# 19. Scalability Requirements

The platform should support:

* Thousands of members
* Large interconnected genealogy structures
* Multi-generation trees
* Heavy mobile usage
* Future Android app support

---

# 20. Future Enhancements

Future modules may include:

* Matrimony integration
* Temple/community mapping
* Event management
* Family archives
* Heritage records
* AI-assisted duplicate detection
* Elder verification workflows
* Android app

---

# 21. MVP (Minimum Viable Product)

Version 1 must include:

### Member Features

* Registration/login
* Optional profile form
* Draft saving
* Family tree visibility
* Search
* Edit request system

---

### Admin Features

* Approval workflows
* Merge approvals
* Colour coding
* Relationship management
* Audit tracking

---

### Technical Features

* Mobile responsive UI
* Secure authentication
* Unique member codes
* Unified genealogy graph
* Non-destructive editing

---

# 22. Final Core Principles

The platform must prioritize:

1. Community privacy
2. Admin-controlled accuracy
3. Unified genealogy architecture
4. Non-destructive editing
5. Relationship traceability
6. Long-term lineage preservation
7. Mobile-first simplicity
8. Scalability for future generations
9. Duplicate prevention and intelligent merging
10. Collaborative community contribution
