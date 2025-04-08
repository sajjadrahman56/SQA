## **INTRODUCTION TO DEFECT MANAGEMENT**

1. **Defect:**  
   - A defect is a deviation from the expected result found during the development phase.  
   - **Example:** A developer writes a login function, but the "Forgot Password" link does not work as expected. This is identified in development and fixed before testing.

2. **Bug:**  
   - A bug is an issue identified during the testing phase by testers. It is an informal term for a defect.  
   - **Example:** A tester finds that clicking the "Submit" button on a form does not save the user’s input, even though it should.

3. **Error:**  
   - An error occurs when a developer makes a coding mistake that prevents the program from running.  
   - **Example:** A syntax mistake in the code causes the application to crash when trying to start.

4. **Failure:**  
   - A failure happens when an issue reaches the end-user after deployment and affects real-world functionality.  
   - **Example:** A banking app incorrectly calculates interest for users after release, causing financial loss.


## **WHY DO SOFTWARE BUGS OCCUR ?** 

_Miscommunication or not clear requirements_

### **1. Miscommunication or unclear requirements**  
**Definition:** When requirements are not clearly communicated between stakeholders, developers, and testers, leading to incorrect or incomplete implementation.  
**Example:** A client asks for a “simple” search bar, but developers implement an advanced filtering system that is unnecessary.  

### **2. Software complexity**  
**Definition:** As software becomes more complex, unforeseen interactions between components can introduce bugs.  
**Example:** A banking application with multiple modules (transactions, loans, accounts) may have integration issues when new features are added.  

### **3. Programming errors**  
**Definition:** Mistakes in writing code, such as syntax errors, logical mistakes, or incorrect data handling.  
**Example:** A developer accidentally writes `=` instead of `==`, leading to incorrect condition checks and unexpected behavior.  

### **4. Changing requirements**  
**Definition:** When requirements change in the middle of development, previously implemented features may break.  
**Example:** A project initially required a single-page web app, but later the client requests a multi-page application, causing major redesigns and new bugs.  

### **5. Time pressures**  
**Definition:** Tight deadlines force developers to rush coding and testing, increasing the risk of defects.  
**Example:** A startup rushes to release a new feature before a product launch, skipping testing, leading to a broken checkout system.  

### **6. Poorly documented code**  
**Definition:** When developers do not properly document their code, future updates and debugging become difficult.  
**Example:** A new developer joins a project but struggles to understand the logic behind a function due to a lack of comments and documentation.  

### **7. Improper test environment setup**  
**Definition:** When the testing environment does not accurately replicate the production environment, undetected issues may arise.  
**Example:** A website works fine on the test server but fails in production because the database configuration is different.  

### **8. Frequent release of software patches without proper testing**  
**Definition:** Rapid updates and fixes are deployed without thorough testing, introducing new bugs.  
**Example:** A quick fix for a login issue accidentally breaks the password reset functionality.  

### **9. Insufficient time for regression testing**  
**Definition:** When not enough time is allocated to test existing features after new changes, old functionalities may break.  
**Example:** A mobile app update introduces a new chat feature, but existing push notifications stop working due to a lack of regression testing.  

### **10. Low priority assigned to test execution**  
**Definition:** When testing is not given enough importance, critical bugs may go unnoticed.  
**Example:** A company prioritizes adding new features over fixing existing bugs, leading to unstable software releases.  
