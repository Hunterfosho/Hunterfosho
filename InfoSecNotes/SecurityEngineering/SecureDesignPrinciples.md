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
    -  Are implemented by technology
> ### Operational Controls
- Operational Controls
    - Use human-driven processes to manage technology in a secure manner
    - Are implemented by people

> #### Management Controls
- ### Management Controls
  - Improve the security of the risk maangement process it self 

# Privacy by Design
> ### Privacy by Design
- Privacy by Design
  - Seek to incorporate strong privacy practices into the design and implementation of technology systems
  - Not bolt on privacy controls for systems already in place  
  - Better privacy
  - reduced reworks
- Privacy Design Principles
  - Proactive, Not Reactive; Preventive, Not Remedial
    - Systems should be designed to prevent privacy risk from occuring in the first place
  - Privacy by The Default Setting
    - Sytems should should protect the privacy of idividuals, even if the individuals don't take direct action
  - Privacy Embedded into Design
    - Privacy should not be a bolt on after thought, privacy is a core requirement of all systems
  - Full Functionaliity; Positive Sum, Not Zero Sum
    - Privacy should not be treated with trade offs with the business, security or other objectives
  - End to End Security
    - Full lifecycle, security practices should persist throughout the entire information lifecycle 
  - Visibility and Transparency; Keep it Open
    - The component parts of systems preserving privacy by design should be open for inspection by users and providers alike.
  - Respect for user privacy: keep it user centric. 
    - Privacy is about protecting personal information and personal information belongs to individual people. 
  
# Secure Defaults
> ### Secure Defaults
- Secure Defaults
    - The secure default principle simply says that the system we design should default to a secure mode if we don't do anything else
- KISS method- Keep it simple; stupid
    - The princple states that when you are designing potentially complex system, we should always err on the side of simplicity
- Zero Trust Model
    - ztna applies the long standing principle of least privilege to network access.  
    - ztna changes the way we think about trust in our past architecture
    - ztna states that no use or device should be granted access to resources based solely upon their location on the network
- Trust but Verify
  - trust but verify is a bedrock practice of security professionals. Yes, we want to be able to trust all of our coworkers, business partners, customers, and outsiders, but that's simply not a reasonable security practice. Malicious insiders are a real risk as are other bad actors, and we need to be sure to verify that security rules are indeed being followed. This is true whether you're enforcing internal security policies, verifying that a partner is carrying out their own security obligations, or checking the work of your own team. Trust that they did the work well, but verify that it is implemented correctly.
  
  
  