 OWASP TOP 10
>   [OWASPTop10:2021](https://owasp.org/Top10/)
- The Open Web Application Security Project (OWASP)
  - Maintains a list of common web security issues
- Broken Access Control
  - Allows unauthorized access
    - Broken access control occurs when developers fail to check on the backend whether a user is authorized to access a particular function of an application. Users with knowledge of the application may send requests directly to the server, bypassing the security controls built into the user interface.
- Cryptographic Failure
  - Allows access to sensitive data
    - Cryptographic failures occur when an insecure web application accidentally exposes sensitive information to eavesdroppers because of poorly configured cryptography. This may be as simple as accidentally placing a customer file on a publicly accessible portion of a website without encryption, or it may occur when web server administrators fail to implement the HTTPS protocol to encrypt information that's sent over the internet.
- Injection Flaw
  - Inserts unwanted code
    - Injection flaws occur when an attacker is able to insert code into a request that's sent to a website and then trick that website into passing the code along to a backend server where it's executed.
- Insecure Design
  - Fails to meet security requirements
    - Insecure design traces security issues back to the initial creation of code. It includes issues that arise when an organization does not properly identify and satisfy security requirements, when it conducts insufficient threat modeling, and when it fails to follow security best practices. 

# SQL Injection Attacks
  
  -  SQL is simply the language used by relational databases that allows users and applications to create, update, delete, and retrieve data.
     -   SELECT statement tells the database that we're trying to retrieve information
     -   FROM clause gives the name of the database table containing the desired information. And then the final part of our query
     -   WHERE clause tells the database the specific records that we're interested in retrieving
         -   Entering a SQL query into the username field, then a ; --
             - Single quotes are criticle to SQL injection
             - Input Validation and parameterized queries protect against SQL injection attacks
- Input Validation
  - Protects against unsage user input by checking it on the server before executing commands
- Parameterized SQL
  - Precomplies SQL code on the database server to prevent user input from altering query structure
  
# Cross-Site Scripting Prevention

-  Cross-Site Scripting (XSS)
   -  Cross-site scripting attacks occur when an attacker embeds malicious scripts in a third-party website that are later run by innocent visitors to that site
   -  HTML enhances websites with formmatting and images
- HTML Tags
  - Mark up text with formatting instructions
  -  XSS attackers embed scripts in sites without permission
- Use Input Validation
  - Don't allow script tags in user-supplied input

# Cross-Site Request Forgery (CSRF, XSRF)
-  Cross-Site request forgery attacks leverage the fact that users are often logged into multiple sites at the same time and use one site to trick the browser into sending malicious requests to another site without the users knowledge
   -  Authenticated cookies keep the sessions across browsers
   -  XSRF secretly sends requests
      -  Often using image tags
- Defending Against CSRF
  - Rearchitecting web applications
  - Prevent the use of HTTP GET requests
  - Advise users to log out of sites
  - Automatically log out users after an idle period
- CSRF is a client side attack

# Server-Side Request Forgery
  - Request forgery attack that targets servers, rather than users, by manipulating server into retrieving malicious data from what it believes to be a trusted source 

# Directory Traversal 
- Directory traverasl attacks allows an attacker to manipulate the web server's file structure
  -  Quick facts about the Unix filesystem
     -  . references the current directory
     -  ..references the directory one level higher in the hierarchy
- Directory traversal attacks
  - When an attacker uses directory navigation references to search for unsecured files on a server

# Over Flow Attacks
- Buffer Overflow Attacks
  - Use input larger than the buffer
    - If the developer fails to check that the input provided by the user is short enough to fit in the buffer, a buffer overflow occurs
  - Input validation would be utilized to prevent this issue

# Session Hijacking
- Cookies provide an easy shortcut for web authentication
  - After a user logs into a system, the web server provides a cookie so that the user doesn't need to continuously log into the system, every time they request a new webpage
  
# Privilege Escalation Attack
  - Gains administrative access
    - developers should perform input validation on all input received from end-users. This validation should perform strict checking to ensure that the input is in the expected format and of the correct length. Second, operations team should ensure that the operating systems, platforms, and applications installed on servers are current supported versions and have all of the latest security patches. Third, developers and system engineers should work together to enforce the principle of least privilege. Any service accounts that support code execution should have the minimum set of privileges necessary to support the execution of that code. Granting these service accounts excess privileges can increase the access of an attacker who exploits the code. And finally, IT organizations should take advantage of controls designed specifically to prevent privilege escalation attacks. These include data execution prevention and address space layout randomization technologies