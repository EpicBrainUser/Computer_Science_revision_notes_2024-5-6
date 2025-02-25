**T1:**

- **WANs**  
  - Stands for Wide Area Network  
  - A network that covers a large geographical area  
  - Includes leased lines (relies on 3rd party architecture, such as ISPs which which offer the “necessary connectivity” such as fiber-optic cables)   
  - Some large organizations will use 1st party infrastructure, though  
  - Some examples include the Internet

    

- **Packet Switching:**  
  - Data is split into 512-byte chunks.  
  - Each packet travels independently through different routes in the network.  
  - Routers decide the best path based on traffic conditions.  
  - Each packet contains a header with source and destination IP addresses. They also contain packet/sequence number so can be identified and reordered  
  - Upon arrival at the destination, packets are reassembled in the correct order.  
  - If any packet is lost or corrupted, a retransmission request is sent.  
  - This system allows for more efficient network usage, enabling simultaneous data transfers.

- **DNS:**  
  - A system of servers, and other resources, used to link a URL typed into a browser with an IP address understood by routers.  
  - How it works:  
    - The user types "archlinux.org" into the web browser.  
    - The browser checks if the IP address for the domain is already stored in its DNS cache.  
    - If not found, the browser sends a request to a DNS recursor (usually provided by the ISP).  
    - The DNS recursor asks a root DNS server to locate the TLD (Top Level Domain) server for ".co.uk".  
    - The TLD server points the recursor to the Authoritative DNS server for archlinux.org.  
    - The Authoritative DNS server provides the correct IP address for archlinux.org.  
    - The recursor sends the IP address back to the browser.  
    - The browser uses the IP address to connect to the BBC server.  
    - The browser requests the webpage, and the BBC server sends the webpage’s content.  
    - The website is displayed for the user, using the domain name instead of the IP address.

- **MAC Addresses and NICs:**  
  - An NIC is a hardware component which enables communication over wired or wireless connections, and each NIC is assigned a unique MAC (Media Access Control) address to identify the device on the network.  
  - A MAC address is an address is assigned to each Network Interface Card (NIC) by the manufacturer  
  - It allows for the Switch to correctly route incoming data packets to the correct device, it checks the destination MAC address. Then the switch looks up the MAC address in its MAC address table to determine the correct port. The switch forwards the data packets to the correct port based on the MAC address, ensuring the data reaches the right node.  
      
- **IP Addresses:**  
  - An address assigned to devices connected to the internet used by routers to direct data packets towards their destination  
  - Geographically assigned, therefore changes when location of device changes  
  - Two types: IPv4 and IPv6

**T2:**

- **LANs**  
  - Stands for Local Area Network  
  - A network that covers a small geographical area  
  - Some examples include homes, schools  
  - Mainly by the use of a single organisation’s infrastructure (no leased lines)  
      
- **Protocols:**  
  - A set of rules that “dictates” how data is transmitted/formatted/processed between nodes on a network

- **Networked computers advantages and disadvantages:**  
  - Advantages of Networks:  
    - Computers can share resources such as printers.  
    - Files can be accessed through any computer in the network.  
    - Data is easy to back up as it is stored centrally on the server.  
  - Disadvantages of Networks:  
    - Purchasing the network hardware is expensive.  
    - Managing a large network is complicated.  
    - Viruses may be able to infiltrate the network and infect every computer.

- **Topologies:**  
  - Advantages of Star Topologies:  
    - Fast data transfer to the switch as each wire isn’t shared with other computers.  
    - If one cable fails, the other computers are not affected.  
    - Allows for central control, admin can update and monitor all nodes  
  - Disadvantages of Star Topologies:  
    - Requires additional hardware such as the central switch and network cables.  
    - If the central switch fails, the whole network goes down  
  - Mesh networks is when individual nodes act as switches as no central switch, to relay information to other nodes  
  - Advantages of Mesh Topologies:  
    - No single point of failure \- it is resilient.  
    - Expansion and modification can be done without disrupting the network.  
  - Disadvantages of Mesh Topologies:  
    - Expensive to install cabling if using wired connections.  
    - Network maintenance and administration is difficult.  
        
- **Network Hardware and Transmission Mediums:**  
  - A Network Interface Card/Controller (NIC) in your computer or device  
  - A switch to provides connection to the network: it will log the MAC address of the connected NIC  
  - A router to relay packets between the LAN and the Internet  
  - A Wireless Access Point connects wireless devices to a network. (Many home wireless access points are part of   
  - the router)  
  - Ethernet, along with WiFi are transmission mediums  
  - Some advantages of Ethernet over WiFi:  
    - More reliable than WiFi, as it is less prone to interference.  
    - Less likely to experience lower speeds, connection drops, or inconsistent performance.  
    - Reduces the risk of issues, such as preventing staff from booking tickets.  
    - More secure and less likely to be intercepted compared to WiFi via packet sniffing

**T3:**

- **Bluetooth**  
  - A wireless method of connecting devices together over a short distance  
  - Operates over 2.4GHz  
  - Devices need to be paired

- **WAPs**  
  - Wireless Access Points are devices that allows devices to connect wirelessly to a network via WiFi

- **Standards**  
  - An agreed set of technical specifications to ensure compatibility.  
  - An example is Ethernet

- **Encryption and Data Interception**  
  - Customers using a wireless network connection, such as WiFi, should exercise caution as they are more vulnerable to data interception.  
  - Data transmitted over WiFi can be intercepted by malicious users using packet sniffing tools, allowing them to capture sensitive information such as passwords, credit card details, or personal messages.  
  - A wired connection, on the other hand, requires a physical connection to the network, making it much harder for attackers to intercept data compared to the "passive" packet sniffing possible with WiFi.  
  - This can be fixed with encryption, which is the process of converting data (plaintext) to prevent unauthorized access  
  - By using WPA (WiFi Protected Access) is a security protocol that encrypts wireless transmission with 256-bit encryption (WPA2 and WPA3 are some examples)  
  - When referring to encryption in general, there is  
    - Symmetric encryption: where the same key is used to encrypt and decrypt plaintext  
    - Asymmetric encryption: a public key known to everyone for encrypting and a private key for decrypting

- **Factors affecting “reception”**  
  - WiFi:  
    - Devices may experience poor reception due to interference.  
    - Interference occurs when devices and physical obstructions (like walls) cause "signal degradation."  
    - The 5GHz band, which offers faster data transmission speeds, is more susceptible to interference from physical obstacles, such as walls  
    - Signal degradation is more apparent when using the 5GHz band.  
    - To improve reception, switching to the 2.4GHz band is recommended

T4:

- **Client-Server:**  
  - The server is a powerful computer which provides services or resources required by any of the clients  
  - The server will:  
    - The server waits for requests from a client  
    - Performs any processing required to fulfil the request  
    - The requested data is sent back to the client  
  - A client is a computer or device which requests the services or resources provided by the server  
  - The client will  
    - Send requests to the server  
    - Waits for a reply  
    - Receives the reply  
  - An example of client-server is accessing web pages  
  - In a school network, servers included:  
    - A file server holds all the data files and databases and manages backups  
    - A print server may organise printing on different printers  
    - An email server may receive emails, detect and block spam, distribute emails to users  
    - A web server may host the school’s external website  
    - A database server may hold student records  
  - Advantages of C-S:  
    - With file servers, files can be accessed from any computer and just one file server needs to be backed up (in case it “fails”, instead of every individual computer needing to be backed up individually)  
    - Email servers provide a central place for email that is then accessed from different devices  
    - One print server can manage all files to be printed. This allows one printer to be shared by many computers  
    - Security is managed by a central server, instead of every individual computer, and there being no central firewall.   
    - Compex processing can be performed by a more powerful computer

- **Peer to Peer:**  
  - Suitable for a small companies with fewer computers  
  - All computers can easily see files on all other computers  
  - All computers can communicate with each other without going through a server  
  - Advantages of P2P  
    - Linking computers in a peer-to-peer network is easy to set up.  
    - Computers can be cabled together without the need for dedicated server equipment.  
    - No dedicated server means reduced costs (cheaper setup).  
    - Without a central server, if it fails, all data and services are lost (unless backed up).  
    - If one computer fails, only the services it provides are lost.  
    - Some networks distribute services among peers, allowing the network to continue functioning even if one computer goes down (no single point of failure)  
- **Hosting:**  
  - Web hosting is a service offered by companies that will host web pages and files for websites  
  - Advantages:  
    - Web hosts have far more bandwidth – so they can serve more users  
    - Web hosts are able to monitor their equipment 24 hours a day

- **The Cloud:**  
  - The Cloud refers to services (resources and applications) that are "delivered" over the Internet.  
  - It allows users to store and access data and software on remote servers instead of on their local device.  
  - This enables users to access their information from any device, as long as they have an internet connection.  
  - Advantages over local storage:  
    -   
    - Cloud computing services are delivered over the internet, allowing users to access all files and software from anywhere, at any time, as long as an internet connection is available.  
    - There is no need for dedicated equipment to store data, such as a large capacity SSD/HDD, as everything can be stored on remote servers.  
    - No need to back up data, as it is done by the service provider  
  - Disadvantages over local storage:  
    - Personal data will be stored on another company’s servers  
    - If the Internet connection is lost, often the service becomes unusable  
    - Slow Internet connections may result in a poor quality   
      of service  
    - Although most cloud services will backup data stored with them, it is not easy for people and organisations to see how resilient this is  
  - Examples include Google Drive, OneDrive, Dropbox

- **Other factors that affect network performance**  
  - Including transmission mediums, there are other factors that affect network performance  
  - Bandwidth:  
    - Measured in Mbps  
    - Affects network performance by determining the amount of data that can be transmitted at once  
    - Lower bandwidth can lead to slower speeds, especially when multiple users access shared resources  
  - Latency:  
    - Measured in ping (milliseconds)  
    - The amount of time it takes for a packet to travel across a network or the delay in data transmission  
    - High latency means requests take longer to reach the server and back, making emails slow to load

T5:

- **Protocols:**  
  - A communications protocol is a set of rules that defines/dictates how data is transmitted/received across a network  
      
- **Layers:**  
  - A layer is a "framework" that organizes communication in networks, helping to understand complex network interactions.  
  - It allows hardware and software to be designed for specific tasks, ensuring different systems work together even when developed independently.  
  - Each layer operates independently but relies on protocols (e.g., HTTP, TCP/IP) to ensure proper communication.  
  - Hardware/software developed for a specific layer only needs to work with the next layer, ensuring the network functions cohesively.  
  - Layers simplify troubleshooting by allowing issues to be quickly identified and fixed without affecting other layers, as each layer is self-contained.  
  - The TCP/IP layer is formed from 4 layers:  
    - Application Layer:  
      - HTTPS  
      - Computer application produces data for sending  
    - Transport Layer:  
      - TCP  
      - Splits data into packets  
    - Internet Layer:  
      - IP  
      - Routes packets  
    - Link Layer  
      - Ethernet Cables  
      - Physical hardware and cables

- **HTTP vs HTTPS:**  
  - HTTP  
    - A protocol that allows web pages written in HTML to be transferred between a client and a web server.  
    - Data transferred via HTTP is not encrypted, making it vulnerable to interception.  
  - HTTPS  
    - Uses protocols like TLS (Transport Layer Security) or SSL (Secure Sockets Layer) to encrypt data during transmission.  
    - Ensures that data cannot be intercepted, offering protection from man-in-the-middle attacks.  
    - This would be used for website handling sensitive data, such as online banking sites, which transfer data such as personal information, passwords, financial transactions between the client and their web server  
    - This encryption prevents man-in-the-middle attacks, reducing the risk of fraud and identity theft.

- **SMTP vs IMAP vs POP:**  
  - SMTP (Simple Mail Transfer Protocol):  
    - SMTP is used for sending emails from a client to a local mail server then to the webmail server (via mail relays), which would be the recipient's email server.  
  - IMAP (Internet Message Access Protocol):  
    - IMAP is used for retrieving received emails from their mail server.  
    - Emails are stored on remote servers, allowing access from any device.  
  - POP (Post Office Protocol):  
    - Used for retrieving emails from the server.  
    - Unlike IMAP, emails are downloaded and stored locally on the recipient’s device, making it harder to access them from multiple devices.  
      

