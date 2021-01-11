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
        
             Output:
                - If an IP address is returned then you are on active server. Do not proceed with an active server.
                - If it's not primary, then proceed with next step.
                
     d. GitClone the repo and run the pre-check script
     
      - In Case of Failures Create the Log files & Investigate the logs
      
     e. Hold the MLX Config & MLX Firmware
     
     f. Apply the Patch - Shell Scripts
     
     g. Verify the Kernel Versions
     
     h. Apply Salt Formula to maintain the old routing tables
     
     ![test image size](https://github.com/TejaswiniJayaram/Hello-World/blob/main/img/Dynamic_Inventory.png)
    
    
     ![test image size](https://github.com/TejaswiniJayaram/Hello-World/blob/main/img/Final_reboot.png)
  



