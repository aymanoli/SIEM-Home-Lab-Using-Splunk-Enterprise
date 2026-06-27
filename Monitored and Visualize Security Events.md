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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic Splunk Search Queries</title>
    <style>
        body{
            font-family: Arial, Helvetica, sans-serif;
            max-width: 900px;
            margin: 40px auto;
            padding: 20px;
            background: #f4f6f9;
            color: #333;
            line-height: 1.6;
        }
        h1{
            text-align: center;
            color: #0f62fe;
        }
        .query{
            background: #fff;
            border-left: 5px solid #0f62fe;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 6px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
        }
        code{
            display: block;
            background: #eef2f7;
            padding: 10px;
            margin-top: 8px;
            border-radius: 4px;
            font-size: 15px;
        }
    </style>
</head>
<body>

<h1>Basic Splunk Search Queries</h1>

<div class="query">
    <h2>1. Search by File Name</h2>
    <p>Searches the <strong>http_sample</strong> index for events where the requested file is <strong>login.php</strong>.</p>
    <code>index="http_sample" file="login.php"</code>
</div>

<div class="query">
    <h2>2. Search HTTP Status Greater Than 200</h2>
    <p>Finds events where the HTTP status code is greater than <strong>200</strong>.</p>
    <code>index="http_sample" status>200</code>
</div>

<div class="query">
    <h2>3. Search Error Responses</h2>
    <p>Displays events with HTTP status codes of <strong>400 or higher</strong>, indicating client or server errors.</p>
    <code>index="http_sample" status>=400</code>
</div>

<div class="query">
    <h2>4. Search GET or POST Requests</h2>
    <p>Finds events where the HTTP request method is either <strong>GET</strong> or <strong>POST</strong>.</p>
    <code>index="http_sample" (method=GET OR method=POST)</code>
</div>

<div class="query">
    <h2>5. Search by Client IP Range</h2>
    <p>Searches for events where the client IP address begins with <strong>100.</strong>.</p>
    <code>index="http_sample" clientip=100.*.*.*</code>
</div>

</body>
</html>
```
