<h1>Denilson-Cisco Packet Tracer Network Design</h1>

<h2>Description</h2>
I used Cisco IOS series 2811 routers to create the network. Fast Ethernet connections with a bandwidth of 100 Mbps are used by these routers. I also utilised WIC-1T module extensions, which allowed for serial DTE connection between routers.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Network configuration (DHC,Ipv4)</b> 

<h2>Environments Used </h2>

- <b>Cisco Packet Tracer</b> 

<h2>Project walk-through:</h2>

<p align="center">
Router Interface Configuration: <br/>
<br />To create the subnets, I followed the instructions in Table 3 above. I set up each router's serial and fast ethernet interfaces, as well as assassignedv4 addresses and subnet masks. For Router0, an example of this setup from Cisco Packet Tracer is shown below<br />

<img src="https://i.imgur.com/TNKUiAA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
DHCP Configuration:  <br/> <br/>The next step was to establish DHCP for IPv4 address allocation after finishing the network design. For each subnet, I utilised each router as the default gateway and hence the DHCP server. As a result, every router had to reply to DHCP queries. In Cisco Packet Tracer, the following screenshot shows how to configure a DHCP pool for Router0:<br/>
<img src="https://i.imgur.com/pkUFlSQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />I set the Gateway/DNS IPv4 for all hosts and servers to DHCP instead of static to finish the DHCP configuration. This allowed IPv4 addresses to be assigned to each subnet automatically. In Cisco Packet Tracer, the following pictures demonstrate the DHCP settings on a computer (PC0) and a server (Server0):<br />

<br/>
<img src="https://i.imgur.com/gt6CHX3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>
<img src="https://i.imgur.com/nl79cVm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />


<br />
RIP Configuration: <br/> <br/> For setting the routing information protocol (RIP) in my network, I used network 192.64.83.0. My routers will use this IPv4 address as the default for numerous subnets in the 192.64.83.x range. My network's RIP configuration enabled connectivity between subnets. The picture below shows an example of RIPv2 (without auto-summary) settings on Router0, taken from Cisco Packet Tracer:<br />
<img src="https://i.imgur.com/Pf1LwBZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Security Configuration:< br/>I created passwords for secure access to my routers through EXEC Mode (Enable), Telnet, Aux Port, and Console Port on all three of my routers. For my network simulation, I utilised password networks. The following is a snapshot of Router1's setup in Cisco Packet Tracer: <br/>
<img src="https://i.imgur.com/0ybJWZu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Running Configuration:  <br/>
Below you can see a summary of the configuration of the routers in respective order:
<br />
<br />
Router 1:  <br/>
<img src="https://i.imgur.com/ZgWZCE6.png?1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Router 2:  <br/>
<img src="https://i.imgur.com/goCJ5hy.png?1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Router 3:  <br/>
<img src="https://i.imgur.com/BwZ3sFN.png?1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Network overview:  <br/>
<img src="https://i.imgur.com/zXdXwtz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Capture the simulation results:  <br/> Now that I've established my network, I need to test it to confirm that it works properly and that data can be exchanged over it. I utilised PDU to test these connections because the target port needed to be supplied.<br/>
<img src="https://i.imgur.com/2vIvlw5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="https://i.imgur.com/d10FgBT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>Evaluate, Analysis and Conclusion<br/> The testing results in the table above demonstrate that not all of the configurations went the way I planned, the calculation was based on the subset table also above, and maybe is due to some IP address not set correct, after following all the steps such as Router Interface, Configuration, DHCP Configuration and RIP Configuration, Security Configuration provided by de Moodle website my testing end up with 6 failures.

In total, 51 devices were used in the design of the network. There are 42 host PCs, three servers, three switches, and three routers among this equipment. Table 4 lists the cables required to link each device in the network and create the six subnets required. There are three of these subnets (A, B and C) 

The other three subnets (D, E, and F) each had a router, switch, server, and several PC devices, whereas the D subnet had no host devices. 
The routers were set up as DHCP servers to assign IPv4 addresses to the host PC and servers in each subnet automatically.
Each router was also set up as a network gateway and configured to utilise RIPv2 with no auto-summary to facilitate communication between subnets. 
Communications between various network devices and ports were examined throughout the simulation. As described in the evaluation above, this allowed the project's objectives specified at the outset to be demonstrated effectively. The network devices were able to interact successfully both inside and across subnets, according to the simulation findings.

<br/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
