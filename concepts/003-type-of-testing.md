# Type of Testing 

### **1. Manual Testing**
- **Definition**: Testing is done manually by a human without the help of automation tools.
- **Example**: A tester manually navigates through a website to see if links work, forms submit, and pages load correctly.

### **2. Automation Testing**
- **Definition**: Testing is performed using automation tools or scripts, helping to reduce manual efforts and speed up repetitive testing.
- **Example**: Using tools like Selenium or JUnit to run predefined test cases for a website automatically.

---

### **Types of Testing by Approach**

#### **A. White Box Testing**
   - **Definition**: Involves testing the internal structure or workings of an application. Testers need knowledge of the code to perform this.
   - **Example**: Testing the logic of code, checking whether loops, conditionals, or branches work as expected.

#### **B. Black Box Testing**
   - **Definition**: Testing the software without knowledge of its internal code or structure. Focuses only on inputs and outputs.
   - **Example**: Testing a login form by entering various usernames and passwords to see if access is granted or denied correctly, without knowing the code behind it.

#### **C. Grey Box Testing**
   - **Definition**: A combination of both White Box and Black Box Testing. The tester has partial knowledge of the internal workings of the software and performs testing with this understanding.
   - **Example**: A tester might know how a database is structured and test how well the application interacts with the database.

---

### **Categories of Software Testing**

#### **1. Functional Testing**
   - **Definition**: This type of testing verifies that the software behaves according to the specified functional requirements.
   - **Example**: Ensuring that when a user clicks the "submit" button on a form, the data gets processed correctly.

   Types of Functional Testing:
   - **Unit Testing**: Tests individual components or pieces of code (e.g., a single function or method).
     - *Example*: Testing if a function that adds two numbers returns the correct sum.
   
   - **Integration Testing**: Checks if different modules or components work together correctly.
     - *Example*: Testing if the login system correctly communicates with the database to fetch user information.
   
   - **System Testing**: Tests the complete system as a whole to ensure it meets the requirements.
     - *Example*: Testing the entire e-commerce application to ensure users can browse products, add items to the cart, and successfully complete a purchase.

   Integration Testing Techniques:
   - **Top-Down**: Testing starts from the top (high-level components) and moves down to the lower-level components.
     - *Example*: Testing the user interface first and then the deeper backend systems.
   
   - **Bottom-Up**: Testing starts from the bottom (low-level components) and moves upward.
     - *Example*: Testing individual services or databases first before moving on to the user interface.

#### **2. Non-Functional Testing**
   - **Definition**: Focuses on how the system works (performance, usability, etc.) rather than what the system does.
   - **Example**: Ensuring a website loads within 2 seconds under heavy traffic.

   Types of Non-Functional Testing:
   - **Performance Testing**: Measures how well the software performs under a certain workload.
     - *Example*: Testing if the website still functions properly when 10,000 users are accessing it simultaneously.
   
   - **Usability Testing**: Focuses on how user-friendly the software is.
     - *Example*: Testing how easy it is for new users to sign up for an account on a website.
   
   - **Compatibility Testing**: Ensures the software works across different platforms, devices, and browsers.
     - *Example*: Testing a website on different operating systems (Windows, Mac, Linux) and different web browsers (Chrome, Firefox, Safari).

   Types of Performance Testing:
   - **Load Testing**: Simulates heavy user activity to check how the system behaves under normal and peak loads.
     - *Example*: Testing an e-commerce site during Black Friday sales to see if it can handle a surge in traffic.
   
   - **Stress Testing**: Pushes the system beyond its normal limits to see how it behaves under extreme conditions.
     - *Example*: Forcing a website to handle more traffic than it was designed for to see if it crashes gracefully.
   
   - **Scalability Testing**: Checks how well the software can scale up in terms of load or usage.
     - *Example*: Testing if a cloud-based service can efficiently handle an increasing number of users without performance degradation.
   
   - **Stability Testing**: Ensures the software remains stable and performs reliably over a long period of time.
     - *Example*: Running an application for 24 hours non-stop to see if it remains stable and free of crashes.

---

### Summary of the Diagram:
- **Manual Testing**: Performed by humans without automation tools.
- **Automation Testing**: Performed using scripts and tools to automate repetitive tasks.
  
**Testing Methods:**
- **White Box**: Internal structure and code logic are tested.
- **Black Box**: Focuses only on inputs/outputs without knowing the code.
- **Grey Box**: Partial knowledge of the system is used.

**Functional Testing** ensures features work as required, while **Non-Functional Testing** ensures performance, usability, and stability under different conditions.
