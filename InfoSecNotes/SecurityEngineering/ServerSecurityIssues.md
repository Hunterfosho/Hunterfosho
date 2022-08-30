### Server Security Issues
- Data Flow Control
  - Data flow control manages the transfer of information to and from your servers
  - All servers are affected by data flow control
  - Database servers must be protected from aggregation, inference, and other database attacks
  - Administrators must take steps to ensure that data flow doesn't become high enough in volume that it overwhelms the available bandwidth of either the server or the network
    - Controlling bandwidth consumption
vers      - Use network devices and server operating systems
  - System architects carefully map out and understand how data flows within their systems paying particular attention to sensitive information
    - understand senstive date flows
      - Use data flow maps to apply controls appropriately
  - Cyber security professionals must apply rigorous security controls to environments that handle that sensitive information
  
### Database Focused Attacks
- Aggregation
  - Occurs when an individual with a low level security clearance is able to put together facts available at that low level to determine a very sensitive piece of information that they should not have access to.
- Inference
  - Occurs when individuals can figure out sensitive information from facts available to them

### NoSQL Databases
-  Relational databases rely on SQL to manage data from tables
-  NoSQL databases do not require as much over head by implementing key value stores
   - Like a filing cabinet that stores value using a key, values are later reterived using that key
   - Very popular with web applications because of the speed
   - Each key may have a different structure value

### Distributed and High Performace Computing
-  Client/Server Model
    -   Web Brower request data from company website
- Large-Scale Parallel Data
    -   Exetremely large data sets and processing power that can't be handled by a single server, or set of servers
        -   Problems like this are divided into pieces and handled by distributed computing systems

### Grid Computing
- Assembles the unused processing capability of many computers at different locations to form a virtual supercomputer with a centrialized controller

### Peer-to-Peer (P2P) Computing
- Assembles a diverse network of systems to offer a computin gservioce without the need for a centrialized controller
  - P2P nodes all have equal importance on the network
    - P2P Examples
      - BitTorrent- Provides content distribution serivces
      - Bitcoin- Offers anonymous financial tranactions
      - Tor- Offers anonymous internet browsing

### P2P Security Concerns
- Untrusted participants in the P2P network may gain access to sensitive information
- P2P Participants may lose control of their computer systems to malicious P2P agents
- P2P nodes may find themselves the targets of law enforcement investigations