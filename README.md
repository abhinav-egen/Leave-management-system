# Leave Management Solution

## Overview
Develop an Employee Leave Management System where employees can apply for leaves, track their leave history, and managers can approve/reject requests.

## Technology Stack
- **Frontend**: Angular
- **Backend**: FastAPI
- **Database**: BigQuery, Firestore
- **Authentication**: Firebase Authentication (dummy for this assignment)
- **Deployment**: Cloud Run

## Features

### 1. Authentication (Dummy Login)
- The application will have a dummy login module with hardcoded credentials.
- **Reportees**: 3 hardcoded usernames and passwords.
- **Managers**: 2 hardcoded usernames and passwords.
- Upon successful login, users will be redirected to their respective dashboards.

### 2. Reportee Functionality
- Apply for leave by providing:
  - Start date
  - End date
  - Reason for leave
- View applied leaves and their statuses.
- Delete leave requests (if not yet approved/rejected).

### 3. Manager Functionality
- View pending leave requests.
- Approve or reject leave requests.

## Backend (FastAPI & Cloud Run)
- Implement APIs to:
  - Submit leave requests (stored in BigQuery).
  - List leave requests:
    - Employees can see their own requests.
    - Managers can see all pending requests.
  - Approve/reject leave requests (restricted to managers).
- Secure APIs using Firebase Authentication and role-based access control.
- Deploy the FastAPI backend on Cloud Run.

## Database Schema (BigQuery)
The following fields will be stored in BigQuery:
- **Employee ID**
- **Start Date**
- **End Date**
- **Reason**
- **Status** (Pending, Approved, Rejected)
- **Manager ID**

## Deployment
- The Angular frontend will be deployed using Firebase Hosting or Cloud Run.
- The FastAPI backend will be deployed on Cloud Run.
- Firestore may be used for storing user roles and authentication-related data.

This project serves as an assignment-based implementation of a Leave Management Solution using Angular, FastAPI, and Google Cloud services.

