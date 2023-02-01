# SUBNETTING

Subnetting is a method of dividing a single physical network into logical sub-networks (subnets). Subnetting allows a business to expand its network without requiring a new network number from its Internet service provider. Subnetting helps to reduce the network traffic and also conceals network complexity. 

A subnet, sometimes known as a subnetwork, is a part of a larger network. Subnets are the logical division of an IP network into many smaller network parts. To reduce traffic, a subnet's purpose is to divide a huge network into a collection of smaller, interconnected networks. Subnets eliminate the need for traffic to pass through extraneous routs, resulting in faster network speeds. Subnets were created to alleviate the shortage of IP addresses on the internet.

The purpose of subnetting is to establish a computer network that is quick, efficient, and robust. As networks grow in size and complexity, traffic must find more efficient pathways. Bottlenecks and congestion would arise if all network traffic travelled across the system at the same time, utilizing the same path, resulting in slow and wasteful backlogs. By creating a subnet, you can limit the number of routers that network traffic must pass through


## What is use of subnetting?

- **Reallocating IP Addresses:-** A limited number of host allocations are available for each class; for example, networks with more than 254 devices require a Class B allocation. Suppose a network administrator works with a Class B or C network and needs to allocate 150 hosts across three physical networks in three different cities. In that case, they must either request more address blocks for each network or divide the network into subnets that allow administrators to use one block of addresses across multiple physical networks.

- **Improves Network Speed:-** Subnetting divides the large network into small subnets, and the purpose of these subnets is to divide a huge network into a collection of smaller, interconnected networks to reduce traffic. Subnets eliminate the need for traffic to pass through extraneous routs, resulting in faster network speeds.

- **Improving Network Security:-** Subnetting helps network administrators to reduce network-wide threats by quarantining compromised areas of the network and making it more complex for trespassers to travel throughout an organization's network.

- **Reliving Network Congestion:-** If a large portion of an organization's traffic is intended to be shared regularly across a group of computers, putting them all on the same subnet can help reduce network traffic. Without a subnet, data packets from every other computer on the network would be visible to all computers and servers.

- **Efficiency:-** Subnetting is used to simplify network traffic by eliminating the need for additional routers. This ensures that the data being sent can move as quickly as possible to its destination, avoiding any potential detours that can slow it down.

## How does Subnetting work?

subnetting divides the network into small subnets. Routers are used to communicate between subnets, whereas each subnet allows its linked devices to communicate with each other. The size of a subnet is determined by the network technology used and the connection needs. Within the restrictions of the address space available for its usage, each organization is responsible for determining the number and size of the subnets it generates

1.The figure given below shows a 172.16.37.5 IPv4 Class B address. The Host ID is 37.5, and the Network Prefix is 172.16.0.0.
![Class B address](https://scaler.com/topics/images/working-of-subnetting-in-html.webp)

2. we generally fix MSB(Most Significant Bit) bits of the Host ID to generate the subnets. In the figure below, we fix one of the host's MSB(Most Significant Bit) bits to generate two network subnets. We cannot change network bits because if we change network bits, the whole network is changed.
![subnet](https://scaler.com/topics/images/creating-a-subnetting.webp)

3. To identify a subnet, we need a subnet mask which is calculated by putting ‘1’ in place of all Network ID bits and the number of bits we reserve in Host ID to generate the subnet. The subnet mask aims to route the data packet from the internet to its desired subnet network. A subnet mask also specifies which portion of an address should be utilized as the Subnet ID. A binary AND operation is used to apply the subnet mask to the whole network address. AND operations work by assuming that output is "true" if both inputs are "true." Otherwise, "false" is returned.

    This yields the Subnet ID. Routers use the Subnet ID to find the optimum path between subnetworks.
![subnet2](https://scaler.com/topics/images/generating-subnet-mask.webp)

4. If we want to generate variable length subnets, then we apply permutations on the number of bits reserved to create subnets. This subnetting is called Variable Length Subnet Masking (VLSM).

5. The broadcast address of a subnet is calculated by making all the remaining bits as‘1’of Host Id after having some bits reserved to represent the subnet.The broadcast address is used to broadcast the message to all the network hosts.
![subnet broadcast address](https://scaler.com/topics/images/broadcast-address.webp)


## Advantages of Subnetting
- Subnetting divides broadcast domains, allowing data to be routed more efficiently, boosting network performance and speed.
- We can subnet a single large network into smaller networks via subnetting. It is simple to handle small networks.
- Subnetting enhances the network's overall performance by removing redundant traffic.
- Subnetting reduces the requirement of an IP range.
- Subnets prevent devices from accessing the whole network, allowing businesses to control which gear and users have access to more sensitive data. It is possible to improve network security. 


## Disadvantages of Subnetting
- Subnetting increases the network's complexity. An experienced network administrator must manage the subnetted network.
- More subnets mean more IP addresses are wasted because each subnet has its own network address and broadcast address.
- As we increase more subnets in the network, we require more routers which increases the overall cost and makes the maintenance process challenging.
- Subnetting necessitates the purchase of expensive internal routers, switches, hubs, and bridges, among other items, which increases the overall network cost.