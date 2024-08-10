## Spring Security Practice Project

This project is designed to practice Spring Security. It includes:

- **Custom Login Handlers**: Custom logic for successful and failed login attempts.
- **Security Rules**: 
  - `/dashboard` requires authentication.
  - Public pages like `/home`, `/contact`, and static assets are open to everyone.
- **Login Settings**: 
  - Custom login page at `/login`.
  - Fields: `userid` (username) and `secretPwd` (password).
  - Success redirects to `/dashboard`; failure to `/login?error=true`.
- **Logout Settings**: 
  - Redirects to `/login?logout=true` and clears session and cookies.
- **In-Memory Users**: 
  - `user` with read access and `admin` with full access.
  - Passwords: plain text for `user`, encrypted for `admin`.
- **Password Security**: 
  - Encoded with a built-in encoder.
- **Compromised Password Check**: 
  - Uses Have I Been Pwned API to check passwords.

**Note:** CSRF protection is disabled for practice. Basic authentication is also enabled.

---

This setup helps in learning and practicing Spring Security features.
