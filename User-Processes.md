 User Processes

This document describes the processes or use cases that users engage in when interacting with our POC prototype application.

## Table of Contents
- [Login Process](#login-process)
- [Register New User](#register-new-user)
- [Create a New User profile](#create-a-new-profile)
  * [Step 1: Profile Name](#step-1-)
  * [Step 2: Profile Contacts](#step-2-)

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

**Who:** All Users

**When:** A user is not registered in the system

To register a new user with the application, first navigate to the login screen by selecting the **Login** button in the top right corner of the screen.

Click the **Sign Up** link below the login form to navigate to the sign up form for new users.

![Sign Up Screen](https://github.com/bcgov/citz-dst-capstone-2021/blob/main/app/docs/images/screen-sign-up.png?raw=true)

Enter relevant user information.

Each field in the form must be validated before the user information is submitted to register a new user:
- **First Name** and **Last Name** fields must be alphanumeric and each be between 1 and 50 characters long.
- **Email** is required and must be a valid email address.
- **Password** is required must contain at least 8 characters, one uppercase character, one number and one special character. Both passwords must match.
- **Job  Profile** is required and must be alphanumeric and be between 1 and 50 characters long.
- **Role** is required and the user must select either Admin, Moderator, or User roles. The default role is User.


Once all fields are filled out and pass validation, select **Submit** to register the new user in the application.

---
