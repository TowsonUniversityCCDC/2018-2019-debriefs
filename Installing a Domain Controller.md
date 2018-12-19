<h3>Here is the guide to how to install a Domain controller using Windows Server 2012</h3>
<h4>Prerequists:</h4>
<ul>
<li>A Valid Windows Server 2012 Product Key.</li>
<li>A basic configured VM.</li>
</ul>
<h4>Version to use (when getting the product key)</h4>
<ul><li>Windows Server 2012 R2 Standard with Update 64-bit (English) - Microsoft Image.</li></ul>
<h4>Start the VM</h4>
<h4>Initial Installation</h4>
<ul>
<li>Click Next</li>
<li>Click Install Now</li>
<li>Input Product Key aquired from Microsoft Imagine</li>
<li>Select "Server with a GUI"</li>
<h5>Please Note: This isn't the default option!If you don't select this, you will have a
server that is only accessible by command prmpt. You will have no Graphical User Interface.</h5>
<li>Accept the license term</li>
<li>Select "Custom: Install Windows Only (advanced)"</li>
<li>Click Next</li>
<h5>Now windows will take a little while to install and configure itself so all you can do is wait</h5>
</ul>
<h4>Initial Setup</h4>
<ul>
<li>Choose an Administrator Password</li>
<h5>Use a unique password that you haven't used elsewere.</h5>
<h5> Please write this password down so you can remember it. It is highly recommended to write this down 
in the VM's Notes on Proxmox (under the summary tab).</h5>
<h5>There is no reason to keep these credentials secret. This is a collaborative lab environment and this is
on of the main points of using proxmox</h5>
<li>Click Finish</li>
<h5>In order for you to use the keys "Ctrl+alt+del" in your VM, you have to click the button with the 4 blocks with an
arrow pointing down and you will see an option called "Ctrl+alt+del".</h5>
</ul>
<h4>Set a Static IP address</h4>
<ul>
<li>Right click on "Network" in the task bar</li>
  <li>Open Network And Sharing Center</li>
  <li>Click Change adapter Setting</li>
  <li>Right click on Ethernet</li>
  <li>Select properties</li>
  <li>Click "Internet Protocol Version 4 (TCP/IPv4)"</li>
  <li>Click Properties</li>
  <h5>Use the following settings:</h5>
  <li>IP address: 192.168.2.[The ID Number of your VM]</li>
  <li>Subnet Mask: 255.255.0.0</li>
  <li>Default Gateway: 192.168.1.2</li>
  <li>Preferred DNS Server: 8.8.8.8</li>
</ul>
<h4>Click Add Roles and Features from the Server Manager Dashboard</h4>
<ul>
<li>Click Next</li>
  <li>Select Role based or feature based installation, click next</li>
  <li>Leave the default server selection, click next</li>
  <h4>Server Roles</h4>
  <li>Click Active Directory Domain Services</li>
  <li>Click Add Features</li>
  <li>Click Next</li>
  <li>Click Next twice (landing on the confirmation page)</li>
  <li>Click "Restart the Destination Server automatically if required"</li>
  <li>Install</li>
  <li>Close</li>
</ul>
<h4>Click the Yellow Notifications Flag at the Top Right of the screen</h4>
<ul>
<li>Click promote this Server to a Domain Controller</li>
  <li>Select Add a New Forest</li>
  <li>Name your domain:</li>
  <h5>We recommend: [yourlastname].domain</h5>
  <li>Enter your DSRM password</li>
  <h5>This can be used to boot the Domain Controller in Safe Mode</h5>
  <h5>We recommend either use the same as your administrator password,
    or record your choice in the notes.</h5>
  <li>You will get the following warning:</li>
<h5>"A delegation for this DNS server cannot be created because the 
  authoritative parent zone cannot be found or it does not run Windows DNS server."</h5>
  <li>Click Next</li>
  <li>Wait for the NetBIOS name field to populate, then click next.</li>
  <li>Click next twice</li>
  <li>Install</li>
</ul>
  <h6>Now you are done.</h6>
