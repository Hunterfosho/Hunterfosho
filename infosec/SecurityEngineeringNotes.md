# Security Engineering Principles
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
4.  Vaildation

>Security is a design element - Bolt on seecurity rarely works

```
If you look back at major security failures over the past decade, many shared a common theme. Some aspect of security was either entirely overlooked or treated as an afterthought after the system design was complete. In this approach known as bolt-on security, security engineers attempt to retrofit an existing system with security features designed to protect confidentiality, integrity, and availability. While this approach is sometimes successful, it is much less effective and much more expensive than simply including security in the design from the start. - Mike Chapple (CISSP 9th Edition-SyBEX)
```

