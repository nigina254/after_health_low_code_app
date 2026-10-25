# AfterHealth — Post-Discharge Care Management App

**AfterHealth** is a low-code healthcare application developed as a group project for the **DevOps and Low-Code Development** course. Built with Microsoft Power Platform, it aims to improve communication between patients and healthcare providers after hospital discharge by bringing discharge information, medications, appointments, follow-up details, and AI-assisted guidance into one application.

The project combines low-code application development with data management, workflow automation, testing, monitoring, and a **Development → Test → Production** deployment pipeline.

## 🎯 Objectives

- Help patients access their post-discharge instructions and relevant health information.
- Give doctors a centralized interface for discharge reports and appointment management.
- Support medication adherence through scheduled reminders.
- Improve access to aftercare information with an integrated conversational assistant.
- Apply DevOps practices to solution versioning, testing, and controlled deployment.

## ✨ Main Features

### Patient experience
- Patient login and a dedicated patient dashboard.
- Access to medication details, dosage schedules, and instructions.
- View, schedule, or cancel appointments.
- Access discharge and follow-up information.
- Chat with **CareMate Copilot** about relevant aftercare information and patient-specific records.

### Doctor experience
- Doctor login and a dedicated doctor interface.
- Doctor home page with access to discharge reports.
- Discharge report and appointment-management screens.
- Interfaces designed to support reviewing and managing patient information.

### Automation and AI
- **Power Automate:** creates calendar reminders for prescribed medication over a specified date range.
- **Microsoft Copilot Studio:** provides a conversational assistant connected to relevant Dataverse information and aftercare guidance.
- **Microsoft Dataverse:** stores structured information used by the application, including patient, doctor, appointment, discharge, and follow-up records.

> **Project status:** This is an academic prototype. The report identifies some features and data flows as future enhancements, so not every planned capability should be assumed to be fully implemented or production-ready.

## 🧰 Technology Stack

- **Microsoft Power Apps** — low-code application UI and logic
- **Microsoft Dataverse** — structured data storage
- **Microsoft Power Automate** — medication reminder workflow
- **Microsoft Copilot Studio** — conversational AI assistant
- **Microsoft Power Platform Pipelines** — solution deployment across environments
- **Azure DevOps / Azure Boards** — task planning and work tracking
- **GitHub** — source control and project files

## 🏗️ DevOps Workflow

The project uses a three-stage application lifecycle management (ALM) workflow:

```text
Development  →  Test  →  Production
```

1. **Development:** create and modify the app, flows, tables, and other solution components.
2. **Test:** deploy a managed solution and validate UI behavior, Dataverse connections, and Copilot interactions.
3. **Production:** promote the tested and approved solution for end-user access.

Deployments are triggered through Power Platform Pipelines. Solution versions are updated before deployment, and required components, connection references, and environment variables must be included and configured for the target environment.

The project also covers functional testing and performance monitoring, including network-call duration, data-loading time, delegation warnings, and screen/control rendering time.

## 🚀 How to Run the Application


### Import and run the solution

If the repository contains an exported Power Platform solution package, use the following general workflow:

1. **Check the repository files.** Locate the exported solution package and review any project documentation. A Git repository containing source files does not necessarily include a ready-to-import solution package.
2. **Open Power Apps.** Go to [make.powerapps.com](https://make.powerapps.com/) and select an environment where you have permission to import solutions.
3. **Import the solution.** In the Power Apps maker portal, open **Solutions** and use the import option to import the provided solution package.
4. **Configure dependencies.** Set up the required Dataverse tables and data, connection references, environment variables, permissions, and any required Power Automate flows.
5. **Configure Copilot.** Ensure the CareMate Copilot component is available and connected to the correct data sources and approved knowledge.
6. **Publish and test.** Publish the required components, launch the app, and verify patient and doctor workflows using authorized test data.

The exact menu labels may vary with the Power Platform interface and your permissions. If no solution package is included, the app may need to be opened from its original Power Platform environment or exported by someone with access.


## 🧪 Testing and Monitoring

The project report describes functional testing and monitoring of application behavior, including:

- Screen rendering and navigation.
- Dataverse data retrieval and updates.
- Appointment and discharge-related workflows.
- Copilot responses and data access.
- Network-call duration and data-loading performance.
- Delegation warnings and unnecessary data operations.

Testing should be repeated in the target environment after changes are deployed.



## 👩‍💻 My Contributions

As documented in the project report, my contributions included:

- Implementing parts of the Power Apps interface and functionality.
- Developing the doctor home page, including layout and navigation.
- Designing and implementing the chatbox and full chat page UI.
- Building and managing the **Development → Test → Production** deployment pipeline.
- Deploying the solution across pipeline stages and handling configuration and version updates.
- Integrating a custom Copilot through Microsoft Copilot Studio.
- Supporting testing, debugging, and application improvements.

This was a collaborative group project; the list above describes my reported contributions rather than claiming sole authorship of the application.

## 📚 Course Context

Developed as part of the **DevOps and Low-Code Development** course, the project provided practical experience with low-code application development, workflow automation, data modeling, AI integration, testing, and deployment lifecycle management.

## 🔗 Repository

[AfterHealth — GitHub repository](https://github.com/nigina254/after_health_low_code_app)

## 👤 Author

**Nigina Abdukhalimova** · [GitHub profile](https://github.com/nigina254)
