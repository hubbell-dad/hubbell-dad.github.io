# Service Level Aggreements



| Problem Description       | Response Time    |Trigger| Communication(updates)     | Group(s) to Enage |
| ------------------------- | ---------------- | -------|---------- |----------------|
| Site Unreachable| ASAP |Dynatrace |Service Bulletin(Jason Bouchard) - Forward to Leads(2hrs)| Basis/NTT/DAD-Java
| Unable to Place Orders(OHW)| ASAP|? | Service Bulletin(John Ray) - Forward to Leads(2hrs)| DAD-Java/HUBS
| Performance drops below standard| Plan - 24hrs| Dynatrace | Email to Leads(24hrs)| DAD-Java/DAD-UX
| Content Updates - Critical| 2hrs | Email |Email when complete |DAD-NET
| Content Updates - Normal | 48hrs | Ticket | Close Ticket When Complete | DAD-NET
| Product Updates - Critical | 2hrs | Email | Email when complete | DAD-Java/HUBS-STEP
| Product Updates - Normal | 48hrs | Ticket | Close Ticket When Complete | HUBS-STEP
| Facet/Attribute Updates | 72hrs | Ticket | Close Ticket When Complete | HUBS-STEP/DAD-Java
| Defects - Critical| ASAP - Special Build | Email | Email when Complete | HUBS-DAD |
| Defects - High| Next Scheduled Build | Email | Email when complete| HUBS-DAD |
| Defects - Medium/Low| Normal Deployment | Ticket | Release Notes | HUBS-DAD |
| Enhancements| Set By Phil B|||


### Definitions
* Content Updates - CMS driven updates
* Product Updates - Product data representative of whats in STEP
* Defects - Any unexpected funtional behavior
* Critical(Content/Product) - Legal, Systemic, or Extremely Time Sensitive
* Normal(Content/Product) - Product or Content not udpated as expected through normal process flow
* Critical Defect - Must fix. An unexpected system behavior that causes failure, data corruption, or significant customer impact and there are no acceptable alternative methods to achieve required results. Special Deployment required.
* High Defect - Consider fix. An unexpected system behavior that causes failure, data corruption, or significant customer impact and there are no acceptable alternative methods to achieve required results.. However, an acceptable alternative method exists to achieve required results. Required in next build.
* Medium(default) - A defect that causes the system to produce incorrect, incomplete or inconsistent results.
* Minor - A minor or cosmetic defect that has acceptable workarounds to achieve required results.
