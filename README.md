## Issue 1: DNS Server Misconfiguration

### Issue Description:
The VM cannot resolve domain names, leading to errors when attempting to access external websites (e.g., `ping google.com` fails).

### Cause:
This issue arises when the DNS server is misconfigured or unreachable, preventing domain name resolution.

---

### Steps to Fix

#### Step 1: Identify the DNS Issue
Before Fix: Attempting to ping `google.com` results in a DNS resolution error (e.g., "Ping request could not find host google.com").

[![Watch the video on DNS Issues](https://img.youtube.com/vi/tG33Rr1cSc4/0.jpg)](https://www.youtube.com/watch?v=tG33Rr1cSc4)

*Click the image or [here](https://www.youtube.com/watch?v=tG33Rr1cSc4) to watch a video demo.*

---

#### Steps 2-7: Resolve the DNS Issue

[![Watch the video on Resolving DNS Issues](https://img.youtube.com/vi/niXR5XyqFR4/0.jpg)](https://www.youtube.com/watch?v=niXR5XyqFR4)

*Click the image or [here](https://www.youtube.com/watch?v=niXR5XyqFR4) to watch a video demo.*

1. Open the Azure portal and navigate to your VM.
2. Go to the **Networking** section and select the network interface associated with your VM.
3. Check and configure the DNS servers:
   - Set to Azure Default DNS.
4. Save the changes and restart the VM.
5. Verify the fix by:
   - Pinging `google.com` successfully from the terminal.
   - Accessing external websites via a browser.

After the fix: The DNS resolution and browser access are successful.

---

### Conclusion:
This process resolves the DNS misconfiguration, allowing the VM to correctly resolve domain names and access external websites, such as Google.
