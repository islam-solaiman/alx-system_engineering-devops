# Simple Web Stack

![Alt](https://raw.githubusercontent.com/islam-solaiman/alx-system_engineering-devops/master/0x09-web_infrastructure_design/0-simple_web_stack.png)

# Description

This is a simple web infrastructure that hosts a website that is reachable via www.foobar.com. There are no firewalls or SSL certificates for protecting the server's network. Each component (database, application server) has to share the resources (CPU, RAM, and SSD) provided by the server.

* What is a server ?

A server is a software or hardware device that accepts and responds to requests made over a network. The device that makes the request, and receives a response from the server, is called a client. On the Internet, the term "server" commonly refers to the computer system that receives requests for a web files and sends those files to the client.

* What is the role of the domain name ?

domain name is the location of a website. For example, the domain name "google.com" points to the IP address "216.58.216.164". Generally, it's easier to remember a name rather than a long string of numbers.

* What type of DNS record www is in www.foobar.com ?

www.foobar.com uses an A record.
www.foobar.com is an A record because it resolves to an IP addess.
This can be checked by running dig www.foobar.com.
Note: the results might be different but for the infrastructure in this design, an A record is used.
Address Mapping record (A Record)—also known as a DNS host record, stores a hostname and its corresponding IPv4 address.

* What is the role of the web server ?

A web server is a computer system capable of delivering web content to end users over the internet via a web browser.
Web servers are primarily used to process and manage HTTP/HTTPS requests and responses from the client system.

* What is the role of the application server ?

The application server is a framework, an environment where applications can run, no matter what they are or what functions they perform. An application server can develop and run web-based applications.

* What is the role of the database ?

database is a large quantity of indexed digital information. It can be searched, referenced, compared, changed or otherwise manipulated with optimal speed and minimal processing expense.

* What is the server using to communicate with the computer of the user requesting the website ?

Communication between the client and the server occurs over the internet network through the (TCP/IP) protocol suite.


#  ssues With This Infrastructure


* This server is a SPOF (Single Point of Failure) because nothing is redundant.

There are multiple SPOF (Single Point Of Failure) in this infrastructure.
For example, if the MySQL database server is down, the entire site would be down.

This website would be temporarily down when new code is deployed and the web server needs to be restarted.

* Downtime when maintenance is needed.

When we need to run some maintenance checks on any component, they have to be put down or the server has to be turned off. Since there's only one server, the website would be experiencing a downtime.

* This infrastructure Cannot scale if there's too much incoming traffic.

It will not be able to handle traffic that exceeds the server capacity.
It would be hard to scale this infrastructure becauses one server contains the required components. The server can quickly run out of resources or slow down when it starts receiving a lot of requests.
