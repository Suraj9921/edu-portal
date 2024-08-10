# Spring Security Practice Project

This project is created to practice and understand Spring Security features. It includes basic security configurations for a web application. Below are the key features and settings:

## Key Features

- **Custom Login Handlers**: 
  - Custom logic for handling successful and failed login attempts.

- **Security Rules**:
  - The `/dashboard` page requires users to be logged in.
  - Public pages such as `/home`, `/contact`, and static assets are accessible without login.

- **Login Settings**:
  - Custom login page at `/login`.
  - Login fields are set to `userid` for the username and `secretPwd` for the password.
  - Successful login redirects to `/dashboard`; failure redirects to `/login?error=true`.

- **Logout Settings**:
  - Logging out redirects to `/login?logout=true` and clears the session and cookies.

- **In-Memory User Accounts**:
  - Two users:
    - `user` with read-only access.
    - `admin` with full access.
  - Passwords are stored in plain text for `user` and encrypted for `admin`.

- **Password Security**:
  - Passwords are encoded using a built-in encoder that supports various methods.

- **Compromised Password Check**:
  - Checks passwords against known compromised passwords using the Have I Been Pwned API.

## Configuration Details

- **CSRF Protection**: Disabled for practice purposes. Enable it as needed for production use.
- **Basic Authentication**: Enabled as a fallback option.

This project serves as a hands-on practice for setting up and configuring Spring Security.
