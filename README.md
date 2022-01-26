# Setup-High-Availability-Load-Balancer-with-HAProxy-to-Control-Web-Server-Traffic
HAProxy which stands for High Availability proxy, is open-source software for TCP and HTTP protocols. Noted for its speed and lightweight framework, it is one of the industry’ most opted load balancers. During high-traffic days such as holidays and festive seasons, hundreds and thousands of concurrent users may end up hitting e-commerce sites like Magento, at such instances, it forms critical to balance the server’s workload. 

# HAproxy configuration and Load balancing
## My Environment Setup
Here our load-balancer HAProxy CentOS7 server having hostname as haproxy with IP address 13.127.113.154

Client Web Servers Setup
I have two CentOS7 VM's, with apache2 installed.

hostname = backend1.example.com IP=13.232.51.126

hostname= backend2.example.com IP=13.233.130.169

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Step 1: Installing Apache on Client Machines

- yum install httpd
Apache has installed open the browser and type the client VM IP=13.232.51.126 and 13.233.130.169


![alt text](https://github.com/rony-james/Setup-High-Availability-Load-Balancer-with-HAProxy-to-Control-Web-Server-Traffic/blob/main/backend1.png?raw=true)

Step 2: Installing HAProxy Server
- yum install haproxy openssl-devel
Install HAProxy on master node 13.127.113.154

Step 3: Configure HAProxy
Open the config file of HAProxy
- vim /etc/haproxy/haproxy.cfg

![alt text](https://github.com/rony-james/Setup-High-Availability-Load-Balancer-with-HAProxy-to-Control-Web-Server-Traffic/blob/main/haproxyconf.png?raw=true)

## Features

- Import a HTML file and watch it magically convert to Markdown
- Drag and drop images (requires your Dropbox account be linked)
