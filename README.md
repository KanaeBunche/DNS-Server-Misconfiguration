<h2>Issue 1: DNS Server Misconfiguration</h2>

<h3>Issue Description:</h3>
The VM cannot resolve domain names, leading to errors when attempting to access external websites (e.g., `ping google.com` fails).

<h3>Cause:</h3>
This issue arises when the DNS server is misconfigured or unreachable, preventing domain name resolution.

<h3>Steps to Fix:</h3>

<h4>1. Check the DNS Issue: Attempting to Ping Google Without DNS Resolution</h4>
<p align="center">
  <img src="https://s2.ezgif.com/tmp/ezgif-2-e3924cd854.gif" alt="DNS Resolution Error Before Fix - Pinging google.com"/>
  <br>
  <i>Before Fix: Attempting to ping google.com results in a DNS resolution error (e.g., "Ping request could not find host google.com").</i>
</p>

<h4>2. Open the Azure Portal and Navigate to Your VM</h4>
<h4>4. Check and Configure the DNS Servers</h4>
<h4>5. Save the Changes and Restart the VM</h4>
  <i>Save your DNS settings and restart the VM.</i>
<h4>6. Verify the DNS Resolution After the Fix: Ping Google Again</h4>
<h4>7. Verify Browser Access After the Fix</h4>
<p align="center">
  <img src="https://s2.ezgif.com/tmp/ezgif-2-ffad981040.gif" alt="Navigate to Azure VM"/>
  <br>
  <i>In the Azure portal, go to the Networking section of your VM.</i>
</p>

<i>After the fix: Browser successfully loads Google without DNS issues.</i>


<h3>Conclusion:</h3>
This process resolves the DNS misconfiguration, allowing the VM to correctly resolve domain names and access external websites such as Google.
