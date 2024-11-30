<h2>Issue 1: DNS Server Misconfiguration</h2>

<h3>Issue Description:</h3>
The VM cannot resolve domain names, leading to errors when attempting to access external websites (e.g., `ping google.com` fails).

<h3>Cause:</h3>
This issue arises when the DNS server is misconfigured or unreachable, preventing domain name resolution.

<h3>Steps to Fix:</h3>

<h4>1. Check the DNS Issue: Attempting to Ping Google Without DNS Resolution</h4>
<p align="center">
  <img src="https://example.com/screenshot-before-fix-ping.png" alt="DNS Resolution Error Before Fix - Pinging google.com"/>
  <br>
  <i>Before Fix: Attempting to ping google.com results in a DNS resolution error (e.g., "Ping request could not find host google.com").</i>
</p>

<h4>2. Open the Azure Portal and Navigate to Your VM</h4>
<p align="center">
  <img src="https://example.com/screenshot-azure-portal.png" alt="Navigate to Azure VM"/>
  <br>
  <i>In the Azure portal, go to the Networking section of your VM.</i>
</p>

<h4>3. Go to the Networking Section and Select the Network Interface</h4>
<p align="center">
  <img src="https://example.com/screenshot-network-interface.png" alt="Select Network Interface"/>
  <br>
  <i>Click on the Network Interface associated with your VM.</i>
</p>

<h4>4. Check and Configure the DNS Servers</h4>
<p align="center">
  <img src="https://example.com/screenshot-dns-settings.png" alt="DNS Server Settings in Azure"/>
  <br>
  <i>Ensure the DNS server is set to Azure Default DNS: `168.63.129.16` or a valid custom DNS server.</i>
</p>

<h4>5. Save the Changes and Restart the VM</h4>
<p align="center">
  <img src="https://example.com/screenshot-restart-vm.png" alt="Restart VM"/>
  <br>
  <i>Save your DNS settings and restart the VM.</i>
</p>

<h4>6. Verify the DNS Resolution After the Fix: Ping Google Again</h4>
<p align="center">
  <img src="https://example.com/screenshot-after-fix-ping.png" alt="Successful DNS Resolution After Fix - Pinging google.com"/>
  <br>
  <i>After the fix: Pinging google.com now works successfully, showing a response from Google.</i>
</p>

<h4>7. Verify Browser Access After the Fix</h4>
<p align="center">
  <img src="https://example.com/screenshot-browser-success.png" alt="Successful Browser Search After Fix"/>
  <br>
  <i>After the fix: Browser successfully loads Google without DNS issues.</i>
</p>

<h3>Conclusion:</h3>
This process resolves the DNS misconfiguration, allowing the VM to correctly resolve domain names and access external websites such as Google.
