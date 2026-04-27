#basic #networking 

When a HTTP server response, the first line always contains a 3-digit status code. Which informs clints about the outcome of the request.
*It can classified under 5 classes--*

| Status       | General code | Range   | Meaning                            |
| ------------ | ------------ | ------- | ---------------------------------- |
| Informal     | 1xx          | 100-199 | Hold on, still processing...       |
| Success      | 2xx          | 200-299 | All good                           |
| Redirection  | 3xx          | 300-399 | What you want is somewhere else... |
| Client Error | 4xx          | 400-499 | You did something wrong...         |
| Server Error | 5xx          | 500-599 | Server did something wrong....     |

### Common HTTP Code
| Code | Name                  | Meaning                                                                                                                                                            |
| ---- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 100  | Continue              | Keep going, request received so far is OK                                                                                                                          |
| 103  | Early Hints           | Server sends headers early while preparing response                                                                                                                |
| 200  | OK                    | The request was completed successfully.                                                                                                                            |
| 201  | Created               | A resource has been created                                                                                                                                        |
| 202  | Accepted              | Request received but processing isn't done yet                                                                                                                     |
| 301  | Moved Permanently     | Page has a new URL forever                                                                                                                                         |
| 302  | Found                 | Temporary redirect                                                                                                                                                 |
| 400  | Bad request           | Malformed or invalid request                                                                                                                                       |
| 401  | Unauthorised          | You need to log in first                                                                                                                                           |
| 403  | Forbidden             | Logged in but not allowed here                                                                                                                                     |
| 404  | Not found             | The page/resource you requested does not exist.                                                                                                                    |
| 405  | Method not allowed    | The resource does not allow this method request, for example, you send a GET request to the resource /create-account when it was expecting a POST request instead. |
| 408  | Request Timeout       | Server waited too long for your request                                                                                                                            |
| 500  | Internal Server Error | The server has encountered some kind of error with your request that it doesn't know how to handle properly.                                                       |
| 502  | Bad Gateway           | Server got a bad response from an upstream server                                                                                                                  |
| 503  | Service Unavailable   | Server is down or overloaded                                                                                                                                       |

- [*] There is a funny [website](https://http.cat/), you can check it out :) 
