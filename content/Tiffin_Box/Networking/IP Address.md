---
tags:
  - basic
  - networking
---
IP (Internet Protocol) Address is a signature of a device, which helps to communicate devices through internet. 

### Why

There are a lot of devices that are connected to internet. Every one is passing information with each other. But pause for a second, how even the right data gooes to right device?? 
To solve this problem the concept of IP address arise. 

### Who invented??

IP was not developed by overnight or by a person. It is a collaborated work from multiple researcher. But when ever IP address is mentioned history recalls [Vint Cerf](https://en.wikipedia.org/wiki/Vint_Cerf) and [Robert Kahn](https://en.wikipedia.org/wiki/Robert_Kahn_(computer_scientist)) 

### History

- **IPv1:** this refers to the early stage of IP address. But officially there is no name for it. 
- **IPv2:**
- **IPv3:**
- **IPv4:**
- **IPv5:**

### IPv4

IPv4 was introduced in September 1981 . It contains **four** sets of **octet** separated by dots. Each octet represents eight bits. So each octet can have value from 0 to 255 ($2^8=265$). 
![[Pasted image 20260409195330.png]]
**Example of IPv4 :** 185.107.80.231
- 185 is first octet
- 107 is second octet
- 80 is third octet
- 231 is forth octet

This format can support 4 billion ($2^{32}$) unique address. But today world we have more than 4 billion devices. That's why IPv6 is introduced.

### IPv6

IPv6 was introduced in December 1995. It contains **eight** groups of four **hexadecimal** numbers, separated by colon. Each group containing 16 bits. In total it 128 bits. 
![[Pasted image 20260409200757.png]]
It means it can support $2^{128}$ or $3.4\times10^{38}$ devices with unique address.  

---
#### Classes of IPv4:

| IP Class |        Address Range         | Use case                                                                    |
| -------- | :--------------------------: | :-------------------------------------------------------------------------- |
| Class A  |  1.0.0.0 to 127.255.255.255  | Very large networks (like multinational companies)                          |
| Class B  | 128.0.0.0 to 191.255.255.255 | Medium-sized networks, such as large organizations                          |
| Class C  | 192.0.0.0 to 223.255.255.255 | Smaller networks, like small businesses or home networks                    |
| Class D  | 224.0.0.0 to 239.255.255.255 | Reserved for multicast groups.Not used for traditional devices or networks. |
| Class E  | 240.0.0.0 to 255.255.255.255 | Reserved for experimental purposes and future use                           |
