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
<
