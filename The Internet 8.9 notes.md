# The Internet

Build a general picture of the network infrastructure

Be aware of the limitations of the physical network

- network bandwidth and latency
- Network infrastructure
- Characteristics of the physical network
- Network conceptual models
- Data transfer
- IP addresses and DNS

Understand that protocols are systems of rules

Learn that IP enables communication between devices

- What is a network?
    - a connection between two devices so they can communicate/exchange data

- What is the LAN?
    - Local Area Network - devices connected to each other via a network bridging device, like a centralized hub or switch, to form a network.
- What is a WLAN?
    - Wireless LAN - a network limited by the geographic capacity to connect devices
- What is the purpose of routers?
    - Routers are gateways to other networks, network devices that connect LAN's to other networks.
- What is the internet?
    - a network of networks

What is a server?

- What is a protocol, and what is its purpose? Name at least two protocols. [link](https://launchschool.com/lessons/4af196b9/assignments/a53e65ce)
    - a system of rules
    - "A set of rules governing the exchange or transmission of data."
    - It is a way to make sure all the different hardware and software are still able to communicate with each other the way they're supposed to despite the differences between the types of systems.
- Why are there so many different protocols?
    - they are used for a specific aspect of network communication, including differences in the overall aspect of communication, differences in use-cases, or differences in the way they address that particular aspect of communication
- What are different aspects of a message?
    - syntactical rules: govern the structure of the order of the elements in the message
    - message transfer rules: the overall flow/order of a message (metaphor: in a conversation, not speaking over one another, etc.)
    - the context of the message: is there a hierarchy? is the situation formal or informal? how is the information flowing: unidirectional or other? how often and under what circumstances can the message from one side be interrupted by or change over to the other side?
    - structure of the message itself?
    - how to transfer the message?
- Why do we think of protocols as layers?
    - "Trying to understand every aspect of it as a single end-to-end process would be extremely difficult. By modularizing it and structuring it into a layered system, we can zoom in on a particular layer to more clearly understand what is happening at that level of the system."

[Protocols](The%20Internet%206f6eebb804fb4f2488624eb7e6b30e11/Protocols%200415c3f4ccc64e72ba3c2e2c40a286c0.csv)

- What are the two most popular forms of computer network communication?
    - OSI model and IP Internet Protocol suite (also known as the TCP/IP or DoD model

What does map mean in this context? [link](https://launchschool.com/lessons/4af196b9/assignments/21ef33af)

- What is the difference between the OSI model and the IP suite?
    - The OSI model focuses on the functions and the IP suite focuses on scope

![The%20Internet%206f6eebb804fb4f2488624eb7e6b30e11/Untitled.png](The%20Internet%206f6eebb804fb4f2488624eb7e6b30e11/Untitled.png)

From [Launch School](https://launchschool.com/lessons/4af196b9/assignments/21ef33af)

OSI - Oh! A Protest Stops Terrible North Dakota Pipeline

IP - A Turtle Is Late

- What is data encapsulation?

    "Here we are essentially hiding data from one layer by encapsulating it within a data unit of the layer below" - what does below mean here?

- What is a PDU?
    - a Protocol Data Unit, a block of data transferred over a network. different protocols or layers have different names for it. At the link/data link layer: frame. Internet/network: packet. Transport layer: datagram (UDP) or segment (TCP)
- What does a PDU consist of?
    - header, data payload, sometimes trailer/footer
- What is the purpose of the header and the trailer?
    - provide metadata specific to that protocol. "an Internet Protocol (IP) packet header would include fields for the Source IP Address and the Destination IP Address, which would be used to correctly route the packet."
- What is the data payload?
    - the data itself
- How is the data payload the key to the way encapsulation is implemented?
- What is the benefit of this approach?
    - reread this part [link](https://launchschool.com/lessons/4af196b9/assignments/21ef33af)
- What does TCP stand for?

    TCP - Transmission Control Protocol

Physical layer

- What is the first layer of the network? What happens here?

- What is a bit?
- How can you send a bit?
- What is bandwidth? Is it the same throughout the network?
- What is latency?
    - Propagation delay
    - Transmission delay
    - Processing delay
    - Queuing delay
    - Total latency
- Last-mile latency
- RTT
- What is a node?
- Why do we learn about the physical limitations if we can't do much to change it?

car/lane metaphor

- layer 1: physical structure - transfer of bits (binary data) converted to signals
    - bit: pair of opposites. typically 1 on, 0 off. 8 bits = 1 byte. 100 bytes = KB. 1000 KB = 1 MB. sent by light, electricity, radio waves.
    - bandwidth - maximum transmission capacity of a device, measured by bit rate: number of bits that can be sent in one second (usually measured by seconds)
        - bandwidthssssecond
        - bandwidth varies across network
        - core bandwidth higher than home
        - lowest point in the overall connection
        - bandwidth bottleneck - point of change from high to low
        - can be serious with large amounts of data, but usually latency is more of an issue
    - latency - amount of time it takes for a bit to travel from source to requesting device or from one point in the network to another point in the network.
        - la-time
        - measure of delay
            - propagation delay: ratio between distance and speed, amount of time it takes for a message to travel from sender to receiver
            - transmission delay: amount of time to push data onto the physical link
            - processing delay: the amount of time it takes to be processed when crossing from one link to another
            - queuing delay: amount of time the data is waiting in the queue or buffer to be processed (since only so much data can be processed at one time)
            - total latency: sum of all of the above in ms
        - last-mile latency: delays close to the end-points, like getting network signal from ISP network to home network. at network edge (entry point into home or corporate LAN) there are shorter/more frequent hops
        - round-trip time (RTT): amount of time to send signal (apart from receiving it)
        - nodes. traceroute or tracert

    Why do we learn about the physical limitations if we can't do much to change it? [link](https://launchschool.com/lessons/4af196b9/assignments/097d7577)

    - electricity is slower over longer distances.
    - light - fiber optic cable thread of glass engineered to reflect light. expensive, hard to work with.
    - wireless: use radio signal to send bits from one place to another. mobile but short range.