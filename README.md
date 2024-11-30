<p align="center">
<img src="https://i.ibb.co/gR1bdDr/DNS-FIX.jpg" alt="osTicket logo" width="70%"/>
</p>
<h2 align="center">Issue 1: DNS Server Misconfiguration</h2>

<h3>Issue Description:</h3>
The VM cannot resolve domain names, leading to errors when attempting to access external websites (e.g., `ping google.com` fails).

<h3>Cause:</h3>
This issue arises when the DNS server is misconfigured or unreachable, preventing domain name resolution.

<h3>Steps to Fix:</h3>

<h4>Step 1: Identify the DNS Issue</h4>
<p align="center">
  <img src="https://s2.ezgif.com/tmp/ezgif-2-e3924cd854.gif" alt="DNS Resolution Error Before Fix - Pinging google.com"/>
  <br>
  <i>Before Fix: Attempting to ping google.com results in a DNS resolution error (e.g., "Ping request could not find host google.com").</i>
</p>

---

<h4>Steps 2-7: Resolve the DNS Issue</h4>
<p align="center">
  <img src="https://s2.ezgif.com/tmp/ezgif-2-ffad981040.gif" alt="Fixing DNS Server Configuration in Azure"/>
  <br>
</p>
<ol>
  <li>Open the Azure portal and navigate to your VM.</li>
  <li>Go to the <b>Networking</b> section and select the network interface associated with your VM.</li>
  <li>Check and configure the DNS servers:
    <ul>
      <li>Set to Azure Default DNS.</li>
    </ul>
  </li>
  <li>Save the changes and restart the VM.</li>
  <li>Verify the fix by:
    <ul>
      <li>Pinging google.com successfully from the terminal.</li>
      <li>Accessing external websites via a browser.</li>
    </ul>
  </li>
</ol>
<i>After the fix: The DNS resolution and browser access are successful.</i>

---

<h3>Conclusion:</h3>
This process resolves the DNS misconfiguration, allowing the VM to correctly resolve domain names and access external websites, such as Google.
