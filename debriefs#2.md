<h5>It's time to start building out a domain controller! Instructions are below!</h5>
<h5>Please change any VM's you've built to the <strong>vmbr01</strong> network</h5>
<ul>

<li> Hardware-> network Devices -> vmbr01</li>
<h4>For the Domain:</h4>
<h5>Create VM</h5>
<li>OS-> Windows 2012 R2</li>
<li>Hardware-> network Devices -> vmbr01</li>
<h4>Keys:</h4>
<h5>Google “Towson Microsoft Imagine”</h5>
<li>https://towson-cis.onthehub.com/WebStore/ProductsByMajorVersionList.aspx?cmi_cs=1&cmi_mnuMain=bdba23cf-e05e-e011-971f-0030487d8897</li>
<h5>Choose Windows Server with GUI Option</h5>
<h5>Choose custom/Install (Not Upgrade)</h5>
<li><h5>System properties (Might be just called "System") -> Change Computer Name to lastName[DC] In System Administrator --> Role based </h5></li>
<h5>Choose Active Directory Domain Services</h5>
<h5>Click "Yes",  Restart automatically when required</h5>
<h5>Promote to DC, name the domain for the Client </h5>
<h6>Make sure your the client is on the same network as the DC</h6>
Hardware-> network Devices -> vmbr01
Point to the DNS server on the DC
Network Interfaces -> Change adapter settings
System properties-> Change Computer Name to lastName[Win7]
System properties -> Use Domain you just created

We will resume meetings after finals. Watch the slack for forthcoming information on remotely attending meetings!
