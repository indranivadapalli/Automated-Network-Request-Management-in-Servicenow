# Automated-Network-Request-Management-in-Servicenow
Project Description
This project focuses on building an automated solution in ServiceNow to manage network-related service requests efficiently. Through a self-service portal, users can submit requests using intuitive forms. The system uses ServiceNow’s workflow engine, catalog items, and approval logic to validate and route requests seamlessly. Once submitted, it triggers automated notifications, task assignments, and—if applicable—integrates with network automation tools to fulfill standard requests without manual effort.

Key Features
🗂️ Custom Service Catalog for common network requests

🧾 Dynamic Forms to capture all relevant request details

✅ Automated Approval Workflows based on request type and sensitivity

🔗 Optional Integration with infrastructure or orchestration tools

🔔 Real-Time Notifications for requesters and technicians

📊 Reporting & Analytics on request volume, resolution time, and SLA performance

✅ Steps in Automated Network Request Management in ServiceNow
🟩 1. Automated Network Request Management In ServiceNow

This is the main process or module you're building. It includes automating the entire request flow—from user submission to final fulfillment.

🟧 2. Service Catalog Creation

Create a Catalog Item under Service Catalog (e.g., "Network Access Request")

Define fields like:

Request type

Business justification

IP address/subnet (if needed)

Set Variables, Categories, and Catalog UI Policies

🟧 3. Creation Of Table

Create a custom table (if needed) to store request data.

Use sys_db_object to define the schema.

Set relationships to existing tables (like sc_request or task).

🟧 4. Request Approvals Creation (Related List)

Add Approvers dynamically based on request parameters.

Use Related Lists to track approvals.

Configure Approval Policies or use Flow Designer to create logic for:

Line manager approval

Network team approval

🟧 5. Overview Of Flows, Actions In Flow Designer

Familiarize yourself with Flow Designer:

Triggers (e.g., Catalog submission)

Actions (e.g., approval, task creation, email notifications)

Look into Data Pills, Conditions, and Loops

🟧 6. Creation & Implementation Of Flows, Actions In Flow Designer

Build the actual flow:

Start with a trigger on Catalog submission

Add approval actions

Add task creation for fulfillment

Send email notifications

Implement error handling, logging, etc.

🟧 7. Final Testing In End User Portal & Instance

Test the request end-to-end in the Service Portal

Check for:

UI/UX issues

Proper approval routing

Data saving in the right tables

Notification delivery

Validate results in both test and production instance.
Getting Started Clone the repository

git clone https://github.com/your-username/your-repo-name.git

Set up a ServiceNow Developer instance at https://developer.servicenow.com/.

Follow the documentation or wiki provided in this repo for step-by-step setup instructions.

Demo

To view a demo, check the Demo Video included in this repository.
