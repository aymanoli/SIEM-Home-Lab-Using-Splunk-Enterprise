<h1>Monitored and Visualize Security Events</h1>
<h2>Upload log file in Splunk</h2>
<ul>
  <li>Go to setings add data</li>
  <li>go to upload section</li>
  <li>select file</li>
  <li>create a new index</li>
  <li>finish the uplod process</li>
  <li>image example</li>
  <img width="1920" height="955" alt="Screenshot From 2026-06-23 09-31-16" src="https://github.com/user-attachments/assets/2fe7b91e-77b9-44b0-baed-5bbb7c49214f" />
</ul>

<hr></hr>

<h2>Monitor with SPL queries</h2>
<p>Use SPL queries to complete the following analysis</p>

##Searches events in the http_sample index where the file is login.php.

```bash
index="http_sample" file="login.php"
```
