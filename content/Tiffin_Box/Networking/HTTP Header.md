---
tags:
  - basic
  - networking
---

Headers are **key-value pairs** sent along with every HTTP request and response. They carry metadata (Extra information) — telling the server or browser _how_ to handle the message, _who_ is sending it, and _what_ it contains.

**Structure:** `key : value`

There are 3 types of headers:
- Request header
- Response header
- General/ security header

### Request Header

These headers are sent from clint to server.

> [!Example] Example of Request header
> ```
GET /api/user/42 HTTP/1.1
Host: api.example.com
Authorization: Bearer eyJhbGciOiJIUzI1NiJ9...
Accept: application/json
User-Agent: Mozilla/5.0 (Windows NT 10.0)
Cookie: session=xyz789
> ```

| Header            | Example              | Purpose                                |
| ----------------- | -------------------- | -------------------------------------- |
| `Host`            | `example.com`        | Which website you're targeting         |
| `User-Agent`      | `Mozilla/5.0`        | Which browser is using                 |
| `Accept`          | `text/html`          | Which format user can handle           |
| `Accept-Language` | `en-US`              | user proffered language                |
| `Referer`         | `https://google.com` | the request is made from which address |
| `Content-Type`    | `application/json`   | format requested body                  |
| `Content-Length`  | `667`                | size of requested body                 |
| [[Cookie]]        | `session=xyz`        | Stored cookies sent to server          |

### Response Header

These headers are sent back to clients after making server request.

>[!Example] Example of Response header
>```
>HTTP/1.1 200 OK
>Content-Type: application/json
>Content-Length: 128
>Cache-Control: private, max-age=300
>Set-Cookie: session=xyz789; HttpOnly; Secure
>```

| Header           | Example                    | Purpose                                                                                          |
| ---------------- | -------------------------- | ------------------------------------------------------------------------------------------------ |
| `Content-Type`   | `text/html; charset=UTF-8` | Format of the response body                                                                      |
| `Content-Length` | `4487`                     | size of the response body                                                                        |
| `Set-Cookie`     | `session=xyz; HttpOnly`    | stores a cookie in your browser                                                                  |
| `Cache-Control`  | `max-age=86400`            | How long to store the content of the response in the browser's cache before it requests it again |

