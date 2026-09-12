# Feature: Member & Family Management 
**Feature ID:** 1
**Branch pattern:** `feature/N-Member-Family-Management`
**Status:** Draft
**Created:** 2026-09-07

## User Stories
---

### US-N.1: Admin management
**As a** Admin
**I want to** track member and non-member guests
**So that** we can see attendance rates and mark people as active or inactive based on attendance history

### US-N.2: User Access
**As a** Church Member
**I want to** acknowledge that I am at church each week and be able to update information 
**So that** The church can have my current information such as, address or phone number if they need to contact me

### US-N.4: Manage Families
**As a** Admin
**I want to** group people with the same address or household into a general Family
**So that** You can find people by family and generally know who somebody is 

## Functional Requirements
---
- **FR-001**: System MUST accept data from a Member/Guest such as thier email, address, and/or phone number
- **FR-002**: System MUST allow a users profile to be editted by admin or a user with admin approval
- **FR-002**: System MUST allow a member to check in when they come to church

## Gherkin AC
---
#### Scenario: Grouping Existing members into a family household (happy path)
* **Given** Two Members have information of the same address
* **And** They are not already in a Family grouping
* **When** An Admin links the two members into a singlular household
* **Then** The two members will be under the same household 

#### Scenario: Guest Access (happy path)
* **Given** A guest wants to become a member or check-in
* **When** They enter their information into the software
* **Then** The guest will have their information entered into the system 