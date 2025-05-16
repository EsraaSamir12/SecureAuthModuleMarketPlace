## 🔐 Authentication & Authorization Module – MarketPlace Project

This module is responsible for handling **authentication, authorization, and security** in the MarketPlace project, built using **ASP.NET Core** with a **Database First** approach and designed as a RESTful API.

### ✅ Key Features:

- **User Registration** with validation and hashed password storage.
- **Login / Logout** functionality using JWT-based authentication.
- **AES-256 Encryption** for securing sensitive data before database insertion.
- **Password Hashing** with salt to prevent credential leakage.
- **JWT Access Tokens** for authenticated user sessions.
- **Refresh Tokens** handled securely on the **server-side**:
  - Stored in the database with expiration time and associated metadata (e.g., IP, device).
  - Refresh token rotation implemented to minimize reuse.
  - Ability to revoke tokens on logout or security events.
- **Role-based Authorization** for controlling access (Admin, Vendor, Customer).
- **Secure token validation** services using middleware and filters.
- Designed following **RESTful best practices** for seamless integration.

### 🛡️ Security Focus:
This system ensures secure handling of user credentials, protects sensitive user data using encryption and hashing, and manages access tokens in a way that prioritizes security and flexibility.

---

💡 This module is production-ready and can be adapted for other projects requiring secure, scalable user authentication and authorization logic.
