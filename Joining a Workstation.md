<h3>Here is the guide to joining a workstation to your domain</h3>
<h4>Prerequisits</h4>
<ul><li>A configured Windows 10 (Not N edition) VM with a valid key</li></ul>
<h4>Networking Setttings</h4>
<ul>
<li>Right Click on Nertwork in Taskbar</li>
<li>Open Network & Internet Settings</li>
<li>Change Adapter Options</li>
<li>Select Properties</li>
<li>Select IPv4</li>
<li>Click Properties</li>
</ul>
<h4>Use the Following Settings</h4>
<ul>
<li>IP Address: 192.168.2.[VM ID]</li>
<li>Subnet Mask: 255.255.0.0</li>
<li>Default Gateway: 192.168.1.2</li>
<li>DNS Server: The IP address of the DC you're attemping to join.</li>
<li>Click Ok</li>
</ul>
<h4>Join the Domain</h4>
<ul>
<li>Open File Explorer</li>
<li>Find the tab "This PC"</li>
<li>Right Click -> Properties</li>
<li> Go to "Computer Name, Domain, and Workgroup Settings"</li>
<li>Select Domain</li>
<li>Enter the name of your domain</li>
<li>Click ok</li>
</ul>
<h5>Restart Your System</h5>
