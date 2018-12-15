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
<strong>gpupdate</strong>
