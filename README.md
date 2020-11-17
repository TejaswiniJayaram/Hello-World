# Design of Reboot System

## OS Patching:

1. Root Access

2. Establish the connection between different servers
    - Through SSH connection
    - Establish a Passwordless Authentication
    
3. Tasks

    a. Login Action
    
    b. After Login - Switch to ROOT User
    
    
    c. Check for the Server Status if it is Primary or Secondary
        - Primary or Secondary -- Leader Election
        
        - Output:
            - If an IP address is returned then you are on active server. Do not proceed with an active server.
            - If it's not primary, then proceed with next step.



