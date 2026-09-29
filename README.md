# Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## 📌 Project Overview

The **Standard Laptop Order Automation** project is a ServiceNow solution designed to streamline the IT procurement process for standard laptop requests using **Flow Designer**.

When a Standard Laptop request is approved, the automation automatically creates a **Catalog Task** and assigns it to the **Hardware** team for configuration.

This reduces manual task creation and assignment, improves task visibility, supports timely configuration, and helps provide a consistent procurement workflow.

## 🎯 Project Objectives

* Provide a seamless Standard Laptop requesting experience.
* Reduce manual intervention and potential errors.
* Improve IT resource utilisation.
* Improve procurement efficiency and productivity.
* Automatically generate configuration tasks after approval.
* Assign configuration tasks to the Hardware team.

## 🛠️ Platform & Technology

* **Platform:** ServiceNow
* **Automation Tool:** Flow Designer
* **Business Area:** IT Procurement / Hardware Configuration
* **Service Catalog:** Standard Laptop
* **Assignment Group:** Hardware

## 🔄 Project Workflow

```text
User
  ↓
Service Catalog
  ↓
Standard Laptop
  ↓
Approval
  ↓
Flow Designer
  ↓
Create Catalog Task
  ↓
Hardware Assignment
  ↓
Catalog Task Verification
```

## ⚙️ Flow Designer Configuration

The project uses a Flow named **"Standard laptop task"**.

### Trigger

* Service Catalog

### Action

* Create Catalog Task

### Configuration

| Field             | Value                     |
| ----------------- | ------------------------- |
| Flow Name         | Standard laptop task      |
| Application       | Global                    |
| Run User          | System user               |
| Trigger           | Service Catalog           |
| Action            | Create Catalog Task       |
| Request Item      | Requested Item Record     |
| Short Description | Laptop need to Configured |
| Description       | Laptop need to Configured |
| Assignment Group  | Hardware                  |
| Approval          | Approved                  |

## 🧩 Implementation

The automation is connected to the **Standard Laptop** catalog item through:

**Maintain Items → Standard Laptop → Process Engine → Flow**

After the flow is activated and linked to the catalog item, an approved Standard Laptop request triggers the automated Catalog Task creation.

## 🧪 Testing

The project was designed to verify the following:

1. Standard Laptop is available in the Service Catalog.
2. A Standard Laptop request can be submitted.
3. The request can proceed through approval.
4. The Flow Designer automation runs after approval.
5. A Catalog Task is automatically created.
6. The task contains the required short description and description.
7. The task is assigned to the **Hardware** group.
8. The generated task can be verified from the Requested Item.

## 📸 Project Evidence

Screenshots included in this repository demonstrate:

* Flow Designer configuration
* Service Catalog → Hardware → Standard Laptop
* Service Catalog trigger
* Create Catalog Task action
* Approval process
* Maintain Items → Process Engine configuration
* Requested Item
* Generated Catalog Task
* Hardware assignment

## 🎥 Project Demonstration

The project demonstration shows the complete workflow:

```text
Standard Laptop Request
        ↓
Approval
        ↓
Flow Designer Automation
        ↓
Catalog Task Creation
        ↓
Hardware Assignment
```

The demo verifies that the Catalog Task is generated automatically after the request is approved.

## 👥 Team

**TN Skill Project – Standard Laptop Order Automation with ServiceNow Flow Designer**

Team size: **4 Members including Team Leader**

## ✅ Conclusion

The project demonstrates an automated Standard Laptop procurement workflow using ServiceNow Flow Designer. After approval of a Service Catalog request, the system automatically creates a Catalog Task, populates the required configuration details, and assigns the task to the Hardware group.

The solution reduces manual task creation, improves task allocation and visibility, and supports timely laptop configuration.
