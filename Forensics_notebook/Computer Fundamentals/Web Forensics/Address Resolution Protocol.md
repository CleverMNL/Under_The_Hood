

ARP builds a cache/history/log called the ARP cache that stores information about the request. Specifically, it stores the IP and MAC sent and received. It is a 4 step process of sending a request with an L2 header that contains the requestor device IP and MAC addresses to the local network looking for a device associated with a specific IP address, after the receiver gets the request, it sends back its MAC address to the requestor device and that device updates its ARP cache to include the IP and the MAC address of the receiver device.

[[ARP_drawing]]