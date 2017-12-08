# Managing Work(Work In Progress)

## Agile Process Definitions
* Epics - Correspond to Business Cases or PDM Objectives - Owned by Executives, Rod, Jason
* Features - Customer Facing Deliverables - Owned by DAD Management
    * Always require a functional owner even if it crosses team boundries
* User Stories - Owned By DAD teams to manage work for Features.
* Tasks - Owned by DAD Developers for managing work required to complete Stories
* Iterations - 3 weeks, Features are slotted for Iteration n+2 when possible
* Plan - Presented to Executive Management as an estimate for Feature/Epic completion
* Current Iteration Backlog - Work team is expected to complete(where developers live)

## ServiceNow Tickets(triaged twice per day)
### MyHubbell Tickets
Development tickets and operation support tickets stay in the Portal Queue
### All other tickets
* Routed to Digital Application Development Queue
#### Triage Process
* Operational Support Tickets(transitioning to issues queue in near future)
    * Create User Story in VSTS(if Hybris under operationial support feature, corresponding Epci otherwise no parent)
        * Tag User Story with INCNumber
        * Tag User Story with Application 
        * Prioritize based on [SLA](SLA.md) criteria 
        * Assign VSTS User Story to Iteration/Team/Team Manager
        * Enter VSTS ticket number in ServiceNow Flex Field 4
        * Change ServiceNow ticket status to Work Started            
* Defects
    * Create Bug in VSTS(if Hybris under operationial support feature, corresponding Epic, otherwise no parent)
        * Tag Bug with INCNumber
        * Tag Bug with Application 
        * Prioritize based on [SLA](SLA.md) criteria 
        * Assign VSTS Bug to Iteration/Team/Team Manager if required by SLA
        * Enter VSTS ticket number in ServiceNow Flex Field 4
        * Change ServiceNow ticket status to Work Started  
* Enhancements
    * If enhancement requires more than 40hrs of development time, URF required, and Business Case Council approval required
        * Request URF, attach to ticket assign to Jason Bouchard for review and submittal to BC council
        * Once approved, VSTS Epic will be created from ServiceNow ticket
    * If enhancement is less than 40hrs
        * Create Feature, including acceptance criteria("definition of done")
        * Tag Feature with ServiceNow ticket Number
        * Tag Feature with Application
        * If Feature part of existing Epic, link to parent Epic
        * Enter VSTS ticket number in ServiceNow Flex Field 4
        * Change SerivceNow ticket status to Work Started

## Non ServiceNow Ticket Requests(email, phone, etc)
* Create VSTS ticket directly using above criteria

## VSTS Ticket Status Flow
### Features
* Active
    * Requirements gathering or assigned to Iteration
* Resolved
    * Feature deployed to UAT awaiting UAT approval from stake holder
* Closed
    * Feature approved by stakeholder(s)
    * Resolve corresponding ServiceNow ticket if one exists in tags
### User Stories(to be discussed?)
* Active - Assigned to current iteration
* Resolved - Developer Tested
* Closed - Tested in QA
### Defects
* Active - Assigned to current iteration
* Resolved - Developer verified
* Closed - Pushed to production, Resolve corresponding ServiceNow ticket if one exists in tags
### Issues(Operational Support not involving code changed - TBD)





