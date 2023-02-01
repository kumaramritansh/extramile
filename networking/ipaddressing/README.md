# IP Addressing

IP address is an address having information about how to reach a specific host, especially outside the LAN. An IP address is a 32 bit unique address having an address space of 232.
Generally, there are two notations in which IP address is written, dotted decimal notation and hexadecimal notation.

- dotted decimal notation
![dotted decimal notation](https://media.geeksforgeeks.org/wp-content/cdn-uploads/IP_addressing_1.jpg)

- hexadecimal notation
![hexadecimal notation](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20190909105903/1212.png)

## Classful IP addressing

Classful IP addressing is an IPv4 addressing architecture that is divided into five classes as follows:

- Class A
- Class B
- Class C
- Class D
- Class E

Each of these classes has a valid range of IP addresses. Classes D and E are reserved for multicast and experimental purposes respectively. The order of bits in the first octet determine the classes of IP address.
IPv4 address is divided into two parts:

- Network ID
- Host ID

The class of IP address is used to determine the bits used for network ID and host ID and the number of total networks and hosts possible in that particular class. Each ISP or network administrator assigns IP address to each device that is connected to its network.

![Classful IP Addressing](https://media.geeksforgeeks.org/wp-content/cdn-uploads/IP_addressing_3.jpg)

### Class A
In class A, the first 8 bits are for the network part of the address, and the remaining 24 bits are reserved for the host part of the address. The leading first bit of the octet is fixed.
![class A](https://media.geeksforgeeks.org/wp-content/cdn-uploads/IP_addressing_4.jpg)

The higher order bit of the first octet in class A is always set to 0. The remaining 7 bits in first octet are used to determine network ID. The 24 bits of host ID are used to determine the host in any network.

We subtract two addresses from the network addresses since they are considered special addresses.

Usable addresses are as follows:
- 2^7-2= 126 network ID(Here 2 address is subtracted because 0.0.0.0 and 127.x.y.z are special address. )
- 2^24 – 2 = 16,777,214 host ID

### Class B
In class B, the first 16 bits are for the network part of the address, and the remaining 16 bits are reserved for the host part of the address. The leading first two bits of the octet are fixed.

![class B](https://media.geeksforgeeks.org/wp-content/cdn-uploads/IP_addressing_5.jpg)

The higher order bits of the first octet of IP addresses of class B are always set to 10. The remaining 14 bits are used to determine network ID. The 16 bits of host ID is used to determine the host in any network. 

Usable addresses are as follows:
- 2^14 = 16384 network address
- 2^16 – 2 = 65534 host address


### Class C
In class C, the first 24 bits are for the network part of the address, and the remaining 8 bits are reserved for the host part of the address. The leading first three bits of the octet are fixed.

![class C](https://media.geeksforgeeks.org/wp-content/cdn-uploads/IP_addressing_6.jpg)

The higher order bits of the first octet of IP addresses of class C are always set to 110. The remaining 21 bits are used to determine network ID. The 8 bits of host ID is used to determine the host in any network.

Usable addresses are as follows:
- 2^21 = 2097152 network address
- 2^8 – 2 = 254 host address

### Class D
IP address belonging to class D are reserved for multi-casting. The higher order bits of the first octet of IP addresses belonging to class D are always set to 1110. The remaining bits are for the address that interested hosts recognize.

Class D does not posses any sub-net mask. IP addresses belonging to class D ranges from 224.0.0.0 – 239.255.255.255.

Class D is reserved for multicasting.

![class D](https://media.geeksforgeeks.org/wp-content/cdn-uploads/IP_addressing_7.jpg)


### Class E
IP addresses belonging to class E are reserved for experimental and research purposes. IP addresses of class E ranges from 240.0.0.0 – 255.255.255.254. This class doesn’t have any sub-net mask. The higher order bits of first octet of class E are always set to 1111.

Class E is reserved for experiment and research purposes

![class E](https://media.geeksforgeeks.org/wp-content/cdn-uploads/IP_addressing_8.jpg)


### summary of classful addressing
![classfull addressing](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2015/07/nethostdata.jpg)