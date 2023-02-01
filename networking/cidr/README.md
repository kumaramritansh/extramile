# Classless Inter Domain Routing (CIDR)

Classful addressing the no of Hosts within a network always remains the same depending upon the class of the Network.

- Class A network contains 2^24 Hosts,
- Class B network contains 2^16 Hosts,
- Class C network contains 2^8 Hosts

let’s suppose an Organization requires 214 hosts, then it must have to purchase a Class B network. In this case, 49152 Hosts will be wasted. This is the major drawback of Classful Addressing.

In order to reduce the wastage of IP addresses a new concept of Classless Inter-Domain Routing is introduced. Now a days IANA is using this technique to provide the IP addresses. Whenever any user asks for IP addresses, IANA is going to assign that many IP addresses to the User.

**Representation:** It is as also a 32-bit address, which includes a special number which represents the number of bits that are present in the Block Id.

```a . b . c . d / n```

Where, n is number of bits that are present in Block Id / Network Id.
Example:

```20.10.50.100/20 ```


## Rules for forming CIDR Blocks:

1. All IP addresses must be contiguous.

2. Block size must be the power of 2 (2n).
If the size of the block is the power of 2, then it will be easy to divide the Network. Finding out the Block Id is very easy if the block size is of the power of 2.
Example:
If the Block size is 25 then, Host Id will contain 5 bits and Network will contain 32 – 5 = 27 bits.
![CIDR](https://media.geeksforgeeks.org/wp-content/uploads/20190313121313/b31.jpg)

3. First IP address of the Block must be evenly divisible by the size of the block. in simple words, the least significant part should always start with zeroes in Host Id. Since all the least significant bits of Host Id is zero, then we can use it as Block Id part.