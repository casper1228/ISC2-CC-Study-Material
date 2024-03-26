# L4 Network Security
# L4 網路安全
## Module 1: Understand Computer Networking
## 模組 1：了解電腦網絡
Domain D4.1.1, D4.1.2

### What is Networking
### 什麼是網絡
A network is simply two or more computers linked together to share data, information or resources.
网络就是将两台或多台计算机连接在一起，共享数据、信息或资源。

To properly establish secure data communications, it is important to explore all of the technologies involved in computer communications. From hardware and software to protocols and encryption and beyond, there are many details, standards and procedures to be familiar with.
要正确建立安全的数据通信，就必须探索计算机通信所涉及的所有技术。从硬件和软件到协议和加密等等，有许多细节、标准和程序需要熟悉。

#### Types of Networks
#### 網路類型
There are two basic types of networks:

* Local area network (LAN) - A local area network (LAN) is a network typically spanning a single floor or building. This is commonly a limited geographical area.
* Wide area network (WAN) - Wide area network (WAN) is the term usually assigned to the long-distance connections between geographically remote networks.
* 局域网（LAN）--局域网（LAN）通常是指横跨一个楼层或建筑物的网络。这通常是一个有限的地理区域。
* 广域网（WAN）--广域网（WAN）通常指地理位置遥远的网络之间的长距离连接。

#### Network Devices
#### 網路設備
* **Hubs** are used to connect multiple devices in a network. They’re less likely to be seen in business or corporate networks than in home networks. Hubs are wired devices and are not as smart as switches or routers.
**集线器**用于连接网络中的多个设备。与家庭网络相比，集线器较少出现在商业或企业网络中。集线器是有线设备，不如交换机或路由器智能。

* You might consider using **a switch**, or what is also known as an intelligent hub. Switches are wired devices that know the addresses of the devices connected to them and route traffic to that port/device rather than retransmitting to all devices. Offering greater efficiency for traffic delivery and improving the overall throughput of data, switches are smarter than hubs, but not as smart as routers. Switches can also create separate broadcast domains when used to create VLANs, which will be discussed later.
* 您可以考虑使用**交换机**，或也称为智能集线器的设备。交换机是一种有线设备，它知道与其连接的设备的地址，并将流量路由到该端口/设备，而不是向所有设备重新传输。交换机比集线器更智能，但不如路由器智能，它能提供更高的流量传输效率，提高数据的整体吞吐量。当用于创建 VLAN 时，交换机还可以创建独立的广播域，这将在后面讨论。

* **Routers** are used to control traffic flow on networks and are often used to connect similar networks and control traffic flow between them. Routers can be wired or wireless and can connect multiple switches. Smarter than hubs and switches, routers determine the most efficient “route” for the traffic to flow across the network.
* 路由器***用于控制网络上的流量，通常用于连接类似的网络并控制它们之间的流量。路由器可以是有线的，也可以是无线的，还可以连接多个交换机。路由器比集线器和交换机更智能，它能为网络中的流量确定最有效的 "路径"。

* **Firewalls** are essential tools in managing and controlling network traffic and protecting the network. A firewall is a network device used to filter traffic. It is typically deployed between a private network and the internet, but it can also be deployed between departments (segmented networks) within an organization (overall network). Firewalls filter traffic based on a defined set of rules, also called filters or access control lists.
**防火墙**是管理和控制网络流量以及保护网络的重要工具。防火墙是一种用于过滤流量的网络设备。它通常部署在专用网络和互联网之间，但也可以部署在组织（整体网络）内的部门（分段网络）之间。防火墙根据一组定义的规则（也称为过滤器或访问控制列表）过滤流量。

* A **server** is a computer that provides information to other computers on a network. Some common servers are web servers, email servers, print servers, database servers and file servers. All of these are, by design, networked and accessed in some way by a client computer. Servers are usually secured differently than workstations to protect the information they contain.
** 服务器**是向网络上其他计算机提供信息的计算机。常见的服务器包括网络服务器、电子邮件服务器、打印服务器、数据库服务器和文件服务器。根据设计，所有这些服务器都是联网的，并以某种方式被客户端计算机访问。服务器的安全保护通常不同于工作站，以保护其包含的信息。

* **Endpoints** are the ends of a network communication link. One end is often at a server where a resource resides, and the other end is often a client making a request to use a network resource. An endpoint can be another server, desktop workstation, laptop, tablet, mobile phone or any other end user device.
** 端点**是网络通信链路的两端。一端通常是资源所在的服务器，另一端通常是提出使用网络资源请求的客户端。端点可以是另一台服务器、台式工作站、笔记本电脑、平板电脑、手机或任何其他终端用户设备。

#### Other Networking Terms
#### 其他網路術語
* Ethernet (IEEE 802.3) is a standard that defines wired connections of networked devices. This standard defines the way data is formatted over the wire to ensure disparate devices can communicate over the same cables.
* 以太网（IEEE 802.3）是一种定义网络设备有线连接的标准。该标准定义了数据通过线路进行格式化的方式，以确保不同的设备可以通过相同的电缆进行通信。

* Media Access Control (MAC) Address - Every network device is assigned a Media Access Control (MAC) address. An example is 00-13-02-1F-58-F5. The first 3 bytes (24 bits) of the address denote the vendor or manufacturer of the physical network interface. No two devices can have the same MAC address in the same local network; otherwise an address conflict occurs.
* 媒体访问控制 (MAC) 地址 - 每个网络设备都分配有一个媒体访问控制 (MAC) 地址。例如 00-13-02-1F-58-F5。地址的前 3 个字节（24 位）表示物理网络接口的供应商或制造商。在同一个本地网络中，不能有两台设备拥有相同的 MAC 地址，否则会发生地址冲突。

* Internet Protocol (IP) Address - While MAC addresses are generally assigned in the firmware of the interface, IP hosts associate that address with a unique logical address. This logical IP address represents the network interface within the network and can be useful to maintain communications when a physical device is swapped with new hardware. Examples are 192.168.1.1 and 2001:db8::ffff:0:1.
* 互联网协议（IP）地址 - MAC 地址通常在接口固件中分配，而 IP 主机则将该地址与唯一的逻辑地址关联起来。该逻辑 IP 地址代表网络中的网络接口，当物理设备更换为新硬件时，该地址有助于保持通信。例如 192.168.1.1 和 2001:db8::fffff:0:1。

### Networking Models
### 網路模型
Many different models, architectures and standards exist that provide ways to interconnect different hardware and software systems with each other for the purposes of sharing information, coordinating their activities and accomplishing joint or shared tasks.
目前有许多不同的模式、架构和标准，提供了将不同的硬件和软件系统相互连接起来的方法，以便共享信息、协调活动和完成联合或共享任务。

Computers and networks emerge from the integration of communication devices, storage devices, processing devices, security devices, input devices, output devices, operating systems, software, services, data and people.
计算机和网络是通信设备、存储设备、处理设备、安全设备、输入设备、输出设备、操作系统、软件、服务、数据和人员的集成。

Translating the organization’s security needs into safe, reliable and effective network systems needs to start with a simple premise. The purpose of all communications is to exchange information and ideas between people and organizations so that they can get work done.
将组织的安全需求转化为安全、可靠和有效的网络系统，需要从一个简单的前提开始。所有通信的目的都是为了在人员和组织之间交换信息和想法，以便完成工作。

Those simple goals can be re-expressed in network (and security) terms such as:
这些简单的目标可以用网络（和安全）术语重新表述，例如

* Provide reliable, managed communications between hosts (and users)
* Isolate functions in layers
* Use packets (representation of data at L3 of OSI model ) as the basis of communication
* Standardize routing, addressing and control
* Allow layers beyond internetworking to add functionality
* Be vendor-agnostic, scalable and resilient
* 在主机（和用户）之间提供可靠、可管理的通信
* 分层隔离功能
* 使用数据包（OSI 模型第 3 层的数据表示）作为通信的基础
* 路由、寻址和控制标准化
* 允许互联网络以外的层增加功能
* 与供应商无关，具有可扩展性和弹性

In the most basic form, a network model has at least two layers:
最基本的网络模型至少有两层：

* UPPER LAYER APPLICATION: also known as the host or application layer, is responsible for managing the integrity of a connection and controlling the session as well as establishing, maintaining and terminating communication sessions between two computers. It is also responsible for transforming data received from the Application Layer into a format that any system can understand. And finally, it allows applications to communicate and determines whether a remote communication partner is available and accessible.
    * APPLICATION
        * APPLICATION 7
        * PRESENTATION 6
        * SESSION 5
* 上层应用层：又称主机层或应用层，负责管理连接的完整性和控制会话，以及建立、维护和终止两台计算机之间的通信会话。它还负责将从应用层接收到的数据转换成任何系统都能理解的格式。最后，它允许应用程序进行通信，并确定远程通信伙伴是否可用和可访问。
    * 应用程序
        * 应用 7
        * 演示 6
        * 会话 5

* LOWER LAYER: it is often referred to as the media or transport layer and is responsible for receiving bits from the physical connection medium and converting them into a frame. Frames are grouped into standardized sizes. Think of frames as a bucket and the bits as water. If the buckets are sized similarly and the water is contained within the buckets, the data can be transported in a controlled manner. Route data is added to the frames of data to create packets. In other words, a destination address is added to the bucket. Once we have the buckets sorted and ready to go, the host layer takes over.
    * DATA TRANSPORT
        * TRANSPORT 4
        * NETWORK 3
        * DATA LINK 2
        * PHYSICAL 1
* 下层：通常称为介质层或传输层，负责接收来自物理连接介质的比特并将其转换为帧。帧按标准尺寸分组。把帧看成一个桶，把比特看成水。如果水桶的大小相似，且水都装在水桶里，那么数据就能以受控的方式传输。路由数据被添加到数据帧中，形成数据包。换句话说，就是在水桶中添加目的地地址。一旦我们将水桶分类并准备就绪，主机层就会接手。
    * 数据传输
        * 传输 4
        * 网络 3
        * 数据链路 2
        * 物理 1

### Open Systems Interconnection (OSI) Model
### 開放系統互連 (OSI) 模型
The OSI Model was developed to establish a common way to describe the communication structure for interconnected computer systems. The OSI model serves as an abstract framework, or theoretical model, for how protocols should function in an ideal world, on ideal hardware. Thus, the OSI model has become a common conceptual reference that is used to understand the communication of various hierarchical components from software interfaces to physical hardware.
开发 OSI 模型是为了建立一种通用的方法来描述互连计算机系统的通信结构。OSI 模型是一个抽象框架或理论模型，用于描述在理想世界中，协议应如何在理想硬件上运行。因此，OSI 模型已成为一种通用的概念参考，用于理解从软件接口到物理硬件的各种分层组件的通信。

The OSI model divides networking tasks into seven distinct layers. Each layer is responsible for performing specific tasks or operations with the goal of supporting data exchange (in other words, network communication) between two computers. The layers are interchangeably referenced by name or layer number. For example, Layer 3 is also known as the Network Layer. The layers are ordered specifically to indicate how information flows through the various levels of communication. Each layer communicates directly with the layer above and the layer below it. For example, Layer 3 communicates with both the Data Link (2) and Transport (4) layers.
OSI 模型将网络任务分为七个不同的层。每一层负责执行特定的任务或操作，目的是支持两台计算机之间的数据交换（换言之，网络通信）。各层可通过名称或层号互换引用。例如，第 3 层也称为网络层。各层的具体排序是为了说明信息如何在各级通信中流动。每一层都与上一层和下一层直接通信。例如，第 3 层与数据链路层 (2) 和传输层 (4) 通信。

The Application, Presentation, and Session Layers (5-7) are commonly referred to simply as data. However, each layer has the potential to perform encapsulation (enforcement of data hiding and code hiding during all phases of software development and operational use. Bundling together data and methods is the process of encapsulation; its opposite process may be called unpacking, revealing, or using other terms. Also used to refer to taking any set of data and packaging it or hiding it in another data structure, as is common in network protocols and encryption.). Encapsulation is the addition of header and possibly a footer (trailer) data by a protocol used at that layer of the OSI model. Encapsulation is particularly important when discussing Transport, Network and Data Link layers (2-4), which all generally include some form of header. At the Physical Layer (1), the data unit is converted into binary, i.e., 01010111, and sent across physical wires such as an ethernet cable.  
应用层、表现层和会话层（5-7）通常被简单地称为数据层。不过，在软件开发和运行使用的各个阶段，每一层都有可能执行封装（执行数据隐藏和代码隐藏）。将数据和方法捆绑在一起就是封装过程；与之相反的过程可称为拆包、揭示或使用其他术语。也可用于指将任何一组数据打包或隐藏在另一种数据结构中（如网络协议和加密中常见的数据结构）。封装是指在 OSI 模型的该层中使用的协议添加了页眉和可能的页脚（尾部）数据。在讨论传输层、网络层和数据链路层（2-4）时，封装尤为重要，这些层通常都包含某种形式的报头。在物理层（1），数据单元被转换成二进制，即 01010111，并通过以太网电缆等物理电线发送。 

It's worth mapping some common networking terminology to the OSI Model so you can see the value in the conceptual model.
我们不妨将一些常见的网络术语与 OSI 模型进行映射，这样你就能看到概念模型的价值所在。

Consider the following examples: 
请看下面的例子： 

* When someone references an image file like a JPEG or PNG, we are talking about the Presentation Layer (6). 
* When discussing logical ports such as NetBIOS, we are discussing the Session Layer (5).
* When discussing TCP/UDP, we are discussing the Transport Layer (4).
* When discussing routers sending packets, we are discussing the Network Layer (3). 
* When discussing switches, bridges or WAPs sending frames, we are discussing the Data Link Layer (2).
* 当有人引用 JPEG 或 PNG 等图像文件时，我们讨论的是呈现层 (6)。
* 讨论 NetBIOS 等逻辑端口时，我们讨论的是会话层（5）。
* 讨论 TCP/UDP 时，我们讨论的是传输层（4）。
* 讨论路由器发送数据包时，我们讨论的是网络层（3）。
* 讨论交换机、网桥或 WAP 发送帧时，我们讨论的是数据链路层 (2)。

Encapsulation occurs as the data moves down the OSI model from Application to Physical. As data is encapsulated at each descending layer, the previous layer’s header, payload and footer are all treated as the next layer’s payload. The data unit size increases as we move down the conceptual model and the contents continue to encapsulate.  
数据在 OSI 模型中从应用层向下移动到物理层时会发生封装。数据在每一层向下封装时，上一层的页眉、有效载荷和页脚都被视为下一层的有效载荷。随着概念模型的下移，数据单元的大小也在增加，内容也在不断封装。 

The inverse action occurs as data moves up the OSI model layers from Physical to Application. This process is known as de-encapsulation  (or decapsulation). The header and footer are used to properly interpret the data payload and are then discarded. As we move up the OSI model, the data unit becomes smaller. The encapsulation/de-encapsulation process is best depicted visually below: 
当数据从物理层向应用层的 OSI 模型层移动时，就会发生相反的动作。这一过程称为去封装（或解封装）。页眉和页脚用于正确解释数据有效载荷，然后被丢弃。随着 OSI 模型的升级，数据单元会越来越小。下面是封装/解封装过程的最佳直观描述： 

|            |             |              |                 |                |
|------------|-------------|--------------|-----------------|----------------|
| 7          | Application |              |        DATA     |                |
| 6          | Presentation| Header -->   |      ||DATA     |                |
| 5          | Session     |              |     |||DATA     |                |
| 4          | Transport   |              |    ||||DATA     |                |
| 3          | Network     |              |   |||||DATA     |                |
| 2          | Data Link   |              |  ||||||DATA||   |   <-- Footer   |
| 1          | Physical    |              | |||||||DATA|||  |                |

|            |             |              |                 |                |
|------------|-------------|--------------|-----------------|----------------|
| 7          | 应用程序     |              |           DATA  |                |
| 6          | 展示        | Header -->    |         ||DATA  |                |
| 5          | 会话        |               |        |||DATA  |                |
| 4          | 传输        |               |       ||||DATA  |                |
| 3          | 网络        |               |       ||||DATA  |                |
| 2          | 数据链路    |                |    ||||||DATA|| | <-- 页脚       |
| 1          | 物理        |                | |||||||DATA|||  |                |

### Transmission Control Protocol/Internet Protocol (TCP/IP)
### 傳輸控制協定/網際網路協定 (TCP/IP)
The OSI model wasn’t the first or only attempt to streamline networking protocols or establish a common communications standard. In fact, the most widely used protocol today, TCP/IP, was developed in the early 1970s. The OSI model was not developed until the late 1970s. The TCP/IP protocol stack focuses on the core functions of networking.  
OSI 模型并不是简化网络协议或建立通用通信标准的首次或唯一尝试。事实上，当今使用最广泛的协议 TCP/IP 也是在 20 世纪 70 年代初开发的。OSI 模型直到 20 世纪 70 年代末才开发出来。TCP/IP 协议栈侧重于网络的核心功能。 

||TCP/IP Protocol Architecture Layers| |
|-|-----------------------------------|-|
||TCP/IP 協定架構層| |
|-|----------------------------------------------- -|-|
|Application Layer |Defines the protocols for the transport layer|
|Transport Layer   |Permits data to move among devices|
|Internet Layer    |Creates/inserts packets|
|Network Interface Layer 	|How data moves through the network|
|应用层定义传输层协议
|传输层允许数据在设备间移动
|创建/插入数据包
|网络接口层 |数据如何在网络中移动

The most widely used protocol suite is TCP/IP, but it is not just a single protocol; rather, it is a protocol stack comprising dozens of individual protocols. TCP/IP is a platform-independent protocol based on open standards. However, this is both a benefit and a drawback. TCP/IP can be found in just about every available operating system, but it consumes a significant amount of resources and is relatively easy to hack into because it was designed for ease of use rather than for security. 
使用最广泛的协议套件是 TCP/IP，但它并不仅仅是一个协议，而是由数十个单独协议组成的协议栈。TCP/IP 是一种基于开放标准、与平台无关的协议。然而，这既是优点也是缺点。几乎所有可用的操作系统中都有 TCP/IP 协议，但它消耗大量资源，而且相对容易被黑客入侵，因为它的设计初衷是为了方便使用，而不是为了安全。

At the Application Layer, TCP/IP protocols include **Telnet**, File Transfer Protocol (**FTP**), Simple Mail Transport Protocol (**SMTP**), and Domain Name Service (**DNS**). The two primary Transport Layer protocols of TCP/IP are **TCP and UDP**. **TCP is a full-duplex connection-oriented protocol, whereas UDP is a simplex connectionless protocol**. In the Internet Layer, **Internet Control Message Protocol (ICMP)** is used to determine the health of a network or a specific link. **ICMP is utilized by ping, traceroute and other network management tools**. The ping utility employs ICMP echo packets and bounces them off remote systems. Thus, you can use ping to determine whether the remote system is online, whether the remote system is responding promptly, whether the intermediary systems are supporting communications, and the level of performance efficiency at which the intermediary systems are communicating.
在应用层，TCP/IP 协议包括 **Telnet**、文件传输协议 (**FTP**)、简单邮件传输协议 (**SMTP**) 和域名服务 (**DNS**)。TCP/IP 的两个主要传输层协议是 **TCP 和 UDP**。**TCP 是一种面向连接的全双工协议，而 UDP 是一种单工无连接协议**。在互联网层，**互联网控制消息协议（ICMP）** 用于确定网络或特定链路的健康状况。ping、traceroute 和其他网络管理工具**都使用**ICMP。ping 实用程序采用 ICMP 回波数据包，并将其弹出远程系统。因此，你可以使用 ping 来确定远程系统是否在线、远程系统是否迅速响应、中间系统是否支持通信以及中间系统通信的性能效率水平。

* Application, Presentation and Session layers at OSI model is equivalent to Application Layer at TCP/IP, and the protocol suite is: FTP, Telnet, SNMP, LPD, TFPT, SMTP, NFS, X Window.
* Transport layer are the same between OSI model and TCP/IP model, protocol suite: TCP, UDP
* Network layer at OSI model is equivalent to Internet layer at TCP/IP model, and protocol suite is: IGMP, IP, ICMP
* Data link and Physical layer at OSI model is equivalent at Network Interface layer at TCP/IP, and protocol suite is: Ethernet, Fast Ethernet, Token Ring, FDDI
* OSI 模型中的应用层、呈现层和会话层相当于 TCP/IP 的应用层，协议套件包括： FTP、Telnet、SNMP、LPD、TFPT、SMTP、NFS、X Window： FTP、Telnet、SNMP、LPD、TFPT、SMTP、NFS、X Window。
* 传输层与 OSI 模型和 TCP/IP 模型相同，协议套件为 TCP、UDP
* OSI 模型的网络层等同于 TCP/IP 模型的互联网层，协议套件为 IGMP、IP、ICMP
* OSI 模型的数据链路层和物理层等同于 TCP/IP 模型的网络接口层，协议套件有：以太网、快速以太网、令牌环： 以太网、快速以太网、令牌环、FDDI

### Base concepts
### 基本概念
* Switch: A device that routes traffic to the port of a known device
* Server: A computer that provides information to other computers
* Firewall: A device that filters network traffic based on a defined set of rules
* Ethernet: A standard that defines wired communications of networked devices
* IP Address: Logical address representing the network interface
* MAC Address: Address that denotes the vendor or manufactures of the physical network interface
* 交换机： 将流量路由到已知设备端口的设备
* 服务器： 向其他计算机提供信息的计算机
* 防火墙： 防火墙：根据一组定义的规则过滤网络流量的设备
* 以太网： 定义网络设备有线通信的标准
* IP 地址： 代表网络接口的逻辑地址
* MAC 地址： 表示物理网络接口供应商或制造商的地址

### Internet Protocol (IPv4 and IPv6)
### 網際網路協定（IPv4 和 IPv6）
IPv4 provides a 32-bit address space. IPv6 provides a 128-bit address space. The first one is exhausted nowadays, but it is still used because of the NAT technology. 32 bits means 4 octets of 8 bits, which is represented in a dotted decimal notation such as 192.168.0.1, which means in binary notation 11000000 10101000 00000000 00000001
IPv4 提供 32 位地址空间。IPv6 提供 128 位地址空间。第一种地址空间如今已被淘汰，但由于使用了 NAT 技术，仍在使用。32 位意味着 4 个八进制 8 位，用点十进制表示，如 192.168.0.1，二进制表示为 11000000 10101000 00000000 00000001

IP hosts/devices associate an address with a unique logical address. An IPv4 address is expressed as four octets separated by a dot (.), for example, 216.12.146.140. Each octet may have a value between 0 and 255. However, **0 is the network itself (not a device on that network), and 255 is generally reserved for broadcast purposes**. Each address is subdivided into two parts: **the network number and the host**. The network number assigned by an external organization, such as the Internet Corporation for Assigned Names and Numbers (ICANN), represents the organization’s network. The host represents the network interface within the network.  
IP 主机/设备将地址与唯一的逻辑地址相关联。IPv4 地址以四个八位字节表示，中间用点（.）隔开，例如 216.12.146.140。每个八位字节的值在 0 到 255 之间。不过，**0 表示网络本身（而不是该网络上的设备），255 通常保留用于广播目的**。每个地址又分为两部分： **网络编号和主机**。由外部组织（如互联网名称与数字地址分配机构（ICANN））分配的网络号代表该组织的网络。主机代表网络内的网络接口。 

**To ease network administration, networks are typically divided into subnets**. Because subnets cannot be distinguished with the addressing scheme discussed so far, a separate mechanism, **the subnet mask**, is used to define the part of the address used for the subnet. The mask is usually converted to decimal notation like 255.255.255.0. **With the ever-increasing number of computers and networked devices, it is clear that IPv4 does not provide enough addresses for our needs.** To overcome this shortcoming, **IPv4 was sub-divided into public and private address ranges.** Public addresses are limited with IPv4, but this issue was addressed in part with private addressing. Private addresses can be shared by anyone, and it is highly likely that everyone on your street is using the same address scheme.  
**为了便于网络管理，网络通常被划分为子网**。由于子网无法用目前讨论的寻址方案来区分，因此需要使用一种单独的机制，即**子网掩码**，来定义用于子网的地址部分。掩码通常转换为十进制符号，如 255.255.255.0。**随着计算机和联网设备数量的不断增加，IPv4 提供的地址显然不能满足我们的需要。** 为了克服这一缺陷，IPv4 被细分为公共地址和专用地址范围。私有地址可由任何人共享，而且很可能你所在街道上的每个人都在使用相同的地址方案。 

The nature of the addressing scheme established by IPv4 meant that network designers had to start thinking in terms of IP address reuse. IPv4 facilitated this in several ways, such as its creation of the private address groups; this allows every LAN in every SOHO (small office, home office) situation to use addresses such as 192.168.2.xxx for its internal network addresses, without fear that some other system can intercept traffic on their LAN. This table shows the private addresses available for anyone to use:
IPv4 所建立的寻址方案的性质意味着网络设计者必须开始考虑 IP 地址的重复使用。IPv4 以多种方式促进了这一点，例如它创建了专用地址组；这使得 SOHO（小型办公室、家庭办公室）环境中的每个局域网都可以使用 192.168.2.xxx 等地址作为内部网络地址，而不必担心其他系统会拦截其局域网上的流量。该表显示了可供任何人使用的专用地址：

| RANGE |
|-------|
|10.0.0.0 to 10.255.255.254|
|172.16.0.0 to 172.31.255.254|
|192.168.0.0 to 192.168.255.254|

The first octet of **127 is reserved for a computer’s loopback address**. Usually, the address 127.0.0.1 is used. **The loopback address is used to provide a mechanism for self-diagnosis and troubleshooting at the machine level**. This mechanism allows a network administrator to treat a local machine as if it were a remote machine and ping the network interface to establish whether it is operational.
第一个八位位组 **127 保留给计算机的环回地址**。通常使用 127.0.0.1 地址。**环回地址用于提供一种在机器层面进行自我诊断和故障排除的机制**。该机制允许网络管理员将本地计算机视作远程计算机，通过 ping 网络接口来确定其是否正常运行。

IPv6 is a modernization of IPv4, which addressed a number of weaknesses in the IPv4 environment:
IPv6 是 IPv4 的现代化，它解决了 IPv4 环境中的一些弱点：

    * A much larger address field: IPv6 addresses are **128 bits**, which supports 2128 or 340,282,366,920,938,463,463,374,607,431,768,211,456 hosts. **This ensures that we will not run out of addresses**.
    * Improved security:** IPsec is an optional part of IPv4 networks, but a mandatory component of IPv6 networks**. This will help ensure the integrity and confidentiality of IP packets and allow communicating partners **to authenticate with each other**.
    * Improved quality of service (QoS): This will help services obtain an appropriate share of a network’s bandwidth.
  * 地址字段更大： IPv6 地址为**128 位**，可支持 2128 或 340,282,366,920,938,463,463,374,607,431,768,211,456 台主机。**这将确保我们不会耗尽地址**。
    * 提高安全性：** IPsec 是 IPv4 网络的可选部分，但却是 IPv6 网络的强制组成部分**。 这将有助于确保 IP 数据包的完整性和保密性，并允许通信伙伴**相互验证**。
    * 提高服务质量（QoS）： 这将有助于服务获得适当的网络带宽份额。

An IPv6 address is shown as **8 groups of four digits**. Instead of numeric (0-9) digits like IPv4, **IPv6 addresses use the hexadecimal range (0000-ffff) and are separated by colons (:)** rather than periods (.). An example IPv6 address is **2001:0db8:0000:0000:0000:ffff:0000:0001**. To make it easier for humans to read and type, it can be shortened by removing the leading zeros at the beginning of each field and substituting two colons (::) for the longest consecutive zero fields. All fields must retain at least one digit. After shortening, the example address above is rendered as 2001:db8::ffff:0:1, which is much easier to type. As in IPv4, there are some addresses and ranges that are reserved for special uses:
IPv6 地址显示为**8 组四位数**。IPv6 地址不使用 IPv4 的数字（0-9），而是使用十六进制范围（0000-ffff），并用冒号（:）** 而不是句号（.）分隔。一个 IPv6 地址示例是 **2001:0db8:0000:0000:0000:fffff:0000:0001**。为了便于人类阅读和输入，可以去掉每个字段开头的前导零，用两个冒号（::）代替最长的连续零字段，从而缩短地址。所有字段必须至少保留一位数字。经过缩写后，上面的示例地址将显示为 2001:db8::fffff:0:1，这就更容易输入了。与 IPv4 一样，有些地址和范围是为特殊用途保留的：

    * ::1 is the local loopback address, used the same as 127.0.0.1 in IPv4.
    * The range 2001:db8:: to 2001:db8:ffff:ffff:ffff:ffff:ffff:ffff is reserved for documentation use, just like in the examples above.
    * **fc00**:: to **fdff**:ffff:ffff:ffff:ffff:ffff:ffff:ffff are addresses reserved for internal network use and are not routable on the internet.
* ::1 是本地环回地址，用法与 IPv4 中的 127.0.0.1 相同。
    * 2001:db8:: 至 2001:db8:ffff:ffff:ffff:ffff:ffff:ffff:ffff 是保留给文档使用的范围，就像上面的例子一样。
    **fc00**:: 至 **fdff**:fffff:fffff:fffff:fffff:fffff:fffff:fffff 是保留给内部网络使用的地址，不能在互联网上路由。

### What is WiFi?
### 什麼是 WiFi？
Wireless networking is a popular method of connecting corporate and home systems because of the ease of deployment and relatively low cost. It has made networking more versatile than ever before. Workstations and portable systems are no longer tied to a cable but can roam freely within the signal range of the deployed wireless access points. However, with this freedom comes additional vulnerabilities.
无线网络因其易于部署和相对低廉的成本而成为连接企业和家庭系统的常用方法。它使联网比以往任何时候都更加灵活。工作站和便携式系统不再受电缆束缚，而是可以在部署的无线接入点信号范围内自由漫游。然而，这种自由也带来了更多的脆弱性。

Wi-Fi range is generally wide enough for most homes or small offices, and range extenders may be placed strategically to extend the signal for larger campuses or homes. Over time the Wi-Fi standard has evolved, with each updated version faster than the last.  
对于大多数家庭或小型办公室来说，Wi-Fi 的覆盖范围通常足够广，而对于较大的校园或家庭来说，可以战略性地放置范围扩展器来扩展信号。随着时间的推移，Wi-Fi 标准也在不断发展，每一个更新版本都比上一个版本更快。 

In a LAN, threat actors need to enter the physical space or immediate vicinity of the physical media itself. For wired networks, this can be done by placing sniffer taps onto cables, plugging in USB devices, or using other tools that require physical access to the network. By contrast, wireless media intrusions can happen at a distance. 
在局域网中，威胁行为者需要进入物理空间或物理介质本身的邻近区域。对于有线网络，可以通过在电缆上放置嗅探器、插入 USB 设备或使用其他需要物理访问网络的工具来实现。相比之下，无线介质入侵可以在远距离进行。

### Security of the Network 
### 網路安全
TCP/IP’s vulnerabilities are numerous. Improperly implemented TCP/IP stacks in various operating systems are vulnerable to various **DoS/DDoS attacks**, **fragment attacks**, **oversized packet attacks**, **spoofing attacks**, **and man-in-the-middle attacks**. TCP/IP (as well as most protocols) is also subject to passive attacks via monitoring or sniffing. Network monitoring, or sniffing, is the act of monitoring traffic patterns to obtain information about a network. 
TCP/IP 的漏洞很多。各种操作系统中实施不当的 TCP/IP 协议栈容易受到各种**DoS/DDoS 攻击**、**碎片攻击**、**超大数据包攻击**、**欺骗攻击**和中间人攻击**。TCP/IP （以及大多数协议）也会受到通过监控或嗅探进行的被动攻击。网络监控或嗅探是通过监控流量模式来获取网络信息的行为。

### Ports and Protocols (Applications/Services)
### 連接埠和協定（應用程式/服務）
* Physical Ports: Physical ports are the ports on the routers, switches, servers, computers, etc. that you connect the wires, e.g., fiber optic cables, Cat5 cables, etc., to create a network.
* 物理端口： 物理端口是指路由器、交换机、服务器、计算机等设备上的端口，您可以通过这些端口连接电线（如光纤电缆、Cat5 电缆等）来创建网络。

* Logical Ports: When a communication connection is established between two systems, it is done using ports. A logical port (also called a socket) is little more than an address number that both ends of the communication link agree to use when transferring data. Ports allow a single IP address to be able to support multiple simultaneous communications, each using a different port number. In the Application Layer of the TCP/IP model (which includes the Session, Presentation, and Application Layers of the OSI model) reside numerous application- or service-specific protocols. Data types are mapped using port numbers associated with services. For example, web traffic (or HTTP) is port 80. Secure web traffic (or HTTPS) is port 443. Table 5.4 highlights some of these protocols and their customary or assigned ports. You’ll note that in several cases a service (or protocol) may have two ports assigned, one secure and one insecure. When in doubt, systems should be implemented using the most secure version as possible of a protocol and its services.
* 逻辑端口： 在两个系统之间建立通信连接时，使用的是端口。逻辑端口（也称为套接字）只不过是通信链路两端同意在传输数据时使用的一个地址编号。端口允许单个 IP 地址同时支持多个通信，每个地址使用不同的端口号。在 TCP/IP 模型的应用层（包括 OSI 模型的会话层、呈现层和应用层）中，存在着许多特定于应用或服务的协议。数据类型使用与服务相关的端口号进行映射。例如，网络流量（或 HTTP）是 80 端口。安全网络流量（或 HTTPS）为 443 端口。表 5.4 重点介绍了其中一些协议及其惯用或指定的端口。您会注意到，在某些情况下，一项服务（或协议）可能分配了两个端口，一个安全端口和一个不安全端口。如有疑问，应尽可能使用最安全版本的协议及其服务来实施系统。

    * Well-known ports (0–1023): These ports are related to the common protocols that are at the core of the Transport Control Protocol/Internet Protocol (TCP/IP) model, Domain Name Service (DNS), Simple Mail Transfer Protocol (SMTP), etc.
    * Registered ports (1024–49151): These ports are often associated with proprietary applications from vendors and developers. While they are officially approved by the Internet Assigned Numbers Authority (IANA), in practice many vendors simply implement a port of their choosing. Examples include Remote Authentication Dial-In User Service (RADIUS) authentication (1812), Microsoft SQL Server (1433/1434) and the Docker REST API (2375/2376).
    * Dynamic or private ports (49152–65535): Whenever a service is requested that is associated with well-known or registered ports, those services will respond with a dynamic port that is used for that session and then released.
    * 知名端口（0-1023）： 这些端口与作为传输控制协议/互联网协议（TCP/IP）模型核心的常用协议、域名服务（DNS）、简单邮件传输协议（SMTP）等有关。
    * 注册端口（1024-49151）： 这些端口通常与供应商和开发人员的专有应用程序有关。虽然这些端口已获得互联网编号分配机构 (IANA) 的正式批准，但在实践中，许多供应商只是实施了自己选择的端口。例如，远程身份验证拨入用户服务 (RADIUS) 身份验证 (1812)、Microsoft SQL Server (1433/1434) 和 Docker REST API (2375/2376)。
    * 动态或专用端口（49152-65535）： 每当请求与众所周知或已注册端口相关联的服务时，这些服务都会响应一个动态端口，该端口用于该会话，然后释放。

### Secure Ports
### 安全端口
Some network protocols transmit information in clear text, meaning it is not encrypted and should not be used. Clear text information is subject to network sniffing. This tactic uses software to inspect packets of data as they travel across the network and extract text such as usernames and passwords. Network sniffing could also reveal the content of documents and other files if they are sent via insecure protocols. The table below shows some of the insecure protocols along with recommended secure alternatives.
某些网络协议以明文传输信息，这意味着这些信息没有加密，不应使用。明文信息会受到网络嗅探的攻击。这种手段使用软件来检查在网络上传输的数据包，并提取用户名和密码等文本。如果文件和其他文件是通过不安全协议发送的，网络嗅探还可能泄露文件和其他文件的内容。下表列出了一些不安全协议以及推荐的安全替代方案。

| Insecure Port | Description | Protocol | Secure Alternative Port | Protocol |
| 不安全端口 | 说明 | 协议 | 安全备用端口 | 协议
|---------------|-------------|----------|-------------------------|----------|
| 21 | Port 21, File Transfer Protocol (FTP) sends the username and password **using plaintext from the client to the server**. This could be intercepted by an attacker and later used to retrieve confidential information from the server. **The secure alternative, SFTP, on port 22 uses encryption to protect the user credentials and packets of data being transferred** | File Transfer Protocol 	|22* - SFTP	| Secure File Transfer Protocol|
| 文件传输协议（FTP）通过明文从客户端向服务器发送用户名和密码**。这可能会被攻击者截获，随后用于从服务器检索机密信息。**22 端口的安全替代方案 SFTP 使用加密技术保护用户凭证和传输的数据包** | 文件传输协议 |22* - SFTP | 安全文件传输协议

| 23 | Port 23, telnet, is used by many Linux systems and any other systems **as a basic text-based terminal**. All information to and from the host on a telnet connection is sent in plaintext and **can be intercepted by an attacker**. This includes username and password as well as all information that is being presented on the screen, since this interface is all text. **Secure Shell (SSH) on port 22 uses encryption to ensure that traffic between the host and terminal is not sent in a plaintext format**| Telnet | 22* - SSH	| Secure Shell|
| 23 | 端口 23，即 telnet，被许多 Linux 系统和任何其他系统**用作基本的文本终端**。通过 telnet 连接与主机之间的所有信息都以明文形式发送，**可被攻击者截获**。这包括用户名和密码以及屏幕上显示的所有信息，因为该界面是全文本的。端口 22 上的安全外壳（SSH）使用加密技术，确保主机与终端之间的通信不会以明文格式发送****| Telnet | 22* - SSH | Secure Shell | 22* - Telnet | 22* - SSH | Secure Shell | 22* - Telnet | 22* - SSH | Secure Shell

| 25 | Port 25, Simple Mail Transfer Protocol (SMTP) is the default unencrypted port for sending email messages. Since it is unencrypted, data contained within the emails could be discovered by network sniffing. The secure alternative is to use port 587 for SMTP using Transport Layer Security (TLS) which will encrypt the data between the mail client and the mail server| Simple Mail Transfer Protocol | 587 - SMTP	| SMTP with TLS |
| 25 | 25 端口，简单邮件传输协议（SMTP）是发送电子邮件的默认未加密端口。由于未加密，电子邮件中包含的数据可能会被网络嗅探器发现。安全的替代方法是使用传输层安全（TLS）将邮件客户端与邮件服务器之间的数据加密的 SMTP 587 端口。

| 37 | Port 37, Time Protocol, may be in use by legacy equipment and has mostly been replaced by using port 123 for Network Time Protocol (NTP). NTP on port 123 offers better error-handling capabilities, which reduces the likelihood of unexpected errors | Time Protocol | 123 - NTP | Network Time Protocol |
| 37 | 37 端口（时间协议）可能被传统设备使用，大部分已被用于网络时间协议（NTP）的 123 端口取代。123 端口上的 NTP 具有更好的错误处理能力，可降低出现意外错误的可能性。

| 53 | Port 53, Domain Name Service (DNS), is still used widely. However, using DNS over TLS (DoT) on port 853 protects DNS information from being modified in transit | Domain Name Service | 853 - DoT | DNS over TLS (DoT) |
| 53 | 53 端口，域名服务（DNS），仍在广泛使用。然而，在 853 端口使用 DNS over TLS (DoT)，可防止 DNS 信息在传输过程中被修改。

| 80 | Port 80, HyperText Transfer Protocol (HTTP) is the basis of nearly all web browser traffic on the internet. Information sent via HTTP is not encrypted and is susceptible to sniffing attacks. HTTPS using TLS encryption is preferred, as it protects the data in transit between the server and the browser. Note that this is often notated as SSL/TLS. Secure Sockets Layer (SSL) has been compromised is no longer considered secure. It is now recommended for web servers and clients to use Transport Layer Security (TLS) 1.3 or higher for the best protection | HyperText Transfer Protocol | 443 - HTTPS | HyperText Transfer Protocol (SSL/TLS) |
| 超文本传输协议（HTTP）是互联网上几乎所有网络浏览器流量的基础。通过 HTTP 发送的信息未经加密，容易受到嗅探攻击。使用 TLS 加密的 HTTPS 更受青睐，因为它能保护服务器和浏览器之间传输中的数据。请注意，这通常被标记为 SSL/TLS。安全套接字层（SSL）已被破解，不再被认为是安全的。现在建议网络服务器和客户端使用传输层安全（TLS）1.3 或更高版本，以获得最佳保护。

| 143 | Port 143, Internet Message Access Protocol (IMAP) is a protocol used for retrieving emails. IMAP traffic on port 143 is not encrypted and susceptible to network sniffing. The secure alternative is to use port 993 for IMAP, which adds SSL/TLS security to encrypt the data between the mail client and the mail server | Internet Message Access Protocol | 993 - IMAP | IMAP for SSL/TLS |
| 143 | 143 端口，互联网消息访问协议（IMAP）是一种用于检索电子邮件的协议。143 端口的 IMAP 流量未加密，容易被网络嗅探。

| 161/162 | Ports 161 and 162, Simple Network Management Protocol, are commonly used to send and receive data used for managing infrastructure devices. Because sensitive information is often included in these messages, it is recommended to use SNMP version 2 or 3 (abbreviated SNMPv2 or SNMPv3) to include encryption and additional security features. Unlike many others discussed here, all versions of SNMP use the same ports, so there is not a definitive secure and insecure pairing. Additional context will be needed to determine if information on ports 161 and 162 is secured or not | Simple Network Management Protocol | 161/162 - SNMP | SNMPv3 |
| 161/162 | 端口 161 和 162（简单网络管理协议）通常用于发送和接收用于管理基础设施设备的数据。由于这些信息中通常包含敏感信息，因此建议使用 SNMP 版本 2 或 3（缩写为 SNMPv2 或 SNMPv3），以包含加密和其他安全功能。与本文讨论的许多其他版本不同，SNMP 的所有版本都使用相同的端口，因此没有明确的安全和不安全配对。要确定端口 161 和 162 上的信息是否安全，还需要其他背景信息。

| 445 | Port 445, Server Message Block (SMB), is used by many versions of Windows for accessing files over the network. Files are transmitted unencrypted, and many vulnerabilities are well-known. Therefore, it is recommended that traffic on port 445 should not be allowed to pass through a firewall at the network perimeter. A more secure alternative is port 2049, Network File System (NFS). Although NFS can use encryption, it is recommended that NFS not be allowed through firewalls either | Server Message Block | 2049 - NFS | Network File System |
| 445 | 445 端口，即服务器消息块（SMB），被许多版本的 Windows 用于通过网络访问文件。文件传输未加密，而且存在许多众所周知的漏洞。因此，建议不要让 445 端口的流量通过网络外围的防火墙。更安全的选择是 2049 端口，即网络文件系统（NFS）。虽然 NFS 可以使用加密，但建议不允许 NFS 通过防火墙。

| 389 | Port 389, Lightweight Directory Access Protocol (LDAP), is used to communicate directory information from servers to clients. This can be an address book for email or usernames for logins. The LDAP protocol also allows records in the directory to be updated, introducing additional risk. Since LDAP is not encrypted, it is susceptible to sniffing and manipulation attacks. Lightweight Directory Access Protocol Secure (LDAPS) adds SSL/TLS security to protect the information while it is in transit | Lightweight Directory Access Protocol | 636 - LDAPS	| Lightweight Directory Access Protocol Secure |
| 轻量级目录访问协议（LDAP）389 端口用于将目录信息从服务器传送到客户端。这可以是用于电子邮件的地址簿或用于登录的用户名。LDAP 协议还允许更新目录中的记录，从而带来额外风险。由于 LDAP 没有加密，因此很容易受到嗅探和操纵攻击。轻量级目录访问协议安全（LDAPS）增加了 SSL/TLS 安全性，以保护传输中的信息。

### SYN, SYN-ACK, ACK

## Module 2 Understand Network (Cyber) Threats and Attacks
## 模組 2 了解網路（網路）威脅和攻擊
Domain D4.1.2, D4.2.2, D4.2.3

### Types of Threats
### 威脅類型
* Spoofing: an attack with the goal of **gaining access to a target system through the use of a falsified identity**. Spoofing can be used against IP addresses, MAC address, usernames, system names, wireless network SSIDs, email addresses, and many other types of logical identification.
* 欺骗：通过伪造身份**访问目标系统的攻击。欺骗可用于攻击 IP 地址、MAC 地址、用户名、系统名、无线网络 SSID、电子邮件地址和许多其他类型的逻辑标识。
  
* Phising: an attack that **attempts to misdirect legitimate users to malicious websites through** the abuse of **URLs or hyperlinks in emails could be considered phishing**.
* 网络钓鱼：通过滥用电子邮件中的**网址或超链接，**试图将合法用户误导到恶意网站的攻击可视为网络钓鱼**。

* DoS/DDoS: a denial-of-service (DoS) attack is a network resource consumption attack that has the **primary goal of preventing legitimate activity on a victimized system**. Attacks involving numerous unsuspecting secondary victim systems are known as distributed denial-of-service (DDoS) attacks.
* DoS/DDoS：拒绝服务（DoS）攻击是一种消耗网络资源的攻击，其**主要目标是阻止受害系统上的合法活动**。涉及众多不知情的次要受害系统的攻击被称为分布式拒绝服务 (DDoS) 攻击。

* Virus: The computer virus is perhaps the earliest form of malicious code to plague security administrators. As with biological viruses, **computer viruses have two main functions—propagation and destruction**. A virus is a **self-replicating** piece of code that spreads without the consent of a user, but frequently with their assistance (a user has to click on a link or open a file).
* 病毒： 计算机病毒可能是最早困扰安全管理员的恶意代码形式。与生物病毒一样，**计算机病毒有两个主要功能--传播和破坏**。病毒是一种**自我复制**的代码，它的传播不需要用户的同意，但经常需要用户的协助（用户必须点击链接或打开文件）。

* Worm: Worms pose a significant **risk to network security**. They contain the same destructive potential as other malicious code objects with an added twist—they propagate themselves without requiring any human intervention.
* 蠕虫： 蠕虫对网络安全构成重大**风险。它们与其他恶意代码对象具有相同的破坏潜力，但有一个额外的特点--它们不需要任何人工干预就能自我传播。

* Trojan: the Trojan is a software program **that appears benevolent but carries a malicious**, behind-the-scenes payload that has the potential to wreak havoc on a system or network. For example, ransomware often uses a Trojan to infect a target machine and then uses encryption technology to encrypt documents, spreadsheets and other files stored on the system with a key known only to the malware creator.
* 特洛伊木马：特洛伊木马是一种**的软件程序，它看似善良，却携带着恶意**，幕后的有效载荷有可能对系统或网络造成严重破坏。例如，勒索软件通常使用特洛伊木马感染目标机器，然后使用加密技术加密系统中存储的文档、电子表格和其他文件，加密密钥只有恶意软件制作者才知道。

* On-path attack: In an on-path attack, attackers place themselves between two devices, often between a web browser and a web server, to intercept or modify information that is intended for one or both of the endpoints. **On-path attacks** are also known as **man-in-the-middle (MITM) attacks**.
* 路径上攻击： 在路径上攻击中，攻击者将自己置于两台设备之间，通常是网络浏览器和网络服务器之间，以拦截或修改本应提供给一个或两个端点的信息。**路径上攻击**也称为**中间人（MITM）攻击**。

* Side-channel: A side-channel attack is a **passive**, **noninvasive attack** to **observe the operation of a device**. Methods include power monitoring, timing and fault analysis attacks.
* 侧信道： 侧信道攻击是一种**被动**、**非侵入式攻击，目的是**观察设备的运行**。方法包括电源监控、定时和故障分析攻击。

* Advanced Persistent Threat: Advanced persistent threat (APT) refers to **threats that demonstrate an unusually high level of technical and operational sophistication spanning months or even years**. APT attacks are often conducted by highly organized groups of attackers.
* 高级持续性威胁： 高级持续性威胁（APT）是指**技术和操作复杂程度异常高、持续时间长达数月甚至数年的威胁**。APT 攻击通常由高度组织化的攻击者群体实施。

* Insider Threat: Insider threats are threats that **arise from individuals who are trusted by the organization**. These could be disgruntled employees or employees involved in espionage. Insider threats are not always willing participants. A trusted user who falls victim to a scam could be an unwilling insider threat.
* 内部威胁：内部威胁是指**来自组织信任的个人**的威胁。这些人可能是心怀不满的员工或参与间谍活动的员工。内部威胁并不总是自愿参与的。受信任的用户成为骗局的受害者，可能是不情愿的内部威胁。

* Malware: A program that is inserted into a system, usually covertly, **with the intent of compromising the confidentiality, integrity or availability of the victim’s data**, applications or operating system or otherwise annoying or disrupting the victim.
* 恶意软件： 通常是暗中插入系统的程序，**目的是破坏受害者数据**、应用程序或操作系统的保密性、完整性或可用性，或以其他方式烦扰或破坏受害者。

* Ransomware: Malware used for the purpose of facilitating a ransom attack. Ransomware attacks often use cryptography to “lock” the files on an affected computer and require the payment of a ransom fee in return for the “unlock” code.
* 赎金软件： 用于勒索攻击的恶意软件。勒索软件攻击通常使用加密技术 "锁定 "受影响计算机上的文件，并要求支付赎金以换取 "解锁 "代码。

### Identify Threats and Tools Used to Prevent Them
### 識別威脅和用於預防威脅的工具
Here are some examples of steps that can be taken to protect networks.  
下面举例说明可以采取哪些措施来保护网络。 

* If a system doesn’t need a service or protocol, it should not be running. Attackers cannot exploit a vulnerability in a service or protocol that isn’t running on a system. 
* Firewalls can prevent many different types of attacks. Network-based firewalls protect entire networks, and host-based firewalls protect individual systems. 
* 如果系统不需要某个服务或协议，它就不应该运行。攻击者无法利用系统中未运行的服务或协议中的漏洞。
* 防火墙可以防止多种不同类型的攻击。基于网络的防火墙可以保护整个网络，基于主机的防火墙可以保护单个系统。
  
### Identify Threats and Tools Used to Prevent Them Continued
### 識別威脅和用於預防威脅的工具（續）
* Instrusion Detection System (IDS) is a form of monitoring to detect abnormal activity; it detects intrusion attempts and system failures. Identifies Threats, Do not prevent threats
* Host-based IDS (HIDS) monitors activity on a single computer. Identifies threats, Do not prevent Threats.
* Network-based IDS (NIDS) monitors and evaluates network activity to detect attacks or event anomalies. Identifies threats, Do not prevent Threats.
* SIEM gathers log data from sources across an enterprise to understand security concerns and apportion resources. Identifies threats, Do not prevent Threats.
* Anti-malware/Antivirus seeks to identify malicious software or processes. Identifies and Prevent threats.
* Scans evaluates the effectiveness of security controls. Identifies threats, Do not prevent Threats.
* Firewall filters network traffic - managers and controls network traffic and protects the network. Identifies and Prevent threats.
* Intrusion Protection System (IPS-NIPS/HIPS) is an active IDS automatically attempts to detect and block attacks before they reach target systems. Identifies and Prevent threats.
* 入侵检测系统（IDS）是一种检测异常活动的监控形式；它能检测入侵企图和系统故障。识别威胁，但不能防止威胁
* 基于主机的 IDS（HIDS）监控单台计算机上的活动。识别威胁，不阻止威胁。
* 基于网络的 IDS (NIDS) 监控和评估网络活动，以检测攻击或异常事件。识别威胁，不防范威胁。
* SIEM 收集来自整个企业的日志数据，以了解安全问题并分配资源。识别威胁，不阻止威胁。
* 反恶意软件/反病毒软件旨在识别恶意软件或进程。识别和预防威胁。
* 扫描评估安全控制的有效性。识别威胁，不预防威胁。
* 防火墙过滤网络流量 - 管理和控制网络流量并保护网络。识别和预防威胁。
* 入侵保护系统（IPS-NIPS/HIPS）是一种主动式 IDS，可在攻击到达目标系统之前自动检测和阻止攻击。识别和预防威胁。

### Intrusion Detection System (IDS)
### 入侵偵測系統（IDS）
**An intrusion occurs when an attacker is able to bypass or thwart security mechanisms and gain access to an organization’s resources.** Intrusion detection is a specific form of monitoring **that monitors recorded information and real-time events to detect abnormal activity indicating a potential incident or intrusion**. An intrusion detection system (IDS) **automates the inspection of logs and real-time system events to detect intrusion attempts and system failures**. An IDS is intended as part of a **defense-in-depth security plan**. **IDSs can** recognize attacks that come from external connections and attacks that spread internally. Once they detect a suspicious event, they respond by sending alerts or raising alarms. A primary goal of an IDS is to provide a means for a timely and accurate response to intrusions. 
**入侵检测是一种特定形式的监控**，通过监控记录的信息和实时事件来检测显示潜在事件或入侵**的异常活动。入侵检测系统（IDS）**自动检查日志和实时系统事件，以检测入侵企图和系统故障**。IDS 是**深度防御安全计划**的一部分。**IDS 可以**识别来自外部连接的攻击和内部传播的攻击。一旦检测到可疑事件，就会发出警报或报警。IDS 的主要目标是提供对入侵做出及时、准确响应的手段。

**IDS types are commonly classified as host-based and network-based. A host-based IDS (HIDS) monitors a single computer or host. A network-based IDS (NIDS) monitors a network by observing network traffic patterns.**
** IDS 通常分为基于主机和基于网络两种类型。基于主机的 IDS（HIDS）监控单台计算机或主机。基于网络的 IDS（NIDS）通过观察网络流量模式监控网络。

**Host-based Intrusion Detection System (HIDS)**: A HIDS monitors activity **on a single computer**, including **process calls and information recorded in system, application, security and host-based firewall logs**. It can often examine events in more detail than a NIDS can, and it can pinpoint specific files compromised in an attack. **It can also track processes employed by the attacker.** A benefit of HIDSs over NIDSs is that HIDSs can detect anomalies on the host system that NIDSs cannot detect. For example, **a HIDS can detect infections where an intruder has infiltrated a system and is controlling it remotely.** HIDSs are more costly to manage than NIDSs because they require administrative attention on each system, whereas NIDSs usually support centralized administration. A HIDS cannot detect network attacks on other systems.
**基于主机的入侵检测系统（HIDS）**： HIDS 监控单台计算机上的***活动，包括系统、应用程序、安全和主机防火墙日志中记录的***进程调用和信息。它通常能比 NIDS 更详细地检查事件，并能确定在攻击中受损的特定文件。** 它还可以跟踪攻击者使用的进程。** HIDS 相对于 NIDS 的一个优势是，HIDS 可以检测到 NIDS 检测不到的主机系统上的异常情况。** HIDS 的管理成本比 NIDS 高，因为 HIDS 需要对每个系统进行管理，而 NIDS 通常支持集中管理。HIDS 无法检测对其他系统的网络攻击。

**Network Intrusion Detection System (NIDS)**: A NIDS monitors and **evaluates network activity to detect attacks or event anomalies**. **It cannot monitor the content of encrypted traffic but can monitor other packet details**. A single NIDS can monitor **a large network by using remote sensors to collect data at key network locations that send data to a central management console**. These sensors can monitor traffic at **routers, firewalls, network switches that support port mirroring, and other types of network taps**. **A NIDS has very little negative effect on the overall network performance**, and when it is deployed on a single-purpose system, it doesn’t adversely affect performance on any other computer. A NIDS is usually able to detect the initiation of an attack or ongoing attacks, but they can’t always provide information about the success of an attack. They won’t know if an attack affected specific systems, user accounts, files or applications.
**网络入侵检测系统（NIDS）**： 网络入侵检测系统监测和**评估网络活动，以检测攻击或异常事件**。**它不能监控加密流量的内容，但可以监控其他数据包细节**。通过使用远程传感器在关键网络位置收集数据，并将数据发送到中央管理控制台**，单个 NIDS 可监控**个大型网络。这些传感器可以监控**路由器、防火墙、支持端口镜像的网络交换机以及其他类型的网络窃听**的流量。**NIDS 对整体网络性能的负面影响很小**，当它部署在单用途系统上时，不会对任何其他计算机的性能产生不利影响。NIDS 通常能够检测到攻击的发起或正在进行的攻击，但并不总能提供攻击是否成功的信息。它们不知道攻击是否影响了特定系统、用户账户、文件或应用程序。

**Security Information and Event Management (SIEM)**: Security management involves the **use of tools that collect information about the IT environment from many disparate sources to better examine the overall security of the organization and streamline security efforts**. These tools are generally known as **security information and event management** (or S-I-E-M, pronounced “SIM”) solutions. The general **idea of a SIEM solution is to gather log data from various sources across the enterprise to better understand potential security concerns and apportion resources accordingly**. SIEM systems can be used along with other components (defense-in-depth) as part of an overall information security program.
**安全信息和事件管理（SIEM）**： 安全管理包括**使用工具，从许多不同来源收集有关 IT 环境的信息，以便更好地检查组织的整体安全性并简化安全工作**。这些工具通常被称为**安全信息和事件管理**（或 S-I-E-M，读作 "SIM"）解决方案。SIEM 解决方案的一般**理念是从整个企业的各种来源收集日志数据，以便更好地了解潜在的安全问题，并相应地分配资源**。SIEM 系统可与其他组件（深度防御）一起使用，作为整体信息安全计划的一部分。

### Preventing Threats
### 預防威脅
* Keep systems and applications up to date. Vendors regularly release patches to correct bugs and security flaws, but these only help when they are applied. Patch management ensures that systems and applications are kept up to date with relevant patches.
* 及时更新系统和应用程序。供应商会定期发布补丁程序来修正漏洞和安全缺陷，但这些补丁程序只有在应用时才会发挥作用。补丁管理可确保系统和应用程序不断更新相关补丁。
* 
* **Remove or disable unneeded services and protocols**. If a system doesn’t need a service or protocol, it should not be running. Attackers cannot exploit a vulnerability in a service or protocol that isn’t running on a system. As an extreme contrast, imagine a web server is running every available service and protocol. It is vulnerable to potential attacks on any of these services and protocols.
  * 删除或禁用不需要的服务和协议**。如果系统不需要某项服务或协议，它就不应该运行。攻击者无法利用系统中未运行的服务或协议中的漏洞。与此形成鲜明对比的是，假设网络服务器正在运行所有可用的服务和协议。它很容易受到任何这些服务和协议的潜在攻击。
    
**Use intrusion detection and prevention systems**. As discussed, intrusion detection and prevention systems observe activity, attempt to detect threats and provide alerts. They can often block or stop attacks.
** 使用入侵检测和防御系统**。如前所述，入侵检测和防御系统可以观察活动，尝试检测威胁并发出警报。它们通常可以阻止或制止攻击。 
 
* **Use up-to-date anti-malware software**. We have already covered the various types of malicious code such as viruses and worms. A primary countermeasure is anti-malware software.
* 使用最新的反恶意软件**。我们已经介绍了病毒和蠕虫等各类恶意代码。反恶意软件是一项主要对策。 

* **Use firewalls**. Firewalls can prevent many different types of threats. Network-based firewalls protect entire networks, and host-based firewalls protect individual systems. This chapter included a section describing how firewalls can prevent attacks.
* 使用防火墙**。防火墙可以防止多种不同类型的威胁。基于网络的防火墙可保护整个网络，基于主机的防火墙可保护单个系统。本章有一节介绍防火墙如何防止攻击。

**Antivirus**: it is a requirement for **compliance with the Payment Card Industry Data Security Standard (PCI DSS)**. Antivirus systems try to identify malware based **on the signature of known malware or by detecting abnormal activity on a system**. This identification is done with various **types of scanners, pattern recognition and advanced machine learning algorithms**. Anti-malware now goes beyond just virus protection as modern solutions try to provide a more holistic approach detecting rootkits, ransomware and spyware. Many endpoint solutions also include software firewalls and IDS or IPS systems.
**防病毒**：这是**符合支付卡行业数据安全标准（PCI DSS）**的要求。反病毒系统会根据已知恶意软件的签名或通过检测系统上的异常活动**来识别恶意软件。这种识别是通过各种**类型的扫描仪、模式识别和先进的机器学习算法**完成的。现在的反恶意软件已不仅仅是病毒防护，现代解决方案试图提供一种更全面的方法来检测 rootkit、勒索软件和间谍软件。许多端点解决方案还包括软件防火墙和 IDS 或 IPS 系统。

**Scans**: Regular vulnerability and port scans are a good way to evaluate the effectiveness of security controls used within an organization. They may reveal areas where patches or security settings are insufficient, where new vulnerabilities have developed or become exposed, and where security policies are either ineffective or not being followed. Attackers can exploit any of these vulnerabilities.
**扫描**： 定期的漏洞和端口扫描是评估组织内使用的安全控制有效性的好方法。扫描可能会发现补丁或安全设置不足的地方、新漏洞已开发或暴露的地方，以及安全策略无效或未得到遵守的地方。攻击者可以利用其中任何一个漏洞。

**Firewalls**: Early computer security engineers borrowed that name for the devices and services that isolate network segments from each other, as a security measure. As a result, firewalling refers to the process of designing, using or operating different processes in ways that **isolate high-risk activities from lower-risk ones**. **Firewalls enforce policies by filtering network traffic based on a set of rules.** While a firewall should always be placed at internet gateways, other internal network considerations and conditions determine where a firewall would be employed, such as network zoning or segregation of different levels of sensitivity. Firewalls have rapidly evolved over time to provide enhanced security capabilities. **It integrates a variety of threat management capabilities into a single framework, including proxy services, intrusion prevention services (IPS) and tight integration with the identity and access management (IAM) environment to ensure only authorized users are permitted to pass traffic across the infrastructure.** While firewalls can manage traffic **at Layers 2 (MAC addresses)**, **3 (IP ranges)** and **7 (application programming interface (API)** and **application firewalls**), **the traditional implementation has been to control traffic at Layer 4**. Traditional firewalls have PORTS IP Address, IDS/IPS, Antivirus Gateway, WebProxy, VPN; NG Firewalls have PORTS IP Address, IAM Attributes, IDS/IPS, WebProxy, Anti-Bot, Antivirus Gateway, VPN, FaaS.
**防火墙**： 早期的计算机安全工程师借用这一名称来称呼将网段相互隔离的设备和服务，作为一种安全措施。因此，防火墙指的是设计、使用或操作不同程序的过程，这些程序**将高风险活动与低风险活动隔离**。**虽然防火墙应始终置于互联网网关处，但其他内部网络考虑因素和条件也会决定在何处使用防火墙，例如网络分区或不同敏感度级别的隔离。防火墙随着时间的推移迅速发展，提供了更强的安全功能。**防火墙可在第 2 层（MAC 地址）**、第 3 层（IP 范围）**和第 7 层（应用编程接口（API）**和**应用防火墙**）管理流量，但传统的实施方式是在第 4 层控制流量**。传统防火墙有 PORTS IP 地址、IDS/IPS、防病毒网关、WebProxy、VPN；下一代防火墙有 PORTS IP 地址、IAM 属性、IDS/IPS、WebProxy、反僵尸、防病毒网关、VPN、FaaS。

**Intrusion Prevention System (IPS)**: An intrusion prevention system (IPS) is a special type of active IDS **that automatically attempts to detect and block attacks before they reach target systems**. A distinguishing difference between an IDS and an IPS is that the **IPS is placed in line with the traffic**. In other words, **all traffic must pass through the IPS and the IPS can choose what traffic to forward and what traffic to block after analyzing it**. This allows the IPS to prevent an attack from reaching a target. Since IPS systems are most effective at preventing network-based attacks, it is common to see the IPS function integrated into firewalls. Just like IDS, there are Network-based IPS (NIPS) and Host-based IPS (HIPS).
**入侵防御系统（IPS）**： 入侵防御系统（IPS）是一种特殊类型的主动式 IDS，**能在攻击到达目标系统之前**自动检测和阻止攻击。IDS 与 IPS 的一个显著区别是，**IPS 与流量**一致。换句话说，**所有流量都必须通过 IPS，IPS 可以在分析后选择转发哪些流量和阻止哪些流量**。这样，IPS 就能阻止攻击到达目标。由于 IPS 系统能最有效地防止基于网络的攻击，因此 IPS 功能通常被集成到防火墙中。与 IDS 一样，IPS 也分为基于网络的 IPS（NIPS）和基于主机的 IPS（HIPS）。

## Module 3 Understand Network Security Infrastructure
## 模組 3 了解網路安全基礎設施
Domain D4.3.1, D4.3.2

### On-Premises Data Centers
### 本機資料中心
When it comes to data centers, there are two primary options: organizations can **outsource the data center or own the data center**. If the data center is owned, it will likely be built on premises. A place, like a building for the data center is needed, along with **power, HVAC, fire suppression and redundancy**.
说到数据中心，主要有两种选择：企业可以**外包数据中心，也可以**自有数据中心。如果拥有数据中心，则很可能是在办公场所内建造。数据中心需要一个像大楼一样的地方，还需要**电源、暖通空调、灭火和冗余**。

* **Data Center/Closets**: The facility wiring infrastructure is **integral to overall information system security and reliability**. **Protecting access to the physical layer of the network is important** in minimizing intentional or unintentional damage. **Proper protection of the physical site** must address these sorts of security challenges. Data centers and wiring closets may include the following: Phone, network, special connections; ISP or telecommunications provider equipment; Servers; Wiring and/or switch components.
** 数据中心/机柜**： 设施布线基础设施是整个信息系统安全性和可靠性的**组成部分。**保护对网络物理层的访问对于**减少有意或无意的破坏非常重要。**对物理站点进行适当保护**必须应对这些安全挑战。数据中心和配线间可能包括以下内容： 电话、网络、特殊连接；ISP 或电信供应商设备；服务器；布线和/或交换机组件。

* **Heating, Ventilation and Air Conditioning (HVAC) / Environmental**: High-density equipment and equipment within enclosed spaces **requires adequate cooling and airflow**. Well-established standards for the operation of computer equipment exist, and equipment is tested against these standards. For example, the recommended range for optimized maximum uptime and hardware life is **from 18° to 27°C**, and it is recommended that a rack have three temperature sensors, positioned at the top, middle and bottom of the rack, to measure the actual operating temperature of the environment. Proper management of data center temperatures, including cooling, is essential. **Cooling is not the only issue with airflow**: Contaminants like dust and noxious fumes require appropriate controls to minimize their impact on equipment. Monitoring for water or gas leaks, sewer overflow or HVAC failure should be integrated into the building control environment, with appropriate alarms to signal to organizational staff. Contingency planning to respond to the warnings should prioritize the systems in the building, so the impact of a major system failure on people, operations or other infrastructure can be minimized.
** 供暖、通风和空调（HVAC）/环境**： 高密度设备和封闭空间内的设备**需要足够的冷却和气流**。计算机设备的运行有既定的标准，并根据这些标准对设备进行测试。例如，优化最大正常运行时间和硬件寿命的推荐范围是**18°至 27°C**，建议在机架的顶部、中部和底部安装三个温度传感器，以测量环境的实际运行温度。正确管理数据中心的温度（包括冷却）至关重要。**冷却并不是气流**的唯一问题： 灰尘和有害气体等污染物需要适当的控制，以尽量减少其对设备的影响。水或气体泄漏、下水道溢流或暖通空调故障的监测应纳入楼宇控制环境，并发出适当的警报，向组织员工发出信号。应对警报的应急计划应优先考虑楼宇内的系统，以便将重大系统故障对人员、运营或其他基础设施的影响降至最低。

* Power: Data centers and information systems in general consume a tremendous amount of electrical power, **which needs to be delivered both constantly and consistently**. Wide fluctuations in the quality of power affect system lifespan, while disruptions in supply completely stop system operations. Power at the site is always an integral part of data center operations. Regardless of fuel source, backup generators must be sized to provide for the critical load (the computing resources) and the supporting infrastructure. Similarly, battery backups must be properly sized to carry the critical load until generators start and stabilize. As with data backups, testing is necessary to ensure the failover to alternate power works properly.
* 电力： 数据中心和一般信息系统消耗大量电力，**需要持续稳定地提供电力。电力质量的大幅波动会影响系统的使用寿命，而电力供应的中断则会完全停止系统的运行。现场供电始终是数据中心运营不可或缺的一部分。无论使用哪种燃料，备用发电机的大小都必须满足关键负载（计算资源）和支持基础设施的需要。同样，备用电池的大小也必须适当，以便在发电机启动和稳定之前提供关键负载。与数据备份一样，有必要进行测试，以确保故障切换到备用电源时能够正常工作。

* Fire Suppression: For server rooms, appropriate fire detection/suppression must be considered based on the size of the room, typical human occupation, egress routes and risk of damage to equipment. For example, water used for fire suppression would cause more harm to servers and other electronic components. Gas-based fire suppression systems are more friendly to the electronics, but can be toxic to humans.
* 灭火： 对于服务器机房，必须根据机房的大小、典型的人员占用情况、逃生路线和损坏设备的风险来考虑适当的火灾探测/灭火。例如，用水灭火会对服务器和其他电子元件造成更大伤害。气体灭火系统对电子设备更友好，但对人体可能有毒。

Which of the following is typically associated with an on-premises data center? **Fire suppression is associated**, **HVAC is associated**, **Power is associated** are all associated with an on-premises data center.
以下哪项通常与内部数据中心有关？**灭火**、**暖通空调**、**供电**都与内部数据中心有关。

Which of the following is not a source of redundant power? **HVAC is not a source of redundant power**, but it is something that needs to be protected by a redundant power supply, which is what the other three options will provide. What happens if the HVAC system breaks and equipment gets too hot? If the temperature in the data center gets too hot, then there is a risk that the server will shut down or fail sooner than expected, which presents a risk that data will be lost. So that is another system that requires redundancy in order to reduce the risk of data loss. But it is not itself a source of redundant power.
以下哪项不是冗余电源？**暖通空调系统不是冗余电源**，但它需要冗余电源的保护，这正是其他三个选项所能提供的。如果暖通空调系统发生故障，设备温度过高，会发生什么情况？如果数据中心的温度过高，服务器就有可能提前关闭或发生故障，从而带来数据丢失的风险。因此，这是另一个需要冗余以降低数据丢失风险的系统。但它本身并不是冗余电源。

### Redundancy
### 冗餘
The concept of redundancy is to design systems with **duplicate components so that if a failure were to occur, there would be a backup**. This can apply to the data center as well. Risk assessments pertaining to the data center should identify when multiple separate utility service entrances are necessary for redundant communication channels and/or mechanisms.  
冗余的概念是设计具有**个重复组件的系统，以便在发生故障时有一个备份**。这也适用于数据中心。与数据中心有关的风险评估应确定何时需要多个独立的公用设施服务入口，以实现冗余通信渠道和/或机制。 

If the organization requires full redundancy, devices should have two power supplies connected to diverse power sources. Those power sources would be backed up by batteries and generators. In a high-availability environment, even generators would be redundant and fed by different fuel types. 
如果组织需要完全冗余，设备应配备两个连接到不同电源的电源。这些电源将由电池和发电机提供支持。在高可用性环境中，即使发电机也是冗余的，并由不同类型的燃料供电。

### Memorandum of Understanding (MOU)/Memorandum of Agreement (MOA) 
### 諒解備忘錄 (MOU)/協議備忘錄 (MOA)
Some organizations seeking to minimize downtime and **enhance BC (Business Continuity) and DR (Disaster Recovery) capabilities** will create agreements with other, similar organizations. They agree that if one of the parties experiences an emergency and cannot operate within their own facility, the other party will share its resources and let them operate within theirs in order to maintain critical functions. These agreements often even include competitors, because their facilities and resources meet the needs of their particular industry. 
一些组织为了尽量减少停机时间，**增强业务连续性（BC）和灾难恢复（DR）能力，**会与其他类似组织签订协议。他们同意，如果其中一方遇到紧急情况，无法在自己的设施内运行，另一方将共享资源，让他们在自己的设施内运行，以维持关键功能。这些协议通常甚至包括竞争对手，因为他们的设施和资源符合其特定行业的需要。

**These agreements are called joint operating agreements (JOA)** or memoranda of understanding (MOU) or memoranda of agreement (MOA). Sometimes these agreements are mandated by regulatory requirements, or they might just be part of the administrative safeguards instituted by an entity within the guidelines of its industry. 
**这些协议被称为联合运营协议（JOA）** 或谅解备忘录（MOU）或协议备忘录（MOA）。这些协议有时是监管要求规定的，有时可能只是某个实体在其行业准则范围内制定的行政保障措施的一部分。

The difference between an MOA or MOU  and an SLA is that a Memorandum of Understanding is more directly related to what can be done with a system or the information. 
MOA 或 MOU 与 SLA 的区别在于，Memorandum of Understanding（谅解备忘录）与系统或信息的功能更直接相关。

The service level agreement goes down to the granular level. For example, if I'm outsourcing the IT services, then I will need to have two full-time technicians readily available, at least from Monday through Friday from eight to five. With cloud computing, I need to have access to the information in my backup systems within 10 minutes. An SLA specifies the more intricate aspects of the services.  
服务水平协议要细化到每个细节。例如，如果我将 IT 服务外包，那么我需要两名全职技术人员随时待命，至少从周一到周五的八点到五点。通过云计算，我需要在 10 分钟内访问备份系统中的信息。服务水平协议（SLA）规定了服务中更为复杂的方面。

We must be very cautious when outsourcing with cloud-based services, because we have to make sure that we understand exactly what we are agreeing to. If the SLA promises 100 percent accessibility to information, is the access directly to you at the moment, or is it access to their website or through their portal when they open on Monday? That's where you'll rely on your legal team, who can supervise and review the conditions carefully before you sign the dotted line at the bottom.
在使用基于云的服务时，我们必须非常谨慎，因为我们必须确保清楚地了解我们所同意的是什么。如果服务水平协议（SLA）承诺对信息的可访问性达到 100%，那么这种访问是目前直接对您的访问，还是周一开放时通过其网站或门户网站的访问？这就需要依靠您的法律团队了，他们可以在您签署底部虚线之前进行监督并仔细审查条件。

### Cloud
＃＃＃ 雲
Cloud computing is usually associated with an internet-based set of computing resources, and typically sold as a service, provided by a **cloud service provider (CSP)**. **It is a very scalable, elastic and easy-to-use “utility” for the provisioning and deployment of Information Technology (IT) services**. There are various definitions of what cloud computing means according to the leading standards, **including NIST**. This NIST definition is commonly used around the globe, cited by professionals and others alike to clarify what the term “cloud” means: “**a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (such as networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction.**” NIST SP 800-145 
云计算通常与一套基于互联网的计算资源相关联，通常作为一种服务出售，由**云服务提供商（CSP）**提供。**它是一种可扩展性强、弹性大且易于使用的 "实用工具"，用于信息技术（IT）服务的供应和部署**。根据包括 NIST 在内的***主要标准，云计算的含义有多种定义。NIST 的这一定义在全球范围内被广泛使用，专业人士和其他人都引用这一定义来阐明 "云 "的含义： "**一种模式，用于实现对可配置计算资源（如网络、服务器、存储、应用程序和服务）共享池的无处不在、便捷、按需的网络访问，这些资源可以快速调配和释放，只需极少的管理工作或服务提供商互动**"。NIST SP 800-145 

### Cloud Characteristics
### 雲端特性
Cloud-based assets include any resources that an organization accesses using cloud computing. **Cloud computing refers to on-demand access to computing resources available from almost anywhere**, **and cloud computing resources are highly available and easily scalable**. Organizations typically lease cloud-based resources from outside the organization. Cloud computing has many benefits for organizations, which include but are not limited to: 
云计算资产包括组织使用云计算访问的任何资源。**云计算是指按需访问几乎可从任何地方获取的计算资源**，**云计算资源具有高度可用性和易扩展性**。组织通常从组织外部租用云计算资源。云计算为组织带来了许多好处，包括但不限于以下方面： 

* Resource Pooling
    * Broadnetwork Access
    * Rapid Elasticity
    * Measured Service
    * On-Demand Self-Service
* 资源池
    * 广泛的网络接入
    * 快速弹性
    * 计量服务
    * 按需自助服务

* Usage is metered and priced according to units (or instances) consumed. This can also be billed back to specific departments or functions.
* Reduced cost of ownership. There is no need to buy any assets for everyday use, no loss of asset value over time and a reduction of other related costs of maintenance and support.
* Reduced energy and cooling costs, along with “green IT” environment effect with optimum use of IT resources and systems.
* Allows an enterprise to scale up new software or data-based services/solutions through cloud systems quickly and without having to install massive hardware locally.
* 对使用情况进行计量，并根据消耗的单位（或实例）定价。也可向特定部门或职能部门收取费用。
* 降低拥有成本。无需为日常使用购买任何资产，资产价值不会随着时间的推移而损失，并可降低其他相关的维护和支持成本。
* 降低能源和冷却成本，同时优化使用 IT 资源和系统，实现 "绿色 IT "环境效应。
* 允许企业通过云系统快速扩展新的软件或基于数据的服务/解决方案，而无需在本地安装大量硬件。

### Service Models
### 服務模式
Some cloud-based services only provide data storage and access. When storing data in the cloud, organizations must ensure that security controls are in place to prevent unauthorized access to the data. There are varying levels of responsibility for assets depending on the service model. This includes maintaining the assets, ensuring they remain functional, and keeping the systems and applications up to date with current patches. In some cases, the cloud service provider is responsible for these steps. In other cases, the consumer is responsible for these steps. 
有些云服务只提供数据存储和访问。在云中存储数据时，企业必须确保采取安全控制措施，防止未经授权访问数据。根据服务模式的不同，资产的责任程度也不同。这包括维护资产，确保其保持功能性，并使用最新补丁对系统和应用程序进行更新。在某些情况下，云服务提供商负责这些步骤。在其他情况下，消费者负责这些步骤。

Types of cloud computing service models include Software as a Service (SaaS) , Platform as a Service (PaaS) and Infrastructure as a Service (IaaS).
云计算服务模式的类型包括软件即服务（SaaS）、平台即服务（PaaS）和基础设施即服务（IaaS）。

* Services
    * Software As Service (SaaS): A cloud provides access to **software applications such as email or office productivity tools**. SaaS **is a distributed model** where software applications are hosted by a vendor or cloud service provider and made available to customers over network resources. SaaS has many benefits for organizations, which include but are not limited to: **Ease of use and limited/minimal administration**. **Automatic updates and patch management**. **The user will always be running the latest version and most up-to-date deployment of the software release, as well as any relevant security updates, with no manual patching required**. Standardization and compatibility. All users will have the same version of the software release.
* 服务
    * 软件即服务（SaaS）： 云提供对**软件应用程序（如电子邮件或办公自动化工具）**的访问。SaaS **是一种分布式模式**，软件应用程序由供应商或云服务提供商托管，并通过网络资源提供给客户。SaaS 对企业有许多好处，包括但不限于以下方面： **易于使用，管理有限/最少**。**自动更新和补丁管理**。**用户将始终运行最新版本和最新部署的软件版本，以及任何相关的安全更新，无需手动打补丁**。标准化和兼容性。所有用户都将使用同一版本的软件。

    * Platform As Service (PaaS): **A cloud provides an environment for customers to use to build and operate their own software**. PaaS is **a way for customers to rent hardware, operating systems, storage and network capacity over the internet from a cloud service provider**. The service delivery model allows customers **to rent virtualized servers and associated services for running existing applications or developing and testing new ones**. The consumer does not manage or control the underlying cloud infrastructure, including network, servers, operating systems or storage, but has control over the deployed applications and possibly application-hosting environment configurations. **A PaaS cloud provides a toolkit for conveniently developing, deploying and administering application software that is structured to support large numbers of consumers, process very large quantities of data and potentially be accessed from any point on the internet**. PaaS clouds will typically provide a set of software building blocks and a set of development tools such as programming languages and supporting run-time environments that facilitate the construction of high-quality, scalable applications. Additionally, PaaS clouds will typically provide tools that assist with the deployment of new applications. In some cases, deploying a new software application in a PaaS cloud is not much more difficult than uploading a file to a web server. PaaS clouds will also generally provide and maintain the computing resources (e.g., processing, storage and networking) that consumer applications need to operate. PaaS clouds provide many benefits for developers, including that the operating system can be changed and upgraded frequently, along with associated features and system services.
    * 平台即服务（PaaS）： **云为客户提供一个环境，用于构建和运行他们自己的软件**。PaaS 是**客户通过互联网向云服务提供商**租用硬件、操作系统、存储和网络容量的一种方式。这种服务交付模式允许客户**租用虚拟化服务器和相关服务，用于运行现有应用程序或开发和测试新的应用程序**。消费者并不管理或控制底层云基础设施，包括网络、服务器、操作系统或存储，但可以控制部署的应用程序以及可能的应用程序托管环境配置。**PaaS 云提供了一个工具包，可方便地开发、部署和管理应用软件，其结构可支持大量消费者，处理大量数据，并可从互联网上的任何地点访问**。PaaS 云通常会提供一套软件构件和一套开发工具，如编程语言和支持运行时环境，以便于构建高质量、可扩展的应用程序。此外，PaaS 云通常提供协助部署新应用程序的工具。在某些情况下，在 PaaS 云中部署新的软件应用程序并不比将文件上传到网络服务器困难多少。PaaS 云通常还会提供和维护消费者应用程序运行所需的计算资源（如处理、存储和网络）。PaaS 云为开发人员提供了许多好处，包括操作系统以及相关功能和系统服务可以经常更改和升级。

    * Infrastrucuture As Service (IaaS): A cloud provides network access **to traditional computing resources such as processing power and storage**. IaaS models **provide basic computing resources to consumers**. This includes **servers, storage, and in some cases, networking resources.** Consumers install operating systems and applications and perform all required maintenance on the operating systems and applications. Although the consumer has use of the related equipment, the cloud service provider retains ownership and is ultimately responsible for hosting, running and maintenance of the hardware. IaaS is also referred to as hardware as a service by some customers and providers. IaaS has a number of benefits for organizations, which include but are not limited to: Ability to scale up and down infrastructure services based on actual usage. This is particularly useful and beneficial where there are significant spikes and dips within the usage curve for infrastructure. Retain system control at the operating system level.
 * 基础设施即服务（IaaS）： 云提供对传统计算资源（如处理能力和存储**）的网络访问**。IaaS 模式**向消费者**提供基本计算资源。消费者安装操作系统和应用程序，并对操作系统和应用程序进行所有必要的维护。虽然消费者可以使用相关设备，但云服务提供商保留所有权，并最终负责硬件的托管、运行和维护。IaaS 也被一些客户和提供商称为硬件即服务。IaaS 对企业有许多好处，包括但不限于 能够根据实际使用情况增减基础设施服务。当基础设施的使用曲线出现明显的峰值和谷值时，这一点尤其有用和有益。在操作系统层面保留系统控制。


### Deployment Models
### 部署模型
 Clouds
    * Public: what we commonly **refer to as the cloud for the public user**. **There is no real mechanism, other than applying for and paying for the cloud service**. It is **open to the public and is**, therefore, **a shared resource that many people will be able to use as part of a resource pool**. A public cloud deployment model includes assets available for any consumers to rent or lease and is hosted by an external cloud service provider (CSP). Service level agreements can be effective at ensuring the CSP provides the cloud-based services at a level acceptable to the organization.
 云
    * 公共云：我们通常**称为面向公共用户的云**。**除了申请云服务并支付费用外，**没有真正的机制。它向公众**开放，因此是**共享资源，许多人都可以作为资源池的一部分**使用。公共云部署模式包括可供任何消费者租用或租赁的资产，并由外部云服务提供商（CSP）托管。服务级别协议可有效确保 CSP 以组织可接受的级别提供基于云的服务。

    * Private: it begins with the same technical concept as public clouds, **except that instead of being shared with the public, they are generally developed and deployed for a private organization that builds its own cloud**. Organizations can create and host private clouds using their own resources. Therefore, this deployment model includes cloud-based assets for a single organization. As such, the organization is responsible for all maintenance. However, an organization can also rent resources from a third party and split maintenance requirements based on the service model (SaaS, PaaS or IaaS). Private clouds provide organizations and their departments private access to the computing, storage, networking and software assets that are available in the private cloud.
 * 私有云：与公共云的技术概念相同，**不同的是，私有云通常不是与公众共享，而是为建立自己云**的私有组织开发和部署。组织可利用自身资源创建和托管私有云。因此，这种部署模式包括单个组织的云资产。因此，该组织负责所有维护工作。不过，组织也可以从第三方租用资源，并根据服务模式（SaaS、PaaS 或 IaaS）分担维护要求。私有云为组织及其部门提供对私有云中可用的计算、存储、网络和软件资产的私有访问。

    * Hybrid: it is created by **combining two forms of cloud computing deployment models, typically a public and private cloud**. Hybrid cloud computing **is gaining popularity with organizations by providing them with the ability to retain control of their IT environments**, conveniently allowing them to use public cloud service to fulfill non-mission-critical workloads, and taking advantage of flexibility, scalability and cost savings. Important drivers or benefits of hybrid cloud deployments include: Retaining ownership and oversight of critical tasks and processes related to technology, Reusing previous investments in technology within the organization, Control over most critical business components and systems, and Cost-effective means to fulfilling noncritical business functions (utilizing public cloud components).
* 混合：它是通过**两种形式的云计算部署模式（通常是公共云和私有云）**而成。混合云计算***受到企业的欢迎，因为它使企业能够保留对其 IT 环境***的控制，方便地使用公共云服务来完成非关键任务的工作负载，并利用灵活性、可扩展性和节约成本的优势。混合云部署的重要驱动因素或优势包括 保留与技术相关的关键任务和流程的所有权和监督权、在组织内部重复使用以前的技术投资、控制最关键的业务组件和系统，以及以具有成本效益的方式履行非关键业务功能（利用公共云组件）。

    * Community: it can be either public or private. **What makes them unique is that they are generally developed for a particular community**. An example could be a public community cloud focused primarily on organic food, or maybe a community cloud focused specifically on financial services. The idea behind the community cloud is that people of like minds or similar interests can get together, share IT capabilities and services, and use them in a way that is beneficial for the particular interests that they share.
   * 社区：可以是公共社区，也可以是私人社区。**社区云的独特之处在于，它们通常是为特定社区开发的**。例如，公共社区云主要关注有机食品，或者社区云专门关注金融服务。社区云背后的理念是，志同道合或兴趣相投的人可以聚集在一起，共享信息技术能力和服务，并以有利于他们共同的特定兴趣的方式使用它们。

### Managed Service Provider (MSP)
### 託管服務提供者 (MSP)
A managed service provider (MSP) is **a company that manages information technology assets for another company**. Small- and medium-sized businesses commonly **outsource part or all of their information technology functions to an MSP to manage day-to-day operations or to provide expertise in areas the company does not have**. Organizations may also use an MSP to provide network and security monitoring and patching services. Today, many MSPs offer cloud-based services augmenting SaaS solutions with active incident investigation and response activities. One such example is a managed detection and response (MDR) service, where a vendor monitors firewall and other security tools to provide expertise in triaging events. 
管理服务提供商（MSP）是**一家为另一家公司管理信息技术资产的公司。中小型企业通常**将其部分或全部信息技术功能外包给 MSP，以管理日常运营或提供公司所不具备的领域的专业知识**。企业还可以利用 MSP 提供网络和安全监控及补丁服务。如今，许多 MSP 提供基于云的服务，通过积极的事件调查和响应活动来增强 SaaS 解决方案。其中一个例子是托管检测和响应（MDR）服务，即由供应商监控防火墙和其他安全工具，提供事件分流方面的专业知识。

Some other common MSP implementations are: Augment in-house staff for projects; Utilize expertise for implementation of a product or service; Provide payroll services; Provide Help Desk service management; Monitor and respond to security incidents; Manage all in-house IT infrastructure.
其他一些常见的 MSP 实施包括 为项目增加内部员工；利用专业知识实施产品或服务；提供薪资服务；提供服务台服务管理；监控和应对安全事件；管理所有内部 IT 基础设施。

### Service-Level Agreement (SLA)
### 服務等級協定 (SLA)
The cloud computing **service-level agreement (cloud SLA)** is an agreement **between a cloud service provider and a cloud service customer based on a taxonomy of cloud computing–** specific terms to set the quality of the cloud services delivered. It characterizes quality of the cloud services delivered in terms of a set of measurable properties specific to cloud computing (business and technical) and a given set of cloud computing roles (cloud service customer, cloud service provider, and related sub-roles).
云计算**服务级别协议（云 SLA）**是云服务提供商和云服务客户之间基于云计算**特定术语分类的协议，用于设定所交付云服务的质量。它根据云计算（业务和技术）特有的一组可衡量属性和一组给定的云计算角色（云服务客户、云服务提供商和相关子角色）来描述所交付云服务的质量。

Think of a **rule book and legal contract—that combination is what you have in a service-level agreement (SLA)**. Let us not underestimate or downplay the importance of this document/ agreement. In it, **the minimum level of service, availability, security, controls, processes, communications, support and many other crucial business elements are stated and agreed to by both parties**.  
想想**规则书和法律合同--这就是服务级别协议（SLA）**中的组合。我们不要低估或贬低这份文件/协议的重要性。在协议中，双方**了最低服务水平、可用性、安全性、控制、流程、通信、支持和许多其他关键业务要素。 

The purpose of an **SLA is to document specific parameters, minimum service levels and remedies for any failure to meet the specified requirements**. It should also affirm data ownership and specify data return and destruction details. Other important SLA points to consider include the following: Cloud system infrastructure details and security standards; Customer right to audit legal and regulatory compliance by the CSP; Rights and costs associated with continuing and discontinuing service use; Service availability; Service performance; Data security and privacy; Disaster recovery processes; Data location; Data access; Data portability; Problem identification and resolution expectations; Change management processes; Dispute mediation processes; Exit strategy;
** 服务水平协议的目的是记录具体参数、最低服务水平以及对任何未达到规定要求**的补救措施。它还应确认数据所有权，并规定数据返还和销毁细节。需要考虑的其他重要 SLA 要点包括以下内容： 云系统基础设施详情和安全标准；客户审核 CSP 是否遵守法律法规的权利；继续使用和停止使用服务的相关权利和成本；服务可用性；服务性能；数据安全和隐私；灾难恢复流程；数据位置；数据访问；数据可移植性；问题识别和解决预期；变更管理流程；争议调解流程；退出策略；

### Network Design
### 網路設計
* **Network segmentation** involves controlling traffic **among networked devices**. Complete or physical network segmentation occurs when a network is isolated from all outside communications, so transactions can only occur between devices within the segmented network.
**网络分段**涉及控制网络设备之间的**流量。完全或物理网络分段是指网络与所有外部通信隔离，因此交易只能在分段网络内的设备之间进行。

* **A DMZ, which stands for Demilitarized Zone,**  is a network area that is designed to be **accessed by outside visitors but is still isolated from the private network of the organization**. The DMZ is often the host of public web, email, file and other resource servers.
* DMZ 是 "非军事区"（Demilitarized Zone）的缩写，**是一个网络区域，旨在**外部访问者访问，但仍与组织的专用网络**隔离。DMZ 通常是公共网络、电子邮件、文件和其他资源服务器的主机。

* **VLANs, which stands for Virtual Private Network**,  are created by **switches to logically segment a network without altering its physical topology**.
**VLAN 是虚拟专用网络**的缩写，由**交换机创建，用于在不改变物理拓扑的情况下对网络进行逻辑分割**。

* **A virtual private network (VPN)** is a **communication tunnel that provides point-to-point transmission of both authentication and data traffic over an untrusted network**.
** 虚拟专用网络（VPN）** 是一种**通信隧道，可在不受信任的网络上点对点传输验证和数据流量**。

* **Defense in depth** uses multiple **types of access controls in literal or theoretical layers** to help an organization avoid a monolithic security stance.
* 深度防御**在字面或理论层**使用多种**类型的访问控制，帮助组织避免单一的安全立场。

* **Network access control (NAC)** is a concept of controlling access to an environment through strict adherence to and implementation of security policy.
** 网络访问控制（NAC）** 是一个通过严格遵守和执行安全策略来控制环境访问的概念。

### Defense in Depth
### 縱深防禦
Defense in depth uses **a layered approach when designing the security posture of an organization**. Think about a castle that holds the crown jewels. The jewels will be placed in a vaulted chamber in a central location guarded by security guards. The castle is built around the vault with additional layers of security—soldiers, walls, a moat. The same approach is true when designing the logical security of a facility or system. Using layers of security will deter many attackers and encourage them to focus on other, easier targets. 
在设计组织的安全态势时，纵深防御采用**分层的方法。想想一座存放着皇冠上的珠宝的城堡。这些珠宝将被放置在一个中央位置的金库中，由保安人员看守。城堡围绕金库建造了多层安全设施--士兵、城墙和护城河。在设计设施或系统的逻辑安全性时，也采用了同样的方法。层层设防可以阻止许多攻击者，促使他们将注意力放在其他更容易攻击的目标上。

Defense in depth **provides more of a starting point for considering all types of controls—administrative, technological, and physical—that empower insiders and operators to work together to protect their organization and its systems**. 
纵深防御**为考虑所有类型的控制（行政、技术和物理控制）提供了更多的出发点，使内部人员和操作人员能够共同保护组织及其系统**。

Some examples that further explain the concept of defense in depth: 
一些例子进一步解释了纵深防御的概念： 

* **Data**: Controls that protect the actual data with technologies such as **encryption, data leak prevention, identity and access management and data controls**.
  ** 数据**： 利用**加密、数据防泄漏、身份和访问管理以及数据控制等技术保护实际数据的控制**。
  
* **Application**: Controls that protect the application itself with technologies such as **data leak prevention, application firewalls and database monitors**.
** 应用程序**： 利用**数据泄漏防护、应用程序防火墙和数据库监控器**等技术保护应用程序本身的控制措施。
  
* **Host**: Every control that is placed at the endpoint level, such as **antivirus, endpoint firewall, configuration and patch management**.
** 主机**： 置于端点级的所有控制，如**防病毒、端点防火墙、配置和补丁管理**。
  
* **Internal network**: Controls that are in place to protect **uncontrolled data flow and user access across the organizational network**. Relevant technologies include **intrusion detection systems, intrusion prevention systems, internal firewalls and network access controls**.
** 内部网络**： 为保护组织网络中**不受控制的数据流和用户访问**而实施的控制。相关技术包括**入侵检测系统、入侵防御系统、内部防火墙和网络访问控制**。
  
* **Perimeter**: Controls that protect against **unauthorized access to the network**. This level includes the use of technologies such as **gateway firewalls, honeypots, malware analysis and secure demilitarized zones (DMZs)**.
** 周边**： 防止**未经授权访问网络**的控制措施。这一级包括使用**网关防火墙、蜜罐、恶意软件分析和安全非军事区（DMZ）**等技术。
  
* **Physical**: Controls that provide a physical barrier, such as **locks, walls or access control**.
** 物理**： 提供物理屏障的控制，如**锁、墙或出入控制**。
  
* **Policies, procedures and awareness**: Administrative controls that reduce **insider threats (intentional and unintentional) and identify risks as soon as they appear**. 
** 政策、程序和意识**： 减少**内部威胁（有意和无意）并在风险出现时立即识别风险的行政控制**。
  
### Zero Trust
### 零信任
Zero trust networks are often **microsegmented networks, with firewalls at nearly every connecting point**. Zero trust encapsulates information assets, the services that apply to them and their security properties. **This concept recognizes that once inside a trust-but-verify environment, a user has perhaps unlimited capabilities to roam around, identify assets and systems and potentially find exploitable vulnerabilities**. Placing a greater number of firewalls or other security boundary control devices throughout the network increases the number of opportunities to detect a troublemaker before harm is done. **Many enterprise architectures are pushing this to the extreme of microsegmenting their internal networks, which enforces frequent re-authentication of a user ID**.  
零信任网络通常是**微分网络，几乎每个连接点都有防火墙**。零信任封装了信息资产、适用于这些资产的服务及其安全属性。**这一概念认为，一旦进入 "信任但验证 "环境，用户就可能拥有无限的漫游能力，可以识别资产和系统，并可能发现可利用的漏洞**。在整个网络中安装更多的防火墙或其他安全边界控制设备，可以增加在造成危害之前发现麻烦制造者的机会。**许多企业架构将这一点发挥到极致，对内部网络进行微分段，从而强制对用户 ID 进行频繁的重新认证**。 

Zero trust is an evolving design approach **which recognizes that even the most robust access control systems have their weaknesses**. It adds defenses at the user, asset and data level, rather than relying on perimeter defense. In the extreme, **it insists that every process or action a user attempts to take must be authenticated and authorized**; **the window of trust becomes vanishingly small**.  
零信任是一种不断发展的设计方法**，它认识到即使是最强大的访问控制系统也有其弱点**。它在用户、资产和数据层面增加了防御措施，而不是依赖周边防御。在极端情况下，**坚持用户尝试采取的每个流程或操作都必须经过验证和授权**；**信任窗口变得越来越小**。 

**While microsegmentation adds internal perimeters, zero trust places the focus on the assets, or data, rather than the perimeter. Zero trust builds more effective gates to protect the assets directly rather than building additional or higher walls.** 
**微分段增加了内部边界，而零信任则将重点放在资产或数据上，而不是边界上。零信任建立了更有效的大门，直接保护资产，而不是建立额外或更高的围墙。

### Network Access Control (NAC)
### 網路存取控制 (NAC)
We need to be able to see **who and what is attempting to make a network connection**. At one time, network access was limited to internal devices. Gradually, that was extended to remote connections, **although initially those were the exceptions rather than the norm**. This started to change with the concepts of bring your own device (BYOD) and Internet of Things (IoT). 
我们需要能够看到**谁和什么在尝试进行网络连接**。网络访问一度仅限于内部设备。后来，这种情况逐渐扩展到远程连接，**尽管最初这些都是例外情况，而不是常态**。随着自带设备（BYOD）和物联网（IoT）概念的出现，这种情况开始发生变化。

**Considering just IoT for a moment**, it is important to understand the range of devices that might be found within an organization. 
**如果只考虑物联网**，就必须了解组织内可能存在的设备范围。

The organization’s **access control policies and associated security policies should be enforced via the NAC device(s). Remember, of course, that an access control device only enforces a policy and doesn’t create one**.
组织的**访问控制策略和相关安全策略应通过 NAC 设备来执行。当然，请记住，访问控制设备只是执行策略，而不是创建**。

The NAC device will provide **the network visibility needed for access security and may later be used for incident response**. Aside from identifying connections, it should also be able to provide isolation for noncompliant devices within a quarantined network and provide a mechanism to “fix” the noncompliant elements, such as turning on endpoint protection. In short, the goal is to ensure that all devices wishing to join the network do so only when they comply with the requirements laid out in the organization policies. This visibility will encompass internal users as well as any temporary users such as guests or contractors, etc., and any devices they may bring with them into the organization.
NAC 设备将提供**访问安全所需的网络可见性，并可能在以后用于事件响应**。除了识别连接外，它还应能够隔离隔离网络中不合规的设备，并提供 "修复 "不合规元素的机制，例如打开端点保护。简而言之，目标是确保所有希望加入网络的设备只有在符合组织政策规定的要求时才能加入。这种可视性将包括内部用户和任何临时用户，如访客或承包商等，以及他们可能带入组织的任何设备。

Let’s consider some possible use cases for NAC deployment: Medical devices; IoT devices; BYOD/mobile devices (laptops, tablets, smartphones); Guest users and contractors; 
让我们考虑一下 NAC 部署的一些可能用例： 医疗设备、物联网设备、BYOD/移动设备（笔记本电脑、平板电脑、智能手机）、访客用户和承包商； 

It is critically important that all mobile devices, regardless of their owner, go through an onboarding process, ideally each time a network connection is made, and that the device is identified and interrogated to ensure the organization’s policies are being met. 
至关重要的是，所有移动设备，无论其所有者是谁，都必须经过入职流程，最好是在每次进行网络连接时，对设备进行识别和检查，以确保符合组织的政策。

### Network Segmentation (Demilitarized Zone (DMZ))
### 網路分段（非軍事區 (DMZ)）
**Network segmentation** is also **an effective way to achieve defense in depth for distributed or multi-tiered applications**. The use of a demilitarized zone (DMZ), for example, is a common practice in security architecture. **With a DMZ**, host systems that are accessible through the firewall **are physically separated from the internal network** by means of secured switches or by using an additional firewall to control traffic between the web server and the internal network. Application DMZs (or semi-trusted networks) are frequently used today to limit access to application servers to those networks or systems that have a legitimate need to connect.
**网络分段**也是分布式或多层应用**实现纵深防御的有效方法。例如，使用非军事区（DMZ）是安全架构中的一种常见做法。**使用 DMZ**，可通过防火墙访问的主机系统**通过安全交换机或使用额外的防火墙控制网络服务器与内部网络之间的流量，与内部网络**物理隔离。如今，应用 DMZ（或半信任网络）经常被用来限制对应用服务器的访问，仅限于那些有合法连接需求的网络或系统。

### Segmentation for Embedded Systems and IoT
### 嵌入式系統與物聯網細分
**Network-enabled devices are any type of portable or nonportable device that has native network capabilities**. This generally assumes the **network in question is a wireless type of network**, typically provided by a mobile telecommunications company. Network-enabled devices include **smartphones, mobile phones, tablets, smart TVs or streaming media players**, network-attached printers, game systems, and much more. 
**支持网络的设备是指具有本地网络功能的任何类型的便携式或非便携式设备**。这通常假定**网络是一种无线网络**，通常由移动电信公司提供。支持网络的设备包括**智能手机、移动电话、平板电脑、智能电视或流媒体播放器**、网络附加打印机、游戏系统等。

The Internet of Things (IoT) **is the collection of devices that can communicate over the internet with one another or with a control console in order to affect and monitor the real world.** IoT devices might be labeled as smart devices or smart-home equipment. Many of the ideas of industrial environmental control found in office buildings are finding their way into more consumer-available solutions for small offices or personal homes.  
物联网（IoT）**是指可以通过互联网相互通信或与控制台通信，从而影响和监控现实世界的设备集合。办公大楼中的许多工业环境控制理念正在被更多的消费者引入小型办公室或个人家庭的解决方案中。 

Embedded systems and network-enabled devices that communicate with the internet are considered IoT devices and need special attention to ensure that communication is not used in a malicious manner. Because an embedded system is often in control of a mechanism in the physical world, a security breach could cause harm to people and property. Since many of these devices have multiple access routes, such as ethernet, wireless, Bluetooth, etc., special care should be taken to isolate them from other devices on the network. You can impose logical network segmentation with switches using VLANs, or through other traffic-control means, including MAC addresses, IP addresses, physical ports, protocols, or application filtering, routing, and access control management. Network segmentation can be used to isolate IoT environments. 
与互联网通信的嵌入式系统和网络设备被视为物联网设备，需要特别关注，以确保通信不会被恶意使用。由于嵌入式系统通常控制着物理世界中的某个机制，因此安全漏洞可能会对人员和财产造成伤害。由于许多这类设备都有多种接入路径，如以太网、无线、蓝牙等，因此应特别注意将它们与网络上的其他设备隔离。您可以使用 VLAN 或其他流量控制手段（包括 MAC 地址、IP 地址、物理端口、协议或应用程序过滤、路由选择和访问控制管理），通过交换机实施逻辑网络分段。网络分段可用于隔离物联网环境。

### Microsegmentation
### 微分段
The toolsets of current adversaries are polymorphic in nature and allow threats to bypass static security controls. **Modern cyberattacks take advantage of traditional security models to move easily between systems within a data center**. Microsegmentation aids in protecting against these threats. A fundamental design requirement of **microsegmentation is to understand the protection requirements for traffic within a data center and traffic to and from the internet traffic flows**. 
当前对手的工具集具有多态性，可让威胁绕过静态安全控制。**现代网络攻击利用传统的安全模式，在数据中心内的系统间轻松移动**。微分区有助于防范这些威胁。微分段的一个基本设计要求是了解数据中心内的流量以及进出互联网流量的保护要求**。

When organizations avoid infrastructure-centric design paradigms, they are more likely to become more efficient at service delivery in the data center and become apt at detecting and preventing advanced persistent threats. 
如果企业避免以基础设施为中心的设计模式，就更有可能提高数据中心服务交付的效率，并善于检测和预防高级持续性威胁。

### Virtual Local Area Network (VLAN)
### 虛擬區域網路 (VLAN)
Virtual local area networks (VLANs) allow network administrators **to use switches to create software-based LAN segments**, which can **segregate or consolidate traffic across multiple switch ports**. **Devices that share a VLAN communicate through switches as if they were on the same Layer 2 network**. Since VLANs act as discrete networks, communications between VLANs must be enabled. Broadcast traffic is limited to the VLAN, reducing congestion and reducing the effectiveness of some attacks. Administration of the environment is simplified, as the VLANs can be reconfigured when individuals change their physical location or need access to different services. VLANs can be configured based on switch port, IP subnet, MAC address and protocols. VLANs do not guarantee a network’s security. At first glance, it may seem that traffic cannot be intercepted because communication within a VLAN is restricted to member devices. However, there are attacks that allow a malicious user to see traffic from other VLANs (so-called VLAN hopping). The VLAN technology is only one tool that can improve the overall security of the network environment.
虚拟局域网（VLAN）允许网络管理员**使用交换机创建基于软件的局域网段**，这样可以**隔离或合并多个交换机端口上的流量**。**共享 VLAN 的设备通过交换机进行通信，就像它们在同一个二层网络上**一样。由于 VLAN 是独立的网络，因此必须启用 VLAN 之间的通信。广播流量仅限于 VLAN，从而减少了拥塞并降低了某些攻击的有效性。当个人改变物理位置或需要访问不同服务时，可以重新配置 VLAN，从而简化了环境管理。VLAN 可根据交换机端口、IP 子网、MAC 地址和协议进行配置。VLAN 不能保证网络的安全性。乍一看，流量似乎不会被拦截，因为 VLAN 内的通信仅限于成员设备。然而，有些攻击可以让恶意用户看到来自其他 VLAN 的流量（即所谓的 VLAN 跳转）。VLAN 技术只是提高网络环境整体安全性的一种工具。

### Virtual Private Network (VPN)
### 虛擬私人網路 (VPN)
A virtual private network (VPN) **is not necessarily an encrypted tunnel**. It is simply **a point-to-point connection between two hosts that allows them to communicate**. Secure communications can, of course, be provided by the VPN, but only if the security protocols have been selected and correctly configured to provide a trusted path over an untrusted network, such as the internet. Remote users employ VPNs to access their organization’s network, and depending on the VPN’s implementation, they may have most of the same resources available to them as if they were physically at the office. As an alternative to expensive dedicated point-to-point connections, organizations use gateway-to-gateway VPNs to securely transmit information over the internet between sites or even with business partners. 
虚拟专用网络（VPN）**不一定是加密隧道**。它只是两个主机之间**的点对点连接，允许它们进行通信**。VPN 当然可以提供安全通信，但前提是必须选择安全协议并正确配置，以便在互联网等不可信网络上提供可信路径。远程用户使用 VPN 访问其组织的网络，根据 VPN 的实施情况，他们可以获得与在办公室时相同的大部分资源。作为昂贵的专用点对点连接的替代方案，组织使用网关对网关 VPN 在站点之间甚至与业务伙伴之间通过互联网安全地传输信息。
