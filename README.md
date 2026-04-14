# ENTERPRISE PLATFORM MODERNIZATION 

### Salesforce to Microsoft Power Platform Migration

#### Role: Senior Business Analyst & Project Lead              
#### Domain: Life Sciences / Pharmaceuticals 

## Executive Summary 

When a global pharmaceutical leader engaged our team to migrate 20+ business-critical applications off Salesforce onto Microsoft Power Platform, it seemed straightforward: replicate everything, preserve every screen, and do it in nine months.

It was neither straightforward nor nine months. 

As the Senior BA and Project Lead managing a globally distributed team across the US, Europe, and Asia-Pacific, I recognised what I came to call the "Replica Fallacy" — the dangerous assumption that a low-code platform built for agility could simply absorb years of layered Apex triggers, hidden validation logic, and 500k+ record data operations without fundamental re-architecture. Surface-level UI screen counts had masked the true complexity beneath. ![](152402b0-cf51-4dcc-80af-22d976a58591_00000.005.jpeg)

Rather than continue reverse-engineering spaghetti logic, I pivoted the entire programme from imitation to intent. Through a formal Logic Inventory protocol and asynchronous stakeholder workshops, I reframed every requirement around a single question: what is this process actually trying to achieve? That shift alone eliminated 40% of cosmetic bugs and unlocked a more performant Model-Driven App architecture that the original Canvas-first approach could never have delivered. ![](152402b0-cf51-4dcc-80af-22d976a58591_00000.006.jpeg)![](152402b0-cf51-4dcc-80af-22d976a58591_00000.007.jpeg)

The outcome: 18 months, double the initial effort estimate, not the numbers in the original slide deck — but the right numbers, earned through technical integrity rather than wishful planning. Custom-engineered solutions replaced expensive third-party middleware including a third-party ETL middleware integration handling 500k+ weekly records, and the consolidated Dataverse environment generated a material reduction in annual platform licensing costs. 

## The Challenge: Navigating the "Replica Fallacy" 

The project was initiated with a rigid stakeholder mandate: a 1:1 functional replica ('same screens, same speed') on a low-code architecture that was never designed for high-code Salesforce parity. 

- **The Logic Trap**: Initial estimations relied on surface-level UI screen counts, missing layered Apex triggers and hidden validation rules. 
- **Architecture Gaps**: High-volume data loads (500k+ records) that were instantaneous in Salesforce faced timeouts and delegation limits in Power Apps. 
- **Complexity Bloat**: Many legacy apps were unnecessarily complicated, requiring intensive reverse engineering of "spaghetti logic" rather than modern requirement gathering. 

## Strategic Intervention & Remote Leadership 

Faced with a timeline that threatened to double, I pivoted the project from 'Reverse Engineering' to Intent-Based Discovery. 

- **Global Stakeholder Management**:  Managed alignment across US, Europe, and Asia-Pacific using asynchronous workshops (Jira) to maintain momentum across time zones. 
- **The Logic Audit**: Implemented a formal "Logic Inventory" protocol to simplify legacy processes before estimation, replacing "T-shirt sizing" with technical reality. 
- **Framework Pivot**: Negotiated the shift from UI-heavy Canvas Apps to performance-optimized Model-Driven Apps (MDA) for complex relational entities, leveraging native responsiveness to eliminate 40% of cosmetic bugs. 

## Technical Innovation & Value Delivered 

To bridge significant platform gaps, I oversaw the engineering of high-impact custom utilities. 

- **Global Search Connector**: Overcame native Canvas limitations by engineering a custom connector for seamless cross-entity search. 
- **Scalable Data Flows**: Replaced expensive Boomi integrations with native Dataflows to support weekly loads of 500k+ records without API throttling. 
- **Advanced Multi-Attachment**:  Developed a custom asynchronous workflow combining JavaScript and Power Automate to enable robust multi-attachment support in Dataverse. 
- **Localization**: Engineered a localization utility for full Japanese language support within Canvas Apps 

## Project Performance & ROI 

|Metric |Initial Estimate |Final Outcome |
| - | - | - |
|Timeline |9 Months |18 Months |
|Effort / Cost |1\.0x |~2.0x  |
|Value Realization |<p>- Significant Reduction in Licensing Cost (~10-20% of SFDC) </p><p>- 5000+ Licenses Migrated to PowerApps </p><p>- 300+ Licenses saved by identifying and de-scoping unutilized apps </p><p>- Lower operational cost </p>

## Key Lessons & Playbook for Future Migrations 
- **Discovery ≠ Demo**: My biggest lesson was prioritizing business outcomes ("What is the intent?") over historical behavior ("How did the old button work?"). 
- **Load Test Early**: Production-level data volumes (500k+ records) must be tested within the first month to identify delegation bottlenecks. 
- **Governance First**: Establish a Change Control Board (CCB) early to sign off on behavioral shifts between Salesforce and Power Platform. 

**Technical Stack: Power Apps (Canvas/Model-Driven), Dataverse, Power Automate, Dataflows, JavaScript, SQL, Salesforce (Apex/SOQL).**
