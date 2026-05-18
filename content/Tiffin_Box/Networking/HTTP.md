---
tags:
  - basic
  - networking
---
HTTP stands for **Hyper Text Transfer Protocol**. It is the foundation of data communication on *World Wide Web*. A set of rules how message should transfer between server and browser.

 It was developed by [Tim Berners-Lee](https://en.wikipedia.org/wiki/Tim_Berners-Lee) and his team between *1989-1991*.
In the early days of Internet, computer can connect each other, but they don't have a standard language to communicate each other.

>[!Warning] Problem:
> Data was passing in plain text. So, anyone can read or steal data.
> 
> To solve this problem [[HTTPS]] was introduces. 

### HTTP Request and Response 

To access a website first browser has to **make request** to a web server. To access a particular resource browser needs a perfect address. [[URL]] solve this problem.

- [i] Structure of HTTP request 
```
GET /blog/post?id=42 HTTP/1.1

Host: tryhackme.com
User-Agent: Mozilla/5.0 Firefox/87.0
Referer: https://tryhackme.com/

```

- Line-1 :  the first line has three things
	- **[[HTTP Method]]** : what we want to do >> `GET`
	- **Path** : which resource  >> `/blog/post?id=42`
	- **Version**: the version of HTTP
- Line -2: the website we want to access
- Line -3: the version of browser we are using
- Line -4: the webpage we want to request
- Line- 5: a empty line, which inform the web server that the request is finished.


- [i] Structure of HTTP response 
```
HTTP/1.1 200 OK

Server: nginx/1.15.8
Date: Fri, 09 Apr 2021 13:34:03 GMT
Content-Type: text/html
Content-Length: 98


<html>
<head>
    <title>TryHackMe</title>
</head>
<body>
    Welcome To TryHackMe.com
</body>
</html>

```

- Line-1 :  the first line contains three things
	- **Version** : the version of HTTP >> `HTTP/1.1`
	- **[[HTTP Status Code]]** : status of response  >> `200`
	- **Reason phrase**: `OK`
- Line -2: the web-server software and version
- Line -3: the time zone of web-server
- Line -4: what type of information will send (like: HTML, IMG, VIDEO.....etc)
- Line- 5: the length of a response
- Line- 6: a empty line, which inform that the response is finished.


