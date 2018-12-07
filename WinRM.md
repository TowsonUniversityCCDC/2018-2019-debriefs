<h3> WinRM is another protocol for remote system management. It operates over TCP/5986.
It operates operates over TCP/5985 and TCP/5986. It can be used to execute arbirary 
commands on a target remote system, simlar to PSExec. </h3>

<h5> Enable WinRM via Group Policy</h5>
<h5> Enabling via Group Policy</h5>
<p> on The Domain Controller:
<ul> 
<li> Computer Configuration -> Policies -> Windows Settings -> Security Settings -> Windows Remote 
Management Service </li>
<li> Computer Configuration -> Perferences -> Control Panel Settings -> Services</li>
<li> Add a New Service </li>
  <h6> Use the following settings AND on the Recovery Tab, restart the serfice if it fails.</h6>
  <li> Computer Configuration -> Policies -> Administrative Templates -> Windows COmponents ->
    Windows Remote Management -> WinRM Service </li>
  <h6> Enable the option "ALlow remote server management through WinRM" </h6>
</ul>

