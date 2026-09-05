<p align="center">
  <img src="https://drive.google.com/uc?export=view&id=1Apq4i7-ZMG_7TQx8to2TTHgL4GsOARsb" alt="ServiceNow Logo" width="200"/>
</p>

# Automated Network Request Management in ServiceNow

An individual ServiceNow project designed to simplify and automate the management of network-related service requests using **Service Catalog, Flow Designer, approvals, notifications, and request management**.

---

## 📌 Project Overview

**Automated Network Request Management in ServiceNow** is a custom request management solution developed to make the submission and processing of network-related requests easier and more organized.

The application allows employees to submit network requests through the **Service Catalog** by providing requester, connection, address, device, and other required details.

The submitted request is then processed using **Flow Designer**, which automates activities such as retrieving catalog variables, creating a network request record, sending the request for approval, sending notifications, and updating the request.

### Key Benefits

- Simplifies network request submission
- Reduces manual processing
- Automates request workflows
- Improves request tracking
- Provides structured request information
- Reduces repetitive administrative work
- Improves visibility of request status

---

## 🎯 Project Objectives

The main objectives of this project are:

- To provide a simple **Service Catalog** for submitting network requests.
- To capture all required requester and network information.
- To use dynamic fields to display relevant information based on user selections.
- To automate request processing using **Flow Designer**.
- To automatically create and manage network request records.
- To implement an approval process for submitted requests.
- To send email notifications during request processing.
- To provide better visibility and tracking of network requests.

---

## ✨ Key Features

### 1. Network Request Service Catalog
Employees can submit network-related requests through a user-friendly Service Catalog form.

### 2. Request Information Capture
The form captures important information such as:

- Requested For
- Email ID
- User Name
- Phone Number
- Connection Type
- Relocated Address
- Device Type
- Address
- Device Details
- Other Details

### 3. Dynamic Form Fields
Relevant fields are displayed based on the selected options. For example, additional information can be entered when a specific device type is selected.

### 4. Automated Record Creation
After a request is submitted, the configured Flow Designer process automatically creates the corresponding network request record.

### 5. Approval Management
Submitted requests are processed through the configured approval workflow before further processing.

### 6. Workflow Automation
Flow Designer automates the request lifecycle and reduces the need for manual processing.

### 7. Email Notifications
Configured email notifications provide updates related to the network request.

### 8. Request Tracking
The request status can be monitored during the processing lifecycle.

### 9. Reporting
Network request information can be monitored using ServiceNow reporting capabilities.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **ServiceNow** | Application development platform |
| **App Engine Studio / Creator Studio** | Application development |
| **Service Catalog** | Network request submission |
| **Flow Designer** | Workflow automation |
| **ServiceNow Tables** | Request data storage |
| **UI Policies / Catalog Configuration** | Dynamic form behavior |
| **Notifications** | Email communication |
| **Reports** | Request monitoring and analysis |

---

## ⚙️ Project Implementation

The project was implemented in the following stages:

### Step 1 – ServiceNow Developer Instance

A ServiceNow Personal Developer Instance (PDI) was used for developing and testing the application.

### Step 2 – Application Creation

A custom application was created for managing network-related requests.

### Step 3 – Service Catalog Configuration

A **Network Request** catalog item was created to allow employees to submit requests.

### Step 4 – Variable Configuration

Required variables were configured to capture requester, connection, address, device, and additional information.

### Step 5 – Dynamic Form Configuration

UI policies and catalog configurations were used to display relevant fields based on user selections.

### Step 6 – Network Request Table

A custom table was configured to store the submitted network request information.

### Step 7 – Flow Designer Automation

A Flow Designer workflow was configured to automate the request process:

```text
Service Catalog
      ↓
Get Catalog Variables
      ↓
Create Network Request Record
      ↓
Approval
      ↓
Send Email Notification
      ↓
Update Network Request Record
