# TCP/IP Model

Tcp/ip model is a framework for understanding and designing computer networks which consist of four core layers.

TCP/IP is the fundamental set of protocols that provides the backbone for internet communication

Each layers has its own set of protocols by which data is being transmitted and recieved

- Protocol defines the set of rules and conventions that dictate how data is transmitted, received, and processed across a network

## Layers

### Network access layer:

This layer is responsible for sending and recieving data interms of frames over a physical medium (ex: LAN cable, Wireless adapters)

###### Widely used protocols:

1. **Ethernet (IEEE 802.3):** Ethernet is one of the most widely used LAN technologies. It defines the rules for wiring and signaling on the physical medium, as well as how devices on the network should address each other (MAC addresses).
2. **Wi-Fi (IEEE 802.11):** Wi-Fi is a set of standards for wireless local area networking. It defines how devices communicate over radio frequencies to establish wireless connections.
3. **Address Resolution Protocol (ARP):** ARP is used for mapping an IP address to a physical (MAC) address in a local network
4. **Reverse Address Resolution Protocol (RARP):** RARP performs the reverse process, mapping a MAC address to an IP address.

### Internet layer

The Internet Layer in the TCP/IP model is primarily responsible for routing packets across different networks to reach their destination

#### widely used protcols

###### Internet Protocol (IP):

- IP is the fundamental protocol at the Internet Layer.

* It provides a standardized way for devices to communicate over a network.
* The two main versions of IP are IPv4 and IPv6. IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses.

###### Internet control message protocol (ICMP):

ICMP is closely associated with IP and is used for sending error messages and diagnostic information about network conditions. Ping and traceroute are examples of tools that use ICMP.

###### Routing protocols

The set of protocols which are responsible for dynamically updating and maintaining routing tables. These protocols allow routers to exchange information about the reachability of networks and determine the best path for forwarding packets.Some of the widely used protcols

- **Routing Information Protocol (RIP):**

  - **Devices:** RIP is often used in small to medium-sized networks.
  - **Example:** A small office network with a few routers.

- **Open Shortest Path First (OSPF):**

  - **Devices:** OSPF is well-suited for large and complex networks.
  - **Example:** Enterprise networks, university campuses, or large corporate networks.

- **Border Gateway Protocol (BGP):**

  - **Devices:** BGP is commonly used between different Autonomous Systems (ASes) in the global Internet.
  - **Example:** Internet Service Providers (ISPs) use BGP to exchange routing information and determine the best paths for traffic between their networks.

### Transport layer:

The Transport Layer in the TCP/IP model is responsible for end-to-end communication between devices on a network. It ensures that data is reliably and accurately delivered from one device to another. The two main protocols associated with the Transport Layer are Transmission Control Protocol (TCP) and User Datagram Protocol (UDP). Here are details about these protocols:

1. **Transmission Control Protocol (TCP):**
   - **Characteristics:**
     - Connection-oriented: Establishes a reliable, connection before data transfer.
     - Provides error checking and correction.
     - Ensures in-order delivery of data.
     - Flow control to manage data transmission rates.
   - **Use Cases:**
     - Reliable data transfer is critical (e.g., file transfers, web pages).
     - Applications that require accurate and ordered delivery of data.
2. **User Datagram Protocol (UDP):**
   - **Characteristics:**
     - Connectionless: Does not establish a connection before data transfer.
     - Unreliable: Does not provide error checking or correction.
     - No flow control: Data is sent without checking whether the receiver is ready.

### Application layer:

The Application Layer is the top layer of the TCP/IP model. It provides network services directly to end-users or applications. The Application Layer is responsible for network communication, including file transfers, email, and other network-related functions. Various protocols operate at this layer to support a wide range of applications. Here are some of the key protocols associated with the Application Layer:

#### widely used protcols

1. **Hypertext Transfer Protocol (HTTP):**
   - HTTP is the foundation of data communication on the World Wide Web. It is used for transferring hypertext, such as HTML files, to enable the display of web pages in browsers.
2. **Hypertext Transfer Protocol Secure (HTTPS):**
   - HTTPS is the secure version of HTTP, adding a layer of encryption (usually using SSL or TLS) to ensure secure communication over the internet, commonly used for online banking, shopping, and other sensitive transactions.
3. **File Transfer Protocol (FTP):**
   - FTP is used for transferring files between computers on a network. It allows users to upload and download files from remote servers.
4. **Secure Shell (SSH):**
   - SSH provides a secure, encrypted communication channel over an unsecured network. It is commonly used for remote command-line login, remote command execution, and other secure network services.
5. **Telnet:**
   - Telnet is a protocol that provides a command-line interface to communicate with a remote device over a network. It is less secure than SSH and is used for testing and troubleshooting network connectivity.
6. **Simple Mail Transfer Protocol (SMTP):**
   - SMTP is used for sending email messages between servers. It defines how email messages should be sent and received over the internet.
7. **Post Office Protocol version 3 (POP3):**
   - POP3 is an email retrieval protocol that allows users to download their email messages from a mail server to their local devices.
8. **Internet Message Access Protocol (IMAP):**
   - IMAP is another email protocol, similar to POP3, but it allows users to manage their email messages directly on the mail server, providing more flexibility.
9. **Domain Name System (DNS):**
   - DNS is responsible for translating human-readable domain names into IP addresses. It is crucial for navigating the internet using domain names (e.g.,[www.example.com](http://www.example.com/)).
10. **Simple Network Management Protocol (SNMP):**
    - SNMP is used for network management and monitoring. It allows devices to be monitored and controlled remotely.
11. **File Transfer Protocol over Secure Shell (SFTP):**
    - SFTP is a secure file transfer protocol that operates over an encrypted SSH connection. It provides a secure way to transfer files similar to FTP.
