# HTTP
## What is HTTP?
HTTP is a core operational protocol of the world wide web. It is what enables your web browser to communicate with a web server that hosts a website. HTTP is the communication protocol you use whenever you browse the web. HTTP stands for Hypertext Transfer Protocol. It is a protocol used for transferring web resources such as HTML documents, images, styles, and other files. 

An HTTP request line consists of a method, path, version and headers.

`GET /home.html HTTP/1.1` 

In this example, GET is the HTTP method, /home.html is the resource requested and HTTP 1.1 is the protocol used.

The most commonly used HTTP protocol is Versions 1.1 and 2.0 

## HTTP methods
The primary or the most commonly used HTTP methods are, GET, POST, PUT, and DELETE.

- The GET method is used to retrieve information from the given server. 
- The POST request is used to send data to the server. 
- The PUT method updates whatever currently exists on the web server with something else. 
- The DELETE method removes the resource.

|HTTPS methods|Description|
|-------------|-----------|
|Get|The client requests a resource on the web server.|
|POST|The client submits data to a resource on the web server.|
|PUT|The client replaces a resource on the web server.|
|DELETE|The client deletes a resource on the web server.|

## HTTP request headers
After the HTTP request line, the HTTP headers are followed by a line break. A header is a case-insensitive name followed by a: and then followed by a value.

Common headers are:
```python
Host: example.com
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.9; rv:50.0) Gecko/20100101 Firefox/50.0
Accept: */*
Accept-Language: en
Content-type: text/json
```
The Host header specifies the host of the server and indicates where the resource is requested from.

The User-Agent header informs the web server of the application that is making the request. It often includes the operating system (Windows, Mac, Linux), version and application vendor.

The Accept header informs the web server what type of content the client will accept as the response.

The Accept-Language header indicates the language and optionally the locale that the client prefers.

The Content-type header indicates the type of content being transmitted in the request body.

## HTTP response code
![Response code 1-2](fig/HTTP%20response%20code%201XX-2XX.png)
![Response code 3-4](fig/HTTP%20response%20code%203XX-4XX.png)
![Response code 5](fig/HTTP%20response%20code%205XX.png)

## Other Internet protocols
Hypertext Transfer Protocols (HTTP) are used on top of Transmission Control Protocol (TCP) to transfer webpages and other content from websites.
This reading explores other protocols commonly used on the Internet.

- Dynamic Host Configuration Protocol (DHCP)
You've learned that computers need IP addresses to communicate with each other. When your computer connects to a network, the Dynamic Host Configuration Protocol or DHCP as it is commonly known, is used to assign your computer an IP address.
Your computer communicates over User Datagram Protocol (UDP) using the protocol with a type of server called a DHCP server. The server keeps track of computers on the network and their IP addresses. It will assign your computer an IP address and respond over the protocol to let it know which IP address to use. Once your computer has an IP address, it can communicate with other computers on the network.

- Domain Name System Protocol (DNS)
Your computer needs a way to know with which IP address to communicate when you visit a website in your web browser, for example, meta.com. The Domain Name System Protocol, commonly known as DNS, provides this function. Your computer then checks with the DNS server associated with the domain name and then returns the correct IP address.

- Internet Message Access Protocol (IMAP)
Do you check your emails on your mobile or tablet device? Or maybe you use an email application on your computer?
Your device needs a way to download emails and manage your mailbox on the server storing your emails. This is the purpose of the Internet Message Access Protocol or IMAP.

- Simple Mail Transfer Protocol (SMTP)
Now that your emails are on your device, you need a way to send emails. The Simple Mail Transfer Protocol, or SMTP, is used. It allows email clients to submit emails for sending via an SMTP server. You can also use it to receive emails from an email client, but IMAP is more commonly used.

- Post Office Protocol (POP)
The Post Office Protocol (POP) is an older protocol used to download emails to an email client. The main difference in using POP instead of IMAP is that POP will delete the emails on the server once they have been downloaded to your local device. Although it is no longer commonly used in email clients, developers often use it to implement email automation as it is a more straightforward protocol than IMAP.

- File Transfer Protocol (FTP)
When running your websites and web applications on the Internet, you'll need a way to transfer the files from your local computer to the server they'll run on. The standard protocol used for this is the File Transfer Protocol or FTP. FTP allows you to list, send, receive and delete files on a server. Your server must run an FTP Server and you will need an FTP Client on your local machine. You'll learn more about these in a later course.

- Secure Shell Protocol (SSH)
When you start working with servers, you'll also need a way to log in and interact with the computer remotely. The most common method of doing this is using the Secure Shell Protocol, commonly referred to as SSH. Using an SSH client allows you to connect to an SSH server running on a server to perform commands on the remote computer.
All data sent over SSH is encrypted. This means that third parties cannot understand the data transmitted. Only the sending and receiving computers can understand the data.

- SSH File Transfer Protocol (SFTP)
The data is transmitted insecurely when using the File Transfer Protocol. This means that third parties may understand the data that you are sending. This is not right if you transmit company files such as software and databases. To solve this, the SSH File Transfer Protocol, alternatively called the Secure File Transfer Protocol, can be used to transfer files over the SSH protocol. This ensures that the data is transmitted securely. Most FTP clients also support the SFTP protocol.