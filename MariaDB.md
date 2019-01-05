<h4>Here is a guide to setting up and configuring Mariadb on CentOS 7</h4>
<ol>
  <li>Create A CentOS 7 minimal Install</li>
    <ul>
      <li> Be sure to create a non-root user during the installation process that has admin privilges(sudo).</li>
    </ul>
    <li>In the command line, type <b>nmtui</b> then edit the only connection so it has a static IP adddress</li>
    <h5>Since you have CLI, you must use the arrow keys, enter, and spacebar.</h5>
   <ul>
   <li>Select the <b>Edit a connection</b> option.</li>
    <li>Select the only connection</li>
    <li>Arrow down to the <b>IPv4 CONFIGURATION</b> and change <b>Automatic</b> to <b>Manual</b>.</li>
    <li>Arrow over to <b>Show</b> and press <b>Enter</b>.</li>
    <li>Fill in the IP address <b>192.168.2[VM #]/24</b></li>
    <li>Gateway: <b>192.168.1.2</b></li>
    <li>DNS Server: <b>8.8.8.8</b></li>
    <li>Ensure the <b>Automatically connect</b> box is checked then select <b>OK</b> and select <b>Back</b>.</li>
    <li>Arrow down to <b>Set system hostname</b> and name the system whatever you'd like.</li>
    <li>Select <b>OK</b>. In the command prompt, type <b>reboot</b> so the new settings take effect.</li>
    </ul>
</ol>
