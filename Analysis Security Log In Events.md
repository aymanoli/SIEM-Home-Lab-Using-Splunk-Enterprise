<h1>Analysis Security Log In Events</h1>
<hr></hr>
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

### 1: Searches events in the http_sample index where the file is login.php.

```bash
index="http_sample" file="login.php"
```
### 2: Finds events where the HTTP status code is greater than 200.
```bash
index="http_sample" status>200
```
### 3: Searches events with status code 400 or higher (client/server errors).
```bash
index="http_sample" AND Status>=400
```
### 4: Finds events where the HTTP method is GET or POST. (Usually written as (method=GET OR method=POST).)
```bash
index="http_sample" AND methods=GET OR method=POST
```
### 5: Searches events where the client IP starts with 100. (wildcard matches any remaining octets).
```bash
index="http_sample" clientip=100.*.*.*
```
<img width="1920" height="955" alt="Screenshot From 2026-06-23 09-38-24" src="https://github.com/user-attachments/assets/3b891c36-ce36-4fd7-99ff-b95f3c4992ef" />
