

## DNS Server Misconfiguration Resolution 

### DNS Server Misconfiguration Fix for Azure VMs

---

### Project Summary 

This project outlines the steps required to fix DNS server misconfigurations on a virtual machine (VM) hosted in Azure. The tutorial walks through identifying the issue, resolving it, and verifying the fix by testing DNS resolution.

- **Languages Used:** None (Instructions and steps)
- **Environments Used:** Azure
- **Technology/Applications/Services Used:** Azure Virtual Machines, Azure Portal

---


The project includes videos demonstrating both the identification of the DNS issue and the resolution process.

- **Video 1:** Demonstrates the issue where `ping google.com` fails due to DNS misconfiguration.  
  ![Watch the video on DNS Issues](https://img.youtube.com/vi/tG33Rr1cSc4/0.jpg)  
  [Click here to watch the video](https://www.youtube.com/watch?v=tG33Rr1cSc4)

- **Video 2:** Shows the steps for fixing the DNS issue, including configuration in the Azure portal and testing the resolution.  
  ![Watch the video on Resolving DNS Issues](https://img.youtube.com/vi/niXR5XyqFR4/0.jpg)  
  [Click here to watch the video](https://www.youtube.com/watch?v=niXR5XyqFR4)

---

### Demonstration 

**Steps to Fix the DNS Issue:**

1. **Identify the DNS Issue**  
   Before the fix, pinging `google.com` results in a DNS resolution error (e.g., "Ping request could not find host google.com").

2. **Resolve the DNS Issue**  
   Follow these steps to fix the DNS configuration:
   - Open the Azure portal and navigate to your VM.
   - Go to the **Networking** section and select the network interface associated with your VM.
   - Check and configure the DNS servers:
     - Set DNS to Azure Default DNS.
   - Save the changes and restart the VM.
   - Verify by pinging `google.com` from the terminal and accessing external websites through a browser.

After these steps, DNS resolution and browser access should work correctly.

---

### Conclusion

By following these steps, the DNS misconfiguration issue is resolved, enabling the Azure VM to properly resolve domain names and access external websites like Google.
