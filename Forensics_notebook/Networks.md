#### First lesson in the first module- https://www.youtube.com/watch?v=bj-Yfakjllc&list=PLIFyRwBY_4bRLmKfP1KnZA6rZbRHtxmXi&index=1

Examine Host, IP Addresses, and Networks

Hosts: any device which sends or received traffic (wth is traffic)

- Computer
- Laptop
- phones
- printers
- servers
- cloud servers
- IoT devices (that would include TV, speakers, light, Alexa, dishwasher if smart, refrigerator if smart)

they all follow the same rule for how to send and receive communications with the internet
  
Clients or server

Clients initiate requests, servers responds

Servers have specific software that knows how to server pages to a client

A server can be a client if it initiates a request. It is relative to a specific communication method, File server example.

IP addresses are an identity of each host: (I want to add a comment here that I have watched and read about the cybersecurity sector for a while now and have taken notes before but this is something I want to pass long as a journal of my journey of sorts. I will do the same for other subject matters of interest such as finance and web development, forensics, etc. a motivation is the renaissance/Enlightment eras. A more specific motivation to cybersecurity is the DefCon community and videos on Youtube.)


---

IP addresses can be thought of as phones. Devices as stamped with a specific address (numbers) that identify that device. This is really just 32 bits broken into 4 chunks.


```
10010000010000000100010010001

1000 1000 - 0001 0000 - 0001 0001 - 0001 0001
```

In this way, the 4 bits set in groups of 2 make up 8. The largest binary representation of 8 bits is 255.  Each group can be a number between 0-255.

IP is simple to understand because it is created to be assigned hierarchically. An easy way to visualize this may be to just create a visual. 

[[IP_address_drawing]]

A fun point made in the video which I remember as vaguely as anything was how floppy disk were used, or how thumb drives stored information. A nice definition for networking was that it is only just a logical grouping of hosts which require similar connectivity. 

Think of the example of a home network or a coffee shop network. The devices become part of a larger connection that helps identify where information is to be transferred to. 


---

The next video deals with hubs, switches, routers, and bridges. These are used to deal with decay. Similar to how repeaters work because electricity can only transfer data so far before decay or loss. This is also why fiberoptics are dope. Saw another video on those which explained why they are so common; they are cheaper, can be grouped/bundled, and they lose less data due to the way they bend back signals passed through 'better'. 

A repeater simply 'regenerates' signals- this actually sounds crazy to think about if you have no idea how electricity functions. One video I will try to link explained it beautifully and made perfect sense of electric signals. In short, when a signal is positive it send a certain voltage, if not, it is 0 and this is the basis for binary. 

Repeaters, hubs, switches, routers, and bridges were built in order to deal with the problems of technology. 

Connecting hosts directly would not scale and the internet would be unmaintainable. A hub is like a multi port repeater.  A bridge is like a hub of hubs. It connects hub-connected hosts. They only have two ports and they "learn"  which hosts are on each side. This makes some sense but is too abstracted to mean anything so I will research this more on google. 

Bridges were the first to contain data transfers to their relative networks, this helped retain safety of information leakage- info from one network going into another network- when it does not need to. It also understands when one network wants to specifically send info to another network.

Switches combine hubs and bridges. They have multiple ports, unlike the dual port bridge. It also learns which host are on each port. This organizes communication logically. Switches help simplify communication logic within a network. It makes it so that devices in a network like a school or building/company can transfer data to each other without having to worry about finding which device to send the data to get to the destination it desires within a network. [[Switches_drawing]]
This illustrates switches and adds a little more scale to networks. 

Routers simplify communications between networks. Think Network to network. In the switches drawing, I also added the illustration of added routers for networks to function. This is the connectivity basis behind the interconnected network/internet. Routers are what also filters traffic and acts as the bouncer for networks. It used to be the case that switches could not perform this kind of filtering. They also "learn" about which networks they are connected to. Using this information, they build what is called a routing table which is a list, for lack of a better word, of all the networks the router "knows about"/connects with. 

- [ ] Routing is the process of transferring data between networks
- [ ] Switches/switching is the process of transferring data within networks

A final point in this video is that this topic was very surface level and that there are many other network devices such as:
- access points
- firewalls
- load balancers
- L3 switches
- IDS/IPS's
- Proxies
- etc

There all aim at fixing issues with the web. Think about what load balancing would mean, and firewalls being used, or if proxies mean the same thing in networks as they do in equity securities.


---

This next video covers the OSI model through a practical perspective.

Purpose of networking: 
	 allow host to  share data remotely.

the rules for networking is make into the system behind the OSI model. 

He makes an analogy using the human body as it is made up of various systems working in conjunction for a specific purpose. The physiology is broken down into the skeletal system, nervous, respiratory, cardiovascular, etc. 

The OSI divides specific rules into 7 layers that each address a specific function to allow the network to - well- work. If they all do function properly, hosts can transfer data. This video aims to help us understand the purpose of each layer and how it contributes to the **goal** of Networking.

L1 = Physical
 - data exists in the form of bits (binary)
 - "something" has to transport those bits regardless of the Wi-Fi, Bluetooth, etc.
These are things like fiberoptic cables, ethernet cables, coaxial cables. etc. Physical things. Wi-Fi is still considered an L1 technology or part of L1 because it serves the purpose of moving bits form one place to another. 

L2 = Data link
-  interacts directly with the L1 technologies; the physical layer
-  in the past, NIC's and Wi-Fi access cards were separate hardware components
- switches are also part of this layer
He labels this a hop to hop layer because it is used to communicate host to host. 

<font color="#b7dde8">One relevant point I realized too was that the further back in time you go into trying to learn about modern technology, the more you may learn and appreciate. </font>

 - Here we are introduced to MAC addresses or address scheme which is 48 bits, represented as 12 hex digits. 
 - 94-65-9C-3C-7A-E3  or  94:65:9C:3C:7A:E3  or  9665.9C3C.7AE3
 - <font color="#c3d69b">Every NIC has a unique MAC address</font>

 This entire process is about getting data from one point to another. All technologies built were designed for this. L2 makes sure to go from one device to the next, it is only concerned with that.

L3 = Network  (as he called end to end)
  - IP addresses
  - This deals with technologies that have an IP such as hosts and routers
The main difference with L3 from L2 is who is deals with, by who I mean what connections. While L2 deals with connection to connection, L3 deals with final destination of connection with initial connection or vice-versa -it doesn't matter . The best was to illustrate it with a visual. So here [[L2 and L3]] . The way that it transfers the data will be by adding L2 and L3 description information attached to the data it wants to transfer. Refer to the visual again. L2 would carry MAC address info, which is a certain amount of bits, and L3 would carry IP address info which is more bits, these are added to the data that is going to be transferred like a packet. The packet would have an L3 header which would look like the source IP address- the sender of data- and destination IP address - the receiver of that data as well as MAC addresses from source to destination. 
For short, it would be something like

```
src:100.11.1.11 -> dst:111.1.1.55
MAC: E8E4.84A5.9665 -> MAC:9665.9C3C.7AE3
```

Each router can be thought as having 2 MAC addresses one when it receives and one when it sends. There is a protocol that ties L2 and L3 called the Address Resolution Protocol (ARP) which links an L3 address to an L2 address.


---

L4 = Transport (service to service as he calls it)

This layer distinguishes (<- is that not a weird word) data streams
The addressing scheme used are called Ports
 - TCP and UDP
   - 0-65535 numbers used to identify in TCP 
   - 0-65535 numbers used to identify in UDP

Specific services like a game or a web chat or a website are each going to be associated with a specific port. Talks about a topic quickly over headers and how they work in L4. Let's assume a person is trying to use a specific chat server online. That server will be 'open'/'listening' for requests on already configured/set-up ports. This port that has been previously selected by the server will take requests from clients and connect them by sending back information using the  headers packet. 


```
: = port 

src-2.1.2.1 :800 # this port number is randomly selected by the client requesting
dst-3.2.3.2 :55 # This is a pre-defined port by the server

```

When the server sends back its information, like the webpage, or game it will send another packet.


```

src-3.2.3.2 :55
dst-2.1.2.1 :800 # This random port will be used by server to help send back info to client

```

One thing to note that is practical knowledge is that each time you make a request on your laptop or other device, you are using a randomly selected UDP/TCP port to design the routing/travel packet to find a device and for it to find you back. 


---

Layers 5, 6, 7 = Session, Presentation, Application (respectively)

Distinction between these layers is vague. ambiguous. so it sucks therefore, they are sometimes just put together. In a similar framework for networking called the TCP/IP model puts all three into a layer 4 called application. The other layers for the TCP/IP model are the Network Access which combines L1 and L2 of the OSI model, the internet which is the same as L3 network, and layer 3 is called Host to Host in TCP/IP but it called the transport layer/L4 in OSI.

Back to OSI:

 This part examines the entire process together. Recall that this is all used to get one request from client to server, that could be making a google search, searching google maps, ordering food online (wait, this is more complex the more I think about it because their could be multiple requests send over the same service). 

Working any of these models could be thought of easier if taken a top-down approach or in this case a 7 to 1 approach. You begin with identifying the application, then the transport (UDP/TCP), then the Network (IP), then the Data link (MAC), and finally the physical. The entire process of sending and creating a packet with this routing/travel information is called encapsulation. 

L5,6,7 seems to not have a direct name, L4 is called a segment, L3 is called a packet, L2 is called a frame and that just packs the entire 'packet' with the added data being transferred. The final step  is to then convert this information into binary (0's and 1's) to be sent over the wire or Wi-Fi. 

The host receiving the request works its way from 1-7 or the opposite of the requester. This important section went in 20 seconds. It starts with the other host who is being requested data. It takes the binary from the physical layer, and read out as the L2 frame which packs the data and the routing/travel packet. This begins a confirmation process to verify if the request is in the right location, if not, it sends it on its way. This entire process is called De-encapsulation. A nice visual was made in the end here and I have tried to re-create it here: [[OSI]]


---

This next section will be about what hosts do to speak on the internet. 