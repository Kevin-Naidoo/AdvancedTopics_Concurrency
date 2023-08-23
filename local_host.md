# Localhost (127.0.0.1)

When you (or your computer) call an **IP address**, you are usually trying to contact another computer on the internet. However, if you call the IP address `127.0.0.1` then you are communicating with the localhost – in principle, with your own computer. 

The localhost is not always directly identified with your computer. In most cases, it has a separate IP address like 192.168.0.1. within your personal network, which is different to the one you use on the internet, and is usually dynamically assigned by the internet service provider. **When you are talking about a localhost, you are referring to when a server is used on your own computer.**

`localhost` is a top-level domain reserved for documentation and testing purposes. When you try to access the domain, a loopback is triggered. If you acces "http://localhost" in the browser, the request will not be forwarded to the internet through the router, but will instead remain in your own system. Localhost has the IP address 127.0.0.1, which refers back to your own server. 

The protocol pair Transmission Control Protocol (TCP) and Internet Protocol (IP) are some of the cornerstones of the internet. However, TCP/IP is also used outside the internet, in local networks. During transmission, the Internet Protocol is responsible for allowing the IP address and subnet mask to address subscribers in a network.

The allocation of public IP addresses (those that can be reached through the internet) is regulated by an international organization: the Internet Corporation for Assigned Names and Numbers (ICANN). ICANN is also responsible for the allocation of domain names, or the Domain Name System (DNS).

TCP/IP recognizes from the first block (127) that you don’t want to access the internet, you are calling yourself instead. This then triggers the loopback.

However, the host file is still present in most operating systems. With Windows, you can find the file under `\system32\drivers\etc\hosts`; with macOS and other Unix systems, it is found under `/etc/hosts`.
