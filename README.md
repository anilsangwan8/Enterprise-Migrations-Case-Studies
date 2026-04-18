# ENTERPRISE PLATFORM MODERNIZATION 

### Salesforce to Microsoft Power Platform Migration

#### **Role**: Senior Business Analyst & Project Lead              
#### **Domain**: Life Sciences / Pharmaceuticals 

Link : [The_Migration_Blueprint.pdf](https://github.com/user-attachments/files/26858389/The_Migration_Blueprint.pdf)

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

## Project Implementation Best Practices

| Area | DO | DON’T |
| :--- | :--- | :--- |
| **Discovery** | **DO** conduct "Logic Audits" to simplify and retire legacy "Spaghetti logic" before building. | **DON’T** assume Reverse Engineering an old app is faster than a fresh business requirement workshop. |
| **Architecture** | **DO** use Model-Driven Apps for data-heavy, complex relational entities to ensure performance. Make App on Start light weight. | **DON’T** use Canvas Apps as a default for everything just to "control the UI." |
| **User Interface** | **DO** adopt the "Power Apps Native" look and feel to leverage built-in responsiveness. | **DON’T** promise an "Exact SFDC Replica." It leads to endless cosmetic reopens. |
| **Performance** | **DO** load test with Production-level data volumes (e.g., 500k+ records) during the first month. | **DON’T** wait for UAT to realize that a data upload or gallery filter is timing out. |
| **Data Handling** | **DO** use Azure Integrations or Dataflows for larger real-time data processing. | **DON’T** rely on Standard Power Automate or App-side logic for large data volume (> 1Lac) transactions. |
| **Governance** | **DO** establish a Change Control Board with Client IT Heads to sign off on behavioral shifts. | **DON’T** let the Business see the first demo without having already signed off on the functional / behavioral differences. |
| **Testing** | **DO** use the Power Apps Test Studio to automate regression and alignment checks. | **DON’T** treat UAT as a discovery phase; it should be a final validation of a frozen scope. |
| **Vendor Management** | **DO** build an Internal Workaround Library for known platform limitations. | **DON’T** wait for Microsoft Support to solve "Blocker" issues; their SLA might not match your project velocity. |
| **App Start** | **DO** use `App.Formulas` and `Concurrent()` to load data in the background. | **DON’T** put heavy `ClearCollect()` in `OnStart` that forces a user to wait 20 seconds. |
| **Data Logic** | **DO** push complex validation to Dataverse Plugins or Calculated Columns (Server-side). | **DON’T** rely on Power Fx formulas on a "Submit" button to handle critical business rules. |
| **Error Handling** | **DO** build a custom Error Log Table to capture when flows or app formulas fail. | **DON’T** assume the "App Checker" or MS Support will catch every performance bottleneck. |

**Technical Stack: Power Apps (Canvas/Model-Driven), Dataverse, Power Automate, PowerBI, Dataflows, JavaScript, SQL, Salesforce (Apex/SOQL).**
