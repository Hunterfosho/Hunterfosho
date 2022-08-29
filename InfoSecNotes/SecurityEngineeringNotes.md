# Secure Design Principles
> Secure Design Principles
```
    1.  Object/Subject Model
    
        1.1  A Subject is someone who is requesting a file from an object
        ```
        Example: A process might request access to a memory location
        ```

    2.  Failure Modes
        2.1  Fail Open - If security controls fail, they are automatically bypassed. This approach favors continued business operations, it poses more security risk  
        2.2  Fail Closed - If a security control fails, the system locks itself down to a state where no access is granted.
    3.  Isolation
        3.1  Isolation -Process isolation prevents memory from accessing processes from other programs
        3.2  Segmentation - prevents network computers in a department from accessing another department in an organization
    4.  Vaildation
        4.1  Constrain Input -Constraining input is about allowing good data. This is the preferred approach. 
        4.2  Validate Data for Type, Length, Format, and Range - Use strong type checking on input data wherever possible.
        4.3  Reject Known Bad Input- Deny "Bad" Data
        4.4  Sanitize Input- Escape values, stripping a null from a user-supplied string

    Constraining input may involve setting character sets on the server so that you can establish the canonical form of the input in a localized way.
```

>Security is a design element - Bolt on security rarely works

```
If you look back at major security failures over the past decade, many shared a common theme. Some aspect of security was either entirely overlooked or treated as an afterthought after the system design was complete. In this approach known as bolt-on security, security engineers attempt to retrofit an existing system with security features designed to protect confidentiality, integrity, and availability. While this approach is sometimes successful, it is much less effective and much more expensive than simply including security in the design from the start. 
```


# Security Models
>Security Models
```
    1.  Bell-LaPadula Model - Enforces confidentiality 
        1.1  Simple Security Rule - No "read up"
        1.2  *-Property - No "write down"
    2.  Biba Model - Enforces integrity
        2.1  Simple Integrity Proterty - No "read down"
        2.2  *-Integrity Property - No "write up"
    3.  Trusted Computer Security Evaluation Criteria (TCSEC) - Orange Book - Discontinued in 2005 - Common Criteria was introduced
        3.1  Certification - Determines that a system meets the security criteria
        3.2  Accreditation - Approves use of a system in a specific environment
            3.3  Accreditation Decisions
                3.3.1  Authorzation to Operate (ATO)
                3.3.2  Interm Authorzation to Operate (IATO)
                3.3.4  Interim Authorzation to Test (IATT)
                3.3.5  Denial of Authorzation to Operate (DATO)


   Certfication and accreditation are different

   Accreditation and authorzation are the same
```

   # Seperation of Duties
   >Seperation of Duties
   ```
    1.  No individual should possess two permissions that, in combonation, allow them to perform a highly sensitive action
        1.1  Account reviews and audits should reduce the risk of privilege creep
        2.2  Information security professionals are often called on to audit separation of duties, and IT staff are often the target
    2. Two-Person Control
        2.1  Requires the authorization of two separate individuals to carry out a sensitive action; also know as dual control
```

# Selecting Security Controls
>Selecting Security Controls
```
    1.  Security Controls- Procedures and mechanisms that an organization puts in place to manage security risks
    2.  Defense in Depth-  Multiple overlapping controls for one objective
```
# Security Control Groups
```
    1.  Preventive- Stop a security issue from occuring in the first place
    2.  Detective-  Identify that a potential security issue has taken place
    3.  Corrective- Remediate security issues that already occured
    4.  Deterent-   Prevent an attacker from seeking to violate security policies
    5.  Physical-   Impact the physical world
    6.  Compensating- Fill a known gap in a security environment
```

>Technical Controls
```
    Use technology to achieve security control objectives
```
>Operational Controls
```
    Use human-driven processes to manage technology in a secure manner
```
Techincal controls are implemented by technology; operational controls are implemented by people.
```








