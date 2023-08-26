# Lab 1

## Q1)

command: `ipconfig`
ip: 192.168.100.248

## Q2)

command: `ipconfig /all`

```jsx

Physical Address. . . . . . . . . : 14-5A-FC-44-AA-77
DHCP Enabled. . . . . . . . . . . : Yes
IPv4 Address. . . . . . . . . . . : 192.168.100.248(Preferred)
Default Gateway . . . . . . . . . : 192.168.100.1
```

## Q3)

```jsx
C:\Users\monoc>hostname
Hadron
```

## Q4)

I pinged my pc to check the connectivity between the laptop and the pc:

```jsx
C:\Users\monoc>ping 192.168.100.61

Pinging 192.168.100.61 with 32 bytes of data:
Reply from 192.168.100.61: bytes=32 time=23ms TTL=128
Reply from 192.168.100.61: bytes=32 time=3ms TTL=128
Reply from 192.168.100.61: bytes=32 time=2ms TTL=128
```

If there are connectivity problems between 2 hosts the ping command will output that the host is unreachable

## Q5)

```jsx
C:\Users\monoc>netstat
Active Connections

Proto  Local Address          Foreign Address        State
TCP    127.0.0.1:8597         Hadron:52935           ESTABLISHED
TCP    127.0.0.1:8597         Hadron:53198           ESTABLISHED
TCP    127.0.0.1:8597         Hadron:53199           ESTABLISHED
TCP    127.0.0.1:8597         Hadron:53200           ESTABLISHED
TCP    127.0.0.1:52866        Hadron:52867           ESTABLISHED
TCP    127.0.0.1:52867        Hadron:52866           ESTABLISHED
TCP    127.0.0.1:52868        Hadron:52869           ESTABLISHED
TCP    127.0.0.1:52869        Hadron:52868           ESTABLISHED
TCP    127.0.0.1:52935        Hadron:8597            ESTABLISHED
TCP    127.0.0.1:53198        Hadron:8597            ESTABLISHED
TCP    127.0.0.1:53199        Hadron:8597            ESTABLISHED
TCP    127.0.0.1:53200        Hadron:8597            ESTABLISHED
TCP    192.168.100.248:51423  162.159.134.234:https  ESTABLISHED
```

## Q6)

```jsx
C:\Users\monoc>tracert [google.com](http://google.com/)
Tracing route to [google.com](http://google.com/) [216.58.209.142]
over a maximum of 30 hops:

1     1 ms     1 ms    84 ms  192.168.100.1
2     9 ms    10 ms     3 ms  38.7.190.1
3   135 ms     3 ms     4 ms  202.141.224.69
4     9 ms     4 ms     5 ms  119.159.244.86
5    10 ms    14 ms     7 ms  10.253.4.70
6   601 ms   110 ms   110 ms  10.253.4.26
7   241 ms   415 ms   108 ms  74.125.118.170
8  1024 ms    26 ms   163 ms  172.253.51.205
9   176 ms   511 ms   508 ms  108.170.247.18
10   199 ms   412 ms   172 ms  142.251.77.153
11    29 ms    22 ms   617 ms  108.170.246.113
12    79 ms   921 ms   207 ms  108.170.227.189
13    22 ms   159 ms    22 ms  [arn09s05-in-f142.1e100.net](http://arn09s05-in-f142.1e100.net/) [216.58.209.142]

Trace complete.
```

google is 13 hops away.

## Q7)

That's because we need to provide the ping command with an Ip address or a domain name. "blue machine" is not a valid domain name or an ip address that is why ping didn't work.

## Q8)

normally, we use straight cables to connect our pcs to the routers in our home.

## Q9)

We cannot connect a switch to a switch using a straight cable because both of them are the same type of network devices. To connect a switch to a switch, we would need to use a cross cable. On the other hand if we were to connect a pc to a router, then we can use a straight cable because both of them are different devices.

## Q10)

# Network Report

---

## Introduction

This report provides an overview of the network setup in a home environment which consists of 2 computers. One of the computers is a desktop and the other one is a laptop. The desktop is Labelled as `DESKTOP-GAOP9H8` and the Laptop is labelled as `Hadron`

## Network Topology

Topology: Star Topology

`DESKTOP-GAOP9H8` is connected to the only router in the network (`192.168.100.1`) a straight cable and the laptop is connected wirelessly to the router using its “Wireless LAN Adapter Wi-Fi” Network interface.

## Hardware and Software

- `DESKTOP-GAOP9H8`
    - Description: This Desktop computer is the primary computer used in the household for all tasks including gaming, productivity and work-related tasks.
    - Hardware:
        - Intel Core i7 6700 processor
        - 16 GB Ram
        - 128 GB SSD + 1 TB HDD
        - NVIDIA Geforce GTX 1060 6GB Graphics card
    - Network Interface: Ethernet Adapter
    - Operation System: Windows 10 Pro 64-bit
- `Hadron`
    - Description: Laptop used for studying and productivity because of its good performance and portable nature.
    - Hardware:
        - AMD Ryzen 5 5500U processor
        - 16 GB Ram
        - 256 GB Nvme SSD + 1 TB Nvme SSD
        - Radeon Graphics
    - Network Interface: Wireless LAN Adapter Wi-Fi
    - Operating System: Windows 11 Pro 64-bit

## **Network Configuration**

- **IP Addresses:** `DESKTOP-GAOP9H8` has a dynamically assigned IP address of `192.168.100.61` from the router's DHCP. `Hadron` also uses DHCP and has the IP address `192.168.100.248`.

## **Security**

- **Firewall:** Windows Defender Firewall is enabled on `DESKTOP-GAOP9H8` and `Hadron`
- **Antivirus/Antimalware:**  `DESKTOP-GAOP9H8` and `Hadron` both use windows defender antivirus and firewall.
- **Password Protection:** Both computers have user accounts with strong passwords.

## **Internet Connection**

- **ISP:** Optix
- **Connection Type:** Cable broadband.
- **Router/Modem:** Huawei HG8546M