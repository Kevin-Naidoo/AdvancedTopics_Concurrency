## What is an IP Adress?

Internet Protocol - Opens up communication and allows for devices to connect to the internet.

 * Can be found on windows using `ipconfig`
 	* Can find IP address, Subnet Mask & Default Gateway

 * Router uses DHCP to give devices IP Addresses.
 * 192.168.1.xxx - Why do they start with those digits
 	*  The subnet mask is responsibile for this
        * Subnet Musk - 255.255.255.0
	* Each group of 3 digits are called an octat
 	* The 255 represents locked-in unchangeable numbers (network portion) the 0 represents an arbitrary number allocated between 0 - 255 (host portion)
 	* The network portion stays the same because the devices nearby are on the same network.
	* If IP address you are trying to connect to outside its network, it has to talk to its default gateway.
	* Three IP addresses are reserved - The network address: 192.168.1.0 & the broadcast address: 192.168.1.255 & the default gateway: 192.169.1.1

