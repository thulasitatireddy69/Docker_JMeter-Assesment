# HttpBin-Docker_JMeter-Assesment
# Overview

This performance test evaluates the responsiveness, reliability, and resource efficiency of the HTTPBin API hosted in a Docker environment.
The setup simulates concurrent user activity for the following API sequence executed on port 8080:

HTTP Method	Endpoint	Description
GET	/get	Fetch request validation
POST	/post	Data submission test
GET	/get	Revalidation after post

# Key Performance Indicators (KPIs)
# KPI	Description	Target/Threshold
Average Response Time	Mean time to process a request	≤ 1 sec
Error Rate	Failed requests	≤ 1%
CPU Utilization	Container CPU usage	≤ 75%
Memory Utilization	RAM usage under load	≤ 70%

# Environment & Assumptions

HTTPBin container hosted on Docker port 8080.

Stable network and no background load during testing.

Each virtual user generated independent requests (no caching).

JMeter configured for remote optimization with sufficient CPU and memory resources.

 # Access Dashboards:

HTTPBin → http://localhost:8080

# Benefits:

Allocated sufficient memory for Docker containers.

Enabled localhostForwarding for seamless communication between JMeter and HTTPBin.

Improved throughput consistency and reduced GC (Garbage Collection) delays.

# Next Steps

Integrate with Jenkins for automated execution and reporting.
