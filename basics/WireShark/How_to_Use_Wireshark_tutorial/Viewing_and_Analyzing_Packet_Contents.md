# Viewing and Analyzing Packet Contents
Now that you've recorded some network data it's time to take a look at the captured packets. The captured data interface contains three main sections: The packet list pane, the packet details pane, and the packet bytes pane.

## Packet List
The packet list pane, located at the top of the window, shows all packets found in the active capture file. Each packet has its own row and corresponding number assigned to it, along with each of these data points.

- **Time**: the timestamp of when the packet was captured is displayed in this column, with the default format being the number of seconds since this specific capture file was first created. To modify this format to something that may be a bit more useful, such as the actual time of day, select the Time Display Format option from Wireshark's view menu -located at the top of the main interface.
- **Souce**: This column contains the address(ip or other) where the packet originated.
- **Destination**: This column contains the address that the packet is being sent to.
- **Protocol**: The packet's protocol name(i.e., TCP)  can be found in this column.
- **Length**: the packet length, in bytes
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg2OTY3OTg0OCwtMjA4ODc0NjYxMl19
-->