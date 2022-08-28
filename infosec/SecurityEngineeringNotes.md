# Secure Design Principles
> Secure Design Principles

1.  Object/Subject Model
   
    1.  A Subject is someone who is requesting a file from an object
    ```
    Example: A process might request access to a memory location
    ```

2.  Failure Modes
    1.  Fail Open - If security controls fail, they are automatically bypassed. This approach favors continued business operations, it poses more security risk  
    2.  Fail Closed - If a security control fails, the system locks itself down to a state where no access is granted.
3.  Isolation
    1.  Isolation -Process isolation prevents memory from accessing processes from other programs
    2.  Segmentation - prevents network computers in a department from accessing another department in an organization
4.  Vaildation
    1.  Constrain Input -Constraining input is about allowing good data. This is the preferred approach. The idea here is to define a filter of acceptable input by using type, length, format, and range. Define what is acceptable input for your application fields and enforce it. Reject everything else as bad data.
    2.  Validate Data for Type, Length, Format, and Range - Use strong type checking on input data wherever possible.
    3.  Reject Known Bad Input- Deny "Bad" Data
    4.  Sanitize Input- Escape values, stripping a null from a user-supplied string

Constraining input may involve setting character sets on the server so that you can establish the canonical form of the input in a localized way.

>Security is a design element - Bolt on security rarely works

```
If you look back at major security failures over the past decade, many shared a common theme. Some aspect of security was either entirely overlooked or treated as an afterthought after the system design was complete. In this approach known as bolt-on security, security engineers attempt to retrofit an existing system with security features designed to protect confidentiality, integrity, and availability. While this approach is sometimes successful, it is much less effective and much more expensive than simply including security in the design from the start. 
```


# Security Models
>Security Models

1.  Bell-LaPadula Model - Enforces confidentiality 
    1.  Simple Security Rule - No "read up"
    2.  *-Property - No "write down"
2.  Biba Model - Enforces integrity
    1.  Simple Integrity Proterty - No "read down"
    2.  *-Integrity Property - No "write up"
3.  Trusted Computer Security Evaluation Criteria (TCSEC) - Orange Book - Discontinued in 2005 - Common Criteria was introduced
    1.  Certification - Determines that a system meets the security criteria
    2.  Accreditation - Approves use of a system in a specific environment
        1.  Accreditation Decisions
            1.  Authorzation to Operate (ATO)
            2.  Interm Authorzation to Operate (IATO)
            3.  Interim Authorzation to Test (IATT)
            4.  Denial of Authorzation to Operate (DATO)
   

   Certfication and accreditation are different
   Accreditation and authorzation are the same

   # Seperation of Duties
   >Seperation of Duties

1.  No individual should possess two permissions that, in combonation, allow them to perform a highly sensitive action
