# Web Infrastructure Design:

![Example of web design]()

## Infrastructure:

### Server:
![Example of server]()

A server is a computer (Physical) or computer system (Virtual) that responds to requests from other computers, known as clients. It can provide various services, such as file storage, access to network resources, or website hosting.

Servers can be hosted at:

 - **Data Centers**: Specialized facilities with security measures and redundancies.

 - **Public Clouds**: Offered by providers such as AWS, Azure and GCP, with global infrastructures.

 - **Private Clouds**: Built by organizations for their own needs.

 - **Placement Centers**: Shared space in facilities managed by third parties.

 - **On-Premises Environments**: Servers located in a company's own facilities.

The choice depends on factors such as performance, security and budget, with some companies opting for hybrid strategies.
### Domain Name:
The domain name is a human-readable label that is associated with a unique IP address on the Internet. Its main function is to translate domain names into IP addresses, thus facilitating the identification of resources on the network.

The DNS record for "www" is generally a CNAME (Canonical Alias ​​Name) type record that points to the primary domain name, in this case, "foobar.com."
### Role of Web Server:
![Example of web server]()

A web server is a program that processes HTTP (**H**yper**t**ext **T**ransfer **P**rotocol) requests to serve web pages to users. It handles communication between the client and the server, serving web content and managing interaction.
### Role of Application Server:
![Example of application server]()

Application server is a software component that runs web applications and manages user requests. It can handle business logic, data processing, and cooperate with the web server to deliver dynamic content.
### Role of Data Base:
![Example of Data Base]()

The database stores and organizes data in a structured way. In the web context, it stores information necessary for the application, such as users, content, and settings.
### Communication with the User's Computer:
Communication is carried out through the HTTP/HTTPS protocol. When a user requests a website, the server responds by sending the requested data through this protocol.

## Problems with Infrastructure

 - ### SPOF (**S**ingular **P**oint **O**f **F**ailure):
A SPOF is a single component whose failure can result in the unavailability of the entire system. For example, if there is a single web server and it fails, the entire site could be down.
 - ### Downtime during Maintenance:
During maintenance, such as deploying new code that requires restarting the web server, there may be downtime, affecting the accessibility of the site.
 - ### Scalability Limitations:
The infrastructure may not be able to handle large volumes of traffic. If demand exceeds system capacity, there may be slowness or even inaccessibility of the site.