### ✅ **General API Concepts**

**1. What is an API? Why are APIs important?**  
An **API (Application Programming Interface)** is a set of rules that allows different software systems to communicate. APIs are important because they enable integration between systems, support automation, and allow developers to build functionality on top of existing services (e.g., Google Maps API, Twitter API).

**2. What are the different types of APIs?**  
- **REST (Representational State Transfer)**: Uses HTTP and is stateless. Most common.
- **SOAP (Simple Object Access Protocol)**: Protocol-based, uses XML, more strict and secure.
- **GraphQL**: A query language that allows clients to request exactly the data they need.
- **Webhooks**: One-way notifications from one system to another (event-driven).
- **Reverse API (Call-In API)**: The server calls the client instead of the client calling the server.

**3. Explain the structure of an API request & response.**  
- **Request** includes:  
  - **Endpoint (URL)**  
  - **HTTP Method (GET, POST, etc.)**  
  - **Headers** (e.g., Authorization, Content-Type)  
  - **Body** (for POST/PUT – usually in JSON format)  
- **Response** includes:  
  - **Status Code**  
  - **Headers**  
  - **Body** (usually JSON/XML data or error messages)

**4. What is an API endpoint?**  
An **endpoint** is a specific URL where an API interacts with a resource. Example:  
`GET https://api.example.com/users/123`

---

### ✅ **HTTP Methods & Status Codes**

**1. What are HTTP methods?**  
- **GET** – Retrieve data  
- **POST** – Create new data  
- **PUT** – Replace existing data  
- **PATCH** – Update part of the data  
- **DELETE** – Remove data

**2. What are HTTP status codes?**  
- **200 OK** – Success  
- **201 Created** – Resource successfully created  
- **400 Bad Request** – Client-side input error  
- **401 Unauthorized** – No valid authentication provided  
- **403 Forbidden** – Authenticated but not allowed  
- **404 Not Found** – Resource not found  
- **500 Internal Server Error** – Server-side error

**3. What is an Idempotent API call?**  
An **idempotent API call** is one where making the same request multiple times has the same effect as making it once (e.g., GET, DELETE, PUT).

---

### ✅ **API Authentication & Authorization**

**1. Difference between Authentication & Authorization?**  
- **Authentication** verifies *who* you are (login/token).  
- **Authorization** verifies *what* you can do (permissions/roles).

**2. How does authentication work in APIs?**  
Via:
- **API Keys** – Simple, used in headers or query params  
- **Access Tokens (OAuth)** – User logs in, token is issued  
- **JWT (JSON Web Token)** – Encoded tokens containing user data

**3. What is an API Key? Why is authentication important?**  
An **API Key** is a token used to identify the calling program. Authentication protects resources from unauthorized access and abuse.

**4. Where can you find an API access token in a web application?**  
Tokens can be found in:
- Local Storage
- Session Storage
- Cookies
- JavaScript variables (in SPAs)

**5. How do browsers store and use API tokens?**  
Stored using:
- **Local Storage** (persistent)
- **Session Storage** (tab/session-limited)
- **Cookies** (can be HTTP-only and secure)
Used in **Authorization headers** when making API calls.

**6. What happens when an access token expires? How should an API handle it?**  
Returns **401 Unauthorized**.  
Client should request a **new token using a refresh token**, or prompt login again.

**7. How do you test unauthorized access to an API?**  
- Send a request without a token  
- Use an expired/invalid token  
- Try accessing a restricted resource with a valid token (to test authorization)

---

### ✅ **API Security & Storage**

**1. What is local storage, and how is it related to authentication tokens?**  
**Local Storage** is browser storage that persists across sessions. Often used to store tokens, especially in SPAs.  

**2. What are the security risks of storing tokens in Local Storage?**  
- Vulnerable to **XSS (Cross-Site Scripting)** attacks  
- No protection from malicious scripts accessing tokens

**3. Explain CORS (Cross-Origin Resource Sharing).**  
**CORS** is a browser security feature that restricts web apps from making requests to a different domain unless the server explicitly allows it using response headers (like `Access-Control-Allow-Origin`).

---

### ✅ **API Communication & Rate Limiting**

**1. What is API Rate Limiting? How does it work?**  
**Rate Limiting** restricts how many API calls a client can make in a time window.  
Implemented using:
- Fixed window (e.g., 1000 requests/hour)
- Sliding window
- Token bucket algorithms

**2. How do APIs handle concurrency and rate limits?**  
- Return **429 Too Many Requests** if limits are hit  
- Use headers like `Retry-After` to tell clients when to try again  
- Implement **throttling**, **queuing**, or **caching** to manage load

---