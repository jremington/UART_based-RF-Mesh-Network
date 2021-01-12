# UART_based-RF-Mesh-Network

This project is based on the following, recommended tutorial   
 http://duino4projects.com/simple-arduino-wireless-mesh/

A strength of this approach is the UART basis, which means it will work with any UART serial RF modem (or wires, of course) and supports an auto-synchronizing node time stamp which is propagated from the lowest node. So, for accurate time stamps, only one node needs an RTC. Presently configured for 4 nodes, up to 16 nodes possible with given time slots. Presently, two integer data input and two data output slots are allocated per node, which also propagate around the network.

I removed all the crash-inducing String objects and cleaned up the remaining code. It has been extensively tested on a network with Arduino Pro Minis, using AltSoftSerial for the "UART" connections.  

A sample log file shows how the local time is updated on each node.
