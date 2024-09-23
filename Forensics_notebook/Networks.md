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

[[First_obs_excalidraw]]

A fun point made in the video which I remember as vaguely as anything was how floppy disk were used, or how thumb drives stored information. A nice definition for networking was that it is only just a logical grouping of hosts which require similar connectivity. 

Think of the example of a home network or a coffee shop network. The devices become part of a larger connection that helps identify where information is to be transferred to. 


---

The next video deals with hubs, switches, routers, and bridges. These are used to deal with decay. Similar to how repeaters work because electricity can only transfer data so far before decay or loss. This is also why fiberoptics are dope. Saw another video on those which explained why they are so common; they are cheaper, can be grouped/bundled, and they lose less data due to the way they bend back signals passed through 'better'. 

A repeater simply 'regenerates' signals- this actually sounds crazy to think about if you have no idea how electricity functions. One video I will try to link explained it beautifully and made perfect sense of electric signals. In short, when a signal is positive it send a certain voltage, if not, it is 0 and this is the basis for binary. 

Repeaters, hubs, switches, routers, and bridges were built in order to deal with the problems of technology. 

Connecting hosts directly would not scale and the internet would be unmaintainable. A hub is like a multi port repeater.  A bridge is like a hub of hubs. It connects hub-connected hosts. They only have two ports and they "learn"  which hosts are on each side. This makes some sense but is too abstracted to mean anything so I will research this more on google. 