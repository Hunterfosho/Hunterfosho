# Secure Design Principles
> ### Secure Design Principles

- Object/Subject Model
    - Subject is someone who is requesting a file from an object
    - Example: A process might request access to a memory location
- Failure Modes
    -  Fail Open - If security controls fail, they are automatically bypassed. This approach favors continued business operations, it poses more security risk  
    -  Fail Closed - If a security control fails, the system locks itself down to a state where no access is granted.
- Isolation
    -  Isolation -Process isolation prevents memory from accessing processes from other programs
    -  Segmentation - prevents network computers in a department from accessing another department in an organization
- Vaildation
    -  Constrain Input -Constraining input is about allowing good data. This is the preferred approach. 
    -  Validate Data for Type, Length, Format, and Range - Use strong type checking on input data wherever possible.
    -  Reject Known Bad Input- Deny "Bad" Data
    -  Sanitize Input- Escape values, stripping a null from a user-supplied string

#### Constraining input may involve setting character sets on the server so that you can establish the canonical form of the input in a localized way.
#### Security is a design element - Bolt on security rarely works

```
If you look back at major security failures over the past decade, many shared a common theme. Some aspect of security was either entirely overlooked or treated as an afterthought after the system design was complete. In this approach known as bolt-on security, security engineers attempt to retrofit an existing system with security features designed to protect confidentiality, integrity, and availability. While this approach is sometimes successful, it is much less effective and much more expensive than simply including security in the design from the start. 
```
# Security Models
> ### Security Models

- Bell-LaPadula Model - Enforces confidentiality 
    -  Simple Security Rule - No "read up"
    -  *-Property - No "write down
- Biba Model - Enforces integrity
    -  Simple Integrity Proterty - No "read down"
    -  *-Integrity Property - No "write up"
- Trusted Computer Security Evaluation Criteria (TCSEC)  
    -  Orange Book - 
    -  Discontinued in 2005  
    -  Common Criteria was introduced
- Certification 
    - Determines that a system meets the security criteria
- Accreditation  
    - Approves use of a system in a specific environment
- Accreditation Decisions
    -  Authorzation to Operate (ATO)
    -  Interm Authorzation to Operate (IATO)
    -  Interim Authorzation to Test (IATT)
    -  Denial of Authorzation to Operate (DATO)

> ### Certfication and accreditation are different
>
> ### Accreditation and authorzation are the same

   # Seperation of Duties
   > ### Seperation of Duties
   
- ### No individual should possess two permissions that, in combonation, allow them to perform a highly sensitive action
    - Account reviews and audits should reduce the risk of privilege creep
    - Information security professionals are often called on to audit separation of duties, and IT staff are often the target
- ### Two-Person Control
  - Requires the authorization of two separate individuals to carry out a sensitive action; also know as dual control
  
 # Selecting Security Controls
> ### Selecting Security Controls
- Security Controls
    - Procedures and mechanisms that an organization puts in place to manage security risks
- Defense in Depth
    -  Multiple overlapping controls for one objective
 > ### Security Control Groups
  - Preventive
    - Stop a security issue from occuring in the first place
-   Detective
    - Identify that a potential security issue has taken place12.  
- Corrective
    - Remediate security issues that already occured
- Deterent 
    -  Prevent an attacker from seeking to violate security policies
- Physical 
    -  Impact the physical world
- Compensating
    - Fill a known gap in a security environment

 > ### Technical Controls
 - Techinical Controls
     -  Use technology to achieve security control objectives
> ### Operational Controls
- Operational Controls
    - Use human-driven processes to manage technology in a secure manner
    
> ### Techincal controls are implemented by technology 
> 
> ### Operational controls are implemented by people
