# Laptop Request Catalog Item – ServiceNow Project  

## Team Details  
**Team ID:** NM2025TMID06861  
**Team Size:** 4  

**Team Leader:** Madasamy S  
**Team Members:**  
- Gnana Rajakishore J  
- Karthick Raja S  
- Ano Raja Jainson J  

---

## Project Overview  
The **Laptop Request Catalog Item** project automates the laptop request process using **ServiceNow**. It replaces manual, error-prone methods with a dynamic catalog form that ensures accuracy, faster approvals, and better tracking for both employees and IT administrators.

---

## Problem Statement  
Employees face delays and errors when requesting laptops through manual processes. A ServiceNow-based automated catalog item is needed to simplify requests, collect accurate data, and enable easy tracking and approval workflows.

---

## Proposed Solution  

### Solution Description  
- A **Service Catalog item** that allows employees to request laptops with guided dynamic fields.  
- **Additional accessories** fields appear only when selected.  
- Includes **form reset** and **change tracking** functionality.  
- Uses **update sets** for deployment and governance.  

### Uniqueness  
- Dynamic field behavior and real-time validation.  
- Workflow automation with minimal manual intervention.  
- Integration with CMDB for asset tracking.  

### Customer Satisfaction  
- Simplified and faster request process.  
- Transparent approvals and notifications.  
- Improved employee experience through automation.  

### Business Model  
- Reduces IT support workload.  
- Improves process efficiency and accuracy.  
- Supports organizational digital transformation goals.  

### Scalability  
- Can be extended for other hardware/software request processes.  
- Modular and reusable ServiceNow components enable easy maintenance.  

---

## Architecture  

### Goal  
To design a scalable and automated system for managing laptop requests, ensuring accuracy, speed, and better governance.  

### Key Components  
- **Frontend:** Service Catalog Form  
- **Application Layer:** Catalog Client Scripts, UI Policies, Workflow Automation  
- **Backend:** Request Tables (`sc_request`, `sc_req_item`, `task`)  
- **Integration:** CMDB for asset mapping  
- **Deployment:** Update Sets (Dev → Test → Prod)  

### Development Phases  
1. Requirement Analysis  
2. Catalog Item Creation  
3. Scripting & Workflow Implementation  
4. Testing & Validation  
5. Deployment using Update Sets  

### Solution Architecture Description  
The architecture leverages ServiceNow’s layered framework.  
Users interact with a dynamic Service Catalog form. Business rules and workflows process the request and store data in ServiceNow tables. Integration with the CMDB ensures asset tracking. Update sets handle version control and deployment across environments.  

---

## Data Flow  

1. User opens the **Laptop Request** form in the Service Catalog.  
2. System displays fields dynamically based on user selections.  
3. The submitted data is stored in ServiceNow tables.  
4. Workflows trigger necessary approvals and task creation.  
5. All changes are tracked and deployed using update sets.  

---

## Technology Stack  
- **Platform:** ServiceNow  
- **Modules Used:** Service Catalog, Flow Designer, CMDB, Update Sets  
- **Scripting:** JavaScript (Client Scripts, UI Policies)  
- **Database:** ServiceNow Tables  

---

## Performance Testing  
- Verified form responsiveness and dynamic loading speed.  
- Tested approval workflows under concurrent requests.  
- Ensured smooth migration between instances via update sets.  

---

## Project Explanation  
> Our project, **Laptop Request Catalog Item**, aims to automate the laptop request process for employees using ServiceNow.  
>  
> The traditional manual method caused delays and data errors. We built a dynamic catalog item that adjusts based on user input — for instance, accessory details appear only when the user selects them.  
>  
> The backend automates workflows and approvals while maintaining data in ServiceNow tables and CMDB for asset management. We used update sets for deployment, ensuring smooth migration across environments.  
>  
> The result is a faster, error-free, and transparent laptop request process that enhances user experience and operational efficiency.  

---

## Setup & Deployment (Optional)  
1. Go to **System Update Sets → Retrieved Update Sets**.  
2. Click **Import Update Set from XML** and upload the downloaded XML file.  
3. Preview and **Commit the Update Set**.  
4. Search for **Service Catalog → Hardware → Laptop Request** to test the item.  

---

## Conclusion  
The **Laptop Request Catalog Item** project successfully automates the laptop request workflow, improving speed, accuracy, and governance.  
It showcases how **ServiceNow** can replace manual, repetitive tasks with efficient and dynamic solutions that scale easily for future requirements.  

---
