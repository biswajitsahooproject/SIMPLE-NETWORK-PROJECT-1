# SIMPLE-NETWORK-PROJECT-1
Network Design Description for ACCOUNTS and DELIVERY Departments
# ACCOUNTS and DELIVERY Department Network Design

This repository contains the network design project for connecting the **ACCOUNTS** and **DELIVERY** departments of a company using **Cisco Packet Tracer**. The project includes the configuration of switches, routers, and PCs, as well as the use of the provided network address `192.168.40.0` to configure IP addresses, subnet masks, and gateways.

## 🏢 **Network Overview**

The design connects two departments:
- **ACCOUNTS Department**: Contains 2 PCs.
- **DELIVERY Department**: Contains 2 PCs.

### **Key Design Elements**:
1. **Switches**: Each department has its own switch to manage the local network.
2. **Router**: A router interconnects both departments, allowing communication between the two.
3. **IP Addressing**: The network is divided into two subnets using the `192.168.40.0` address block:
   - **ACCOUNTS Subnet**: `192.168.40.0/25`
   - **DELIVERY Subnet**: `192.168.40.128/25`
4. **Subnet Masks**: Both subnets use the subnet mask `255.255.255.128`.
5. **Gateways**:
   - **ACCOUNTS Gateway**: `192.168.40.1`
   - **DELIVERY Gateway**: `192.168.40.129`

### **Devices and Connections**:
- 2 PCs in the **ACCOUNTS** department.
- 2 PCs in the **DELIVERY** department.
- 2 switches to connect each department's PCs.
- A router that connects the two subnets.

---

## 🌐 **Network Configuration**

### **IP Address Configuration**:
- **ACCOUNTS Department**: 
  - IP Range: `192.168.40.1` to `192.168.40.126`
  - Subnet Mask: `255.255.255.128`
  - Default Gateway: `192.168.40.1`
  
- **DELIVERY Department**:
  - IP Range: `192.168.40.129` to `192.168.40.254`
  - Subnet Mask: `255.255.255.128`
  - Default Gateway: `192.168.40.129`

### **Cabling**:
- **PC to Switch**: Use **copper straight-through cables** to connect PCs to their respective switches.
- **Switch to Router**: Use a **copper cross-over cable** to connect each switch to the router’s interfaces.
- **Router Interfaces**: The router has two interfaces:
  - One connected to the ACCOUNTS department (IP `192.168.40.1`).
  - One connected to the DELIVERY department (IP `192.168.40.129`).

### **Router Configuration**:
- Assign the IP address `192.168.40.1` to the router interface connected to the ACCOUNTS department.
- Assign the IP address `192.168.40.129` to the router interface connected to the DELIVERY department.
- Enable routing between the two subnets using **static routing** or **dynamic routing protocols** like **RIP**.

---

## 🖥️ **Testing Connectivity**

Once the devices are configured and connected:
1. From any PC in the **DELIVERY** department, open the Command Prompt or Terminal.
2. Use the `ping` command to test connectivity between the **DELIVERY** and **ACCOUNTS** departments.

   Example:  
   `ping 192.168.40.2` (from DELIVERY to ACCOUNTS)

3. If the ping is successful, it confirms that the departments are correctly connected and can communicate with each other.

---

## 🔧 **Technologies Used**

- **Cisco Packet Tracer**: For creating and simulating the network design.
- **Routing Protocols**: Static routing or RIP to ensure communication between departments.
- **IP Addressing**: Used `192.168.40.0/25` for subnetting.

---

## 📂 **Project Files**

- **Network Design File**: `Accounts_Delivery_Network.pkt` – Cisco Packet Tracer file containing the network topology and configurations.

---

## 👨‍💻 **Author Information**

- **Name**: Biswajit Sahoo
- **LinkedIn**: [Biswajit Sahoo LinkedIn](https://linkedin.com/in/biswajit-sahoo-b06a53220)
- **Email**: [biswajitsahoo152001@gmail.com](mailto:biswajitsahoo152001@gmail.com)

---

