<h3> Here is the guide to configure and use SMB </h3>
<h5> Prerequisites:</h5>
<ul> 
  <li>RUnning Domain Controller (DC) with Active Directory (AD)</li>
  <li>Windows Workstation (any version of normal Windows Desktop) joined on your domain </li>
  <li> At least one domain user account in AD</li>
</ul>

<h5>Enable Server Message Block SMB via Group Policy:</h5>
<h5>Firewall Rules</h5>
<h6>Enable connections over TCP/445</h6>
<ul>
<li> Computer Configuration -> Policies -> Windows Settings -> Security Settings -> Windows Firewall with 
Advanced Security -> Windows Firewall with Advanced Security (again) -> Inbound Rules</li>
<li>Right Click -> Create New Rule</li>
<li>Select Port -> TCP/445</li>
<li>Name the rule and apply to the Organizational Unit (OU) containing your Windows Workstation</li>
</ul>
<b>Note:</b> 
<h6>Group Policy is applied to domain members at a specific time interval.
To force an update on a particular workstation, run the command:</h6>
<b>gpupdate</b>
<h5>Challenges:</h5>
<ul> 
  <li> Copy a file with SMB </li>
  <li> From your Windows Workstation (not you Domain Controler), log into your domain using your Domain Administrator account.</li>
  <li>Open a command prompt and copy the .txt file from your Domain Controller onto your Local Windows Workstation.</li>
</ul>
<h6>You will need the commands:</h6>
<ul> 
 <li><b>dir</b></li>
 <li><b>copy</b></li>
 </ul>
 <h6>With SMB enabled, you will have remote access to the file system of any domain members.</h6>
 <h6> To designate a filepath on the remote machine, use the following syntax:</h6>
 <b>\\[nameOfRemoteSystem]\c$\[filePathYouWant]</b>
 <ul>
  <li>Add a new Domain User</li>
  <li>You will need the command:</li>
  <b>net user</b>
  <li> Confirm that the new user appears in the AD.</li>
</ul>
