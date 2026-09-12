# Feature: Van Route & Transportation Tracking 
**Feature ID:** 2
**Branch pattern:** `feature/N-Van-Transportation-Tracking`
**Status:** Draft
**Created:** 2026-09-07

## User Stories
---
### US-N.1: Route Configuration
**As a** Admin 
**I want to** Create, Update, Merge, or remove named routes.
**So that** Routes will be properly managed.
### US-N.2: Stop & Passenger List
**As a** Driver
**I want to** Access stops and list of people at specific stops
**So that** I know who to pick up and what stops to go to each week
### US-N.3: Driver Assginment
**As a** Admin 
**I want to** see each assigned route and each driver available
**So that** each route will be driven each week and each driver is assigned somewhere


## Functional Requirements
---
- **FR-001**: System MUST update, merge, remove, or create routes 
- **FR-002**: System MUST allow drivers to access their route and list of people along route
- **FR-002**: System MUST allow drivers to be assigned to routes and be able to manage drivers

## Gherkin AC
---
#### Scenario: Driver access (happy path)
* **Given** Driver has route
* **When** driver accesses his routes addresses and list of people to pick up
* **Then** people are properly picked up and everyone is picked up
