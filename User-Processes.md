 User Processes

This document describes the processes or use cases that users engage in when interacting with our POC prototype application.

## Table of Contents
- [Login Process](#login-process)
- [Register New User](#register-new-user)
- [Create a New Project](#create-a-new-project)
  * [Step 1: Project Identification](#step-1-project-identification)
  * [Step 2: Project Contacts](#step-2-project-contacts)
  * [Step 3: Project Timeline Information](#step-3-project-timeline-information)
      - [Add a Milestone](#add-a-milestone)
      - [Edit a Milestone](#edit-a-milestone)
      - [Delete a Milestone](#delete-a-milestone)
  * [Step 4: Business Case Objectives](#step-4-business-case-objectives)
      - [Add a Business Case Objective](#add-a-business-case-objective)
      - [Edit a Business Case Objective](#edit-a-business-case-objective)
      - [Delete a Business Case Objective](#delete-a-business-case-objective)
  * [Step 5: Key Performance Indicators](#step-5-key-performance-indicators)
      - [Add a New Key Performance Indicator](#add-a-new-key-performance-indicator)
      - [Edit a Key Performance Indicator](#edit-a-key-performance-indicator)
      - [Delete a Key Performance Indicator](#delete-a-key-performance-indicator)
- [Complete a Quarterly Report](#complete-a-quarterly-report)
  * [Step 1: Project Information](#step-1-project-information)
  * [Step 2: Status Summary](#step-2-status-summary)
  * [Step 3: Financial Information](#step-3-financial-information)
  * [Step 4: Business Case Objective Tracking](#step-4-business-case-objective-tracking)
  * [Step 5: Key Milestone Status](#step-5-key-milestone-status)
  * [Step 6: Key Performance Indicators](#step-6-key-performance-indicators)
  * [DIO Submission](#dio-submission)
- [Review a Quarterly Report](#review-a-quarterly-report)


## Login Process

> :warning: The login solution presented in this POC prototype is temporary and will be replaced with an existing authentication system such as KeyCloak.

**Who:** All User Personas

**When:** A registered user is not currently logged into the application.

When a user first comes to the application they are presented with a landing page that describes the project goals, application roles, and a link to an about view describing the project further.

![Landing Page](https://github.com/bcgov/citz-dst-capstone-2021/blob/main/app/docs/images/screen-landing.png?raw=true)

User selects the yellow **Login** button in the top right corner of the screen to navigate to the sign in view.

![Login Screen](https://github.com/bcgov/citz-dst-capstone-2021/blob/main/app/docs/images/screen-login.png?raw=true)

User enters email and password into fields.

User selects **Submit** to send login information to API to validate login process.

If a user successfully logs in, then they are redirected to their dashboard. Otherwise they remain on the sign in view.

---

## Register New User

**Who:** Submitter, Finance Analyst, Data Analyst, & Executive

**When:** A user is not registered in the system

To register a new user with the application, first navigate to the login screen by selecting the **Login** button in the top right corner of the screen.

Click the **Sign Up** link below the login form to navigate to the sign up form for new users.

![Sign Up Screen](https://github.com/bcgov/citz-dst-capstone-2021/blob/main/app/docs/images/screen-sign-up.png?raw=true)

Enter relevant user information.

Each field in the form must be validated before the user information is submitted to register a new user:
- **First Name** and **Last Name** fields must be alphanumeric and each be between 1 and 50 characters long.
- **Email** is required and must be a valid email address.
- **Password** is required must contain at least 8 characters, one uppercase character, one number and one special character. Both passwords must match.
- **Job Title** is required and must be alphanumeric and be between 1 and 50 characters long.
- **Role** is required and the user must select either Admin, Submitter, Finance Analyst, Executive, or User roles. The default role is User.
- **Ministry** is required and the user must select from a list of BC Government ministries.

Once all fields are filled out and pass validation, select **Submit** to register the new user in the application.

---

## Create a New Project

 **Who:** Submitter

>**When:** An approved project is not registered in the system.

**Assumptions:**
- Submitter has required information available when filling out form.
- Milestones, business case objectives, and key performance indicators have been defined and approved in the project approval process.

When a project is approved for funding by the DIO it can then be entered into the application for quarterly status reporting. This helps reduce manual effort seen in the original reporting process by having the Submitter enter project information and contacts once instead of every report.

When a Submitter logs into the application, they are presented with a list of projects that exist in the system.