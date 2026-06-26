<h1>Installation and Configuration Splunk</h1>
<h2> Objectives</h2>
In this module, install both systems and configure Splunk on an Ubuntu machine.
<hr>
</hr>

<h1> SOC Lab Setup Required </h1>
Download all of this in your host system
<ul>
  <li>Virtual Box</li>
  <li>Unbuntu Linux System</li>
  <li>Windows System</li>
</ul>
<hr>
</hr>

<h1>Configured Splunk Enterprise</h1>
Here, the Splunk download is in the Ubuntu system for centralized log monitoring.
<h2>Step by Step</h2>
<ul>
<li>Downlod Splunk Enterprise from website</li>
<li>Extract it by this command</li>
<code>sudo tar xvfz <splunk file name> -C /opt </code>  
<img width="1920" height="955" alt="Screenshot From 2026-06-23 09-08-42" src="https://github.com/user-attachments/assets/6631c1c5-a754-4a2e-8b53-ede2467bb88e" />
<li> Navigate the path and use the command below </li>
<code>sudo ./splunk --accept-license</code>
<img width="1920" height="955" alt="Screenshot From 2026-06-23 09-12-59" src="https://github.com/user-attachments/assets/cea7f431-f047-423b-8254-7c567a0030dc" />
<li>Open browser and search with your machine ip <mechineip:8000></li>
<li>And login your Splunk system</li>
  <img width="1920" height="955" alt="Screenshot From 2026-06-23 09-15-38" src="https://github.com/user-attachments/assets/ed5d3958-f976-4f66-9abb-1d48a498154b" />
</ul>
<hr>
</hr>
  
<h1>Set up Splunk Universal Forwarder</h1>
<p> Now you go to your Windows machine and download the Splunk universal forwarder from your browser and install the software in your Windows system as like other installation software. <strong> In the installation process, they asked for your machine IP, then you put here your Ubuntu system IP for forwarding the logs and events to your Ubuntu system.</strong> </p>
