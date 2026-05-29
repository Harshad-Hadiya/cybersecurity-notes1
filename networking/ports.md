Two types of ports 

1. virtual ports
2. physical ports


| Protocol | Port  | Purpose                                 |
| -------- | ----- | --------------------------------------- |
| HTTP     | 80    | Unencrypted web traffic                 |Hyper text transfer protocol
| HTTPS    | 443   | Encrypted web traffic (SSL/TLS)         |Hyper text transfer protocol secure
| FTP      | 21    | File transfer (unencrypted)             |File transfer protocol
| SFTP     | 22    | Secure file transfer (SSH)              |Secure file transfer protocol
| SSH      | 22    | Secure shell, remote access             |Secure shell
| Telnet   | 23    | Remote access (unencrypted, deprecated) |Telecommunications network protocol
| DNS      | 53    | Domain name resolution                  |Domain name system
| DHCP     | 67-68 | Dynamic IP assignment                   |Dynamic host control protocol
| SMTP     | 25    | Send email                              |simple mail transfer protocol
| POP3     | 110   | Receive email (older)                   |post office protocol version 3
| IMAP     | 143   | Receive email (modern)                  |Internet message access protocol
| RDP      | 3389  | Remote desktop (Windows)                |Remote desktop protocol

## HTTP Methods & Headers

| Method  | Purpose                    | Hacker Relevance                                |
| ------- | -------------------------- | ----------------------------------------------- |
| GET     | Fetch data from server     | Parameter tampering, URL manipulation           |
| POST    | Send data to server        | SQLi, login brute force, form injection         |
| PUT     | Update existing resource   | Unauthorized file upload, resource overwrite    |
| DELETE  | Remove resource            | Unauthorized deletion, data destruction         |
| PATCH   | Partial update to resource | Privilege escalation, partial data modification |
| OPTIONS | Check allowed methods      | Recon, discover available endpoints             |


* Request Headers:
Host
User-Agent
Cookie
Authorization
Content-Type
Referer

* Response Headers:
Set-Cookie
Server
Content-Type
X-Frame-Options
Access-Control-Allow-Origin (CORS)
Cache-Control
