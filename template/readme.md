# Summary
You must understand and read  the palo alto AWS Transit Gateway Deployment Guide.The panorama config are generated following the the deployment guide but combine the east west with outbound firewall. Firewalls need to be added to template stacks and assigned with variables manually. You can check the rendered config to see what the actual config are.

# Instruction

## Manual steps required for using this script
1. After creating device group. A commit is required.
2. Devie grouop heiarchy needs to be created manually. A commit is required
3. Onboard firewalls to the appropriate device groups. A commit is required
4. After creating template stacks at the end of the script, firewalls need to be assigned to the appropriate template stack manually. A commit is required.
5. Variables for each *device*, NOT template stack, need to be defined manually and applied 
6. Pre-shared keys for IPSec VPN tunnel needs to be overriden in each template stack manually.
