# Cisco_Tracker_Troubleshooting

## 📌 Project Overview

This project demonstrates how to create and troubleshoot a basic network using **Cisco Packet Tracer**.

The network contains **2 PCs connected to 1 switch**. No router is used because both PCs belong to the same network.

## 🖥️ Network Topology

```text
PC0 ───────── Switch0 ───────── PC1
```

### Devices Used

* 2 PCs
* 1 Switch
* 2 Copper Straight-Through Cables
* No Router

## 🌐 IP Configuration

### PC0

```text
IP Address:   192.168.10.25
Subnet Mask:  255.255.255.0
Default Gateway: Not Required
```

### PC1

```text
IP Address:   192.168.10.26
Subnet Mask:  255.255.255.0
Default Gateway: Not Required
```

Both PCs are in the same network:

```text
192.168.10.0/24
```

## 🔧 Configuration Steps

### Step 1: Create the Network

1. Open Cisco Packet Tracer.
2. Add two PCs.
3. Add one switch.
4. Connect PC0 to Switch0.
5. Connect PC1 to Switch0.
6. Use Copper Straight-Through cables.

### Step 2: Configure PC0

Go to:

**PC0 → Desktop → IP Configuration**

Enter:

```text
IP Address: 192.168.10.25
Subnet Mask: 255.255.255.0
```

### Step 3: Configure PC1

Go to:

**PC1 → Desktop → IP Configuration**

Enter:

```text
IP Address: 192.168.10.26
Subnet Mask: 255.255.255.0
```

Leave the Default Gateway empty.

## 🧪 Testing the Connection

Open:

**PC0 → Desktop → Command Prompt**

Run:

```text
ping 192.168.10.26
```

If the configuration is correct, the result will be similar to:

```text
Reply from 192.168.10.26
Reply from 192.168.10.26
Reply from 192.168.10.26
Reply from 192.168.10.26
```

This confirms that PC0 and PC1 can communicate successfully.

## 🔍 Troubleshooting

If the ping fails, check the following:

1. Check whether the cables are connected correctly.
2. Make sure the switch ports are green.
3. Check the IP address of both PCs.
4. Check the subnet mask.
5. Make sure both PCs are in the same network.
6. Make sure there are no duplicate IP addresses.
7. Use the following command to check the configuration:

```text
ipconfig
```

To check the ARP table:

```text
arp -a
```

## 📚 Commands Used

```text
ipconfig
ping <IP-address>
arp -a
```

## 🎯 Objective

The main objective of this project is to understand:

* Basic LAN configuration
* IP addressing
* Subnet masks
* Switch connectivity
* ICMP ping testing
* Basic network troubleshooting
* ARP operation

## ✅ Result

The two PCs were successfully connected through the switch and communication was verified using the **ping** command.

## 🛠️ Software Used

**Cisco Packet Tracer**

## 👨‍💻 Author

**Guruprakash K**

B.Tech – Computer Science and Business Systems
