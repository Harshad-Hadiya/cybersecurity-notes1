Two types of ports 

1. virtual ports
2. physical ports


| Protocol | Port  | Purpose                                 |            Full FOrm                     |
| -------- | ----- | --------------------------------------- | --------------------------------------   |
| HTTP     | 80    | Unencrypted web traffic                 |  ( Hyper text transfer protocol)         |  
| HTTPS    | 443   | Encrypted web traffic (SSL/TLS)         |   Hyper text transfer protocol secure    |
| FTP      | 21    | File transfer (unencrypted)             |   File transfer protocol                 |
| SFTP     | 22    | Secure file transfer (SSH)              |   Secure file transfer protocol          |
| SSH      | 22    | Secure shell, remote access             |   Secure shell                           |
| Telnet   | 23    | Remote access (unencrypted, deprecated) |   Telecommunications network protocol    |
| DNS      | 53    | Domain name resolution                  |   Domain name system                     |
| DHCP     | 67-68 | Dynamic IP assignment                   |   Dynamic host control protocol          |
| SMTP     | 25    | Send email                              |   simple mail transfer protocol          |
| POP3     | 110   | Receive email (older)                   |   post office protocol version 3         |
| IMAP     | 143   | Receive email (modern)                  |   Internet message access protocol       |
| RDP      | 3389  | Remote desktop (Windows)                |   Remote desktop protocol                |

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

## HTTP Status Codes

Status codes tell you what happened with your request.

| Code Range | Meaning       | Examples                                                            |
| ---------- | ------------- | ------------------------------------------------------------------- |
| 1xx        | Informational | 100 Continue, 101 Switching Protocols                               |
| 2xx        | Success       | 200 OK, 201 Created, 204 No Content                                 |
| 3xx        | Redirection   | 301 Moved Permanently, 302 Found, 304 Not Modified                  |
| 4xx        | Client Error  | 400 Bad Request, 401 Unauthorized, 403 Forbidden, 404 Not Found     |
| 5xx        | Server Error  | 500 Internal Server Error, 502 Bad Gateway, 503 Service Unavailable |


Key Status Codes Breakdown
200 OK
Request succeeded

201 Created
Resource created successfully

301/302
Redirect to new 

400 Bad Request
Malformed request

401 Unauthorized
Authentication required

403 Forbidden
Access denied (found but blocked)

404 Not Found
Resource doesn't exist

500 Internal Server Error
Server misconfiguration/crash

503 Service Unavailable
Server overloaded

