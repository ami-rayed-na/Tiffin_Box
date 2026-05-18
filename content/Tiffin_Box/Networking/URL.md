---
tags:
  - basic
  - networking
---
URL stands for **Uniform Resource Locator**. It tells the address of the resource on the internet. It tells the browser *where* & *how* to go there.

 ```
 https://user:password@www.example.com:8080/blog/post?id=42&lang=en#comments
 ```
 There are few parts in URL. But not all parts are used in every time.

| Part             | Example          | What it mean                                     |
| ---------------- | ---------------- | ------------------------------------------------ |
| **Scheme**       | `https://`       | the protocol to use                              |
| **User**         | `user:password`  | some service require authentication before login |
| **Subdomain**    | `www.`           | subsection of the domain                         |
| **Domain**       | `example.com`    | address of website                               |
| **Port**         | `:8080`          | the connecting port number                       |
| **Path**         | `/blog/post`     | the file name or location of the resource        |
| **Query String** | `?id=42&lang=en` | extra information passed to the server           |
| **Fragment**     | `#comments`      | specific section of the page                     |