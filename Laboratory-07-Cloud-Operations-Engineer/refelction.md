# Mission Reflection

This laboratory helped me understand the importance of monitoring both the server and the applications running on it. Even if a container is working properly, the host server still needs enough CPU, memory, and disk space to support the application. Checking the host resources gives an early indication of possible problems before they affect users.

If a user complains that they cannot access a web application, the docker logs command can help identify what happened. The logs show the requests received by the application and the status codes returned by the server. In this activity, the successful requests returned HTTP 200, while the request for the missing page returned HTTP 404. This makes it easier to determine if the problem is related to a missing page or another application issue.

Logs and metrics provide different types of information. Logs show events and requests that happened inside the application. Metrics show numerical information about resource usage, such as CPU and memory consumption. Both are useful because logs help explain what happened, while metrics help show how the system is performing.

Large companies cannot manually check every container one at a time because they may operate thousands of containers. They can use monitoring tools such as Prometheus and Grafana to collect, organize, and display information from many systems.

My ability to troubleshoot Linux environments improved because I practiced commands for checking system resources, running containers, testing web services, reading logs, and monitoring container performance. I learned that monitoring is an important part of keeping cloud applications reliable and available.
