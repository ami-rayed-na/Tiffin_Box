---
tags:
  - basic
  - networking
  - https
---

TLS *(Transport Layer Security)* Handshake is the process used to establish a secure connection between a client (browser) and a server before actual data communication begins.

The TLS handshake is a core part of HTTPS communication. Its main purpose is to:

- Authenticate the server
- Exchange encryption keys securely
- Establish a secure encrypted session

### Steps of TLS handshake

- **Client Hello:** The client (browser) send message to the server containing 
	- Supported TLS version
	- Supported encryption method
	- Other security information

- **Server Hello:** The server response with
	- Selected TLS version
	- Selected encrypted method
	- [[TLS certificate]]

- **Certificate Verification:** The browser checks the certificate to verify
	- The certificate validity
	- The authority of certificate provider
	- The identity of website 
	- Check the expiry date of certificate

- **Key Exchange:** The browser generates a secret key using the public key from certificate and send it over. Only the server can decrypt it with its private key.

- **Session Key ready:** Both side now independently derive the same shared session key from the exchanged secrets. The servers confirm it ,the tunnel in open.

- **Encrypted HTTP:** Normal HTTP flow through the tunnel. The content are identical to plain HTTP --- just scrambled so only these two parties can read it.