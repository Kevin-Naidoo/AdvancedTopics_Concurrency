## What is an IP Address?

Internet Protocol - Opens up communication and allows for devices to connect to the internet.

 * Can be found on windows using `ipconfig`
 	* Can find IP address, Subnet Mask & Default Gateway

 * Router uses DHCP to give devices IP Addresses.
 * `192.168.1.xxx` - Why do they start with those digits
 	*  The subnet mask is responsibile for this
        * Subnet Musk - `255.255.255.0`
	* Each group of 3 digits are called an octat
 	* The 255 represents locked-in unchangeable numbers (network portion) the 0 represents an arbitrary number allocated between 0 - 255 (host portion)
 	* The network portion stays the same because the devices nearby are on the same network.
	* If IP address you are trying to connect to outside its network, it has to talk to its default gateway.
	* Three IP addresses are reserved - The network address: `192.168.1.0` & the broadcast address: `192.168.1.255` & the default gateway: `192.169.1.1`

## Are we out of IP Addressing :anguished:

There are 2<sup>32</sup> IP addresses available.
The are 5 classes of IP addresses.


| | Range                       | Subnet Mask   |
|--- | --------------------------  | ------------- |
|A| 1.0.0.0 - 126.255.255.2555  | 255.0.0.0     |
|B| 128.0.0.0 - 191.255.0.0     | 255.255.0.0   |
|C| 192.0.0.0 - 223.255.255.0   | 255.255.255.0 | 
|D| 224.0.0.0 - 239.255.255.255 |               |
|E| 240.0.0.0 - 255.255.255.255 |               |

### Classes:

 `Class A` -> Host heavy networks -> 2<sup>24</sup> <br>
 `Class B` -> 2<sup>16</sup> <br>
 `Class C` -> Largest IP range: 2<sup>8</sup> <br>
 `Class D` -> Multicast <br>

Between `Class A` & `Class B` is 127.0.0.0 --> These are reserved on you computer for testing. The 127 triggers **loopback**

## Private IP Addresses and NAT:

`RFC 1918` - Private IP addresses. You need a public IP Address to interact with the internet. 


| | Range                       | Subnet Mask   |
|--- | --------------------------  | ------------- |
|A| 10.0.0.0 - 10.255.255.255 | 255.0.0.0     |
|B| 172.16.0.0 - 172.31.255.255 | 255.255.0.0   |
|C| 192.168.0.0 - 192.168.255.255 | 255.255.255.0 |


Private IP are not routable on the internet. So...<br>
### NAT -> Network Address Translation

	* Router performs NAT
	* Translates private IP into public IP via Router
	* It allocates 1 IP Address by ISP -> Internet Service Provider
	* When request is sent back, it is routed back to that specific device
	* This soultion did not last because we still ran out of IP Addresses <br>

### Thus intoduction to IPv6 -> 2<sup>128</sup> 
