# Creating a New Dashboard
<hr></hr>

## First Dashboard

Keep the existing log file
### 1: Displays the top 5 most frequently accessed URI paths from the http_status index.
```bash
index="http_status" | top limit=5 uri_path
```
### For create a dashboard go to new dash board
<img width="1920" height="955" alt="Screenshot From 2026-06-27 20-46-53" src="https://github.com/user-attachments/assets/75b29d1b-eded-4c95-a976-152070ed1c5b" />
### Give the dashboard and panel title
<img width="1920" height="955" alt="Screenshot From 2026-06-27 20-49-31" src="https://github.com/user-attachments/assets/65ae1194-adb2-43fc-a91c-762ee4f9bff7" />


### 2: Maps client IP addresses to their cities and displays the number of events from each city on a geographic map.
```bash
index="http_sample" 
| iplocation clientip 
| geostats count by City
```
<img width="1920" height="955" alt="Screenshot From 2026-06-27 20-53-18" src="https://github.com/user-attachments/assets/80e31986-c5a3-4ef3-ba8f-3b5d42abb000" />

### To see the dashboard, navigate to the dashboard section
<img width="1920" height="1080" alt="Screenshot From 2026-06-27 20-54-53" src="https://github.com/user-attachments/assets/c305a745-3f95-439b-b7d5-95fec125d425" />

