# funktionog-homelab
Homelab Documentation
**Home Network Lab Overview**

### **Network Infrastructure**
Your home network lab leverages Ubiquiti equipment for advanced management and scalability. Key components include:

- **Flex Mini Switch**: A compact switch with PoE input support for efficient connectivity.
- **UniFi Express Router**: Core router with a robust firewall and tailored rules for network security.
- **Ubiquiti UniFi Access Points (APs)**: Deployed for high-speed Wi-Fi coverage, each assigned to specific VLANs for segmentation.

The network is segmented into three primary VLANs to isolate traffic and enhance security. Devices on different VLANs communicate only when explicitly allowed, reducing potential risks.

---

### **VLAN Configuration**
The VLANs and their purposes are as follows:

1. **VLAN 10: Home Network**
   - Devices: Personal laptops, smartphones, and tablets.
2. **VLAN 20: Kids’ Network**
   - Devices: Children's devices with strict access controls and content filtering.
3. **VLAN 30: Lab Network**
   - Devices: Virtual machines, servers, and vulnerable ISOs for cybersecurity training.

Traffic between VLANs is controlled via tailored firewall rules on the UniFi Express Router. For instance, the kids’ network is locked down to ensure safety and prevent unauthorized access.

---

### **Virtual Machines and Training Setup**
The lab network hosts several virtual machines (VMs) managed using VirtualBox:

- **Operating Systems**:
  - **Parrot OS**: A security-focused Linux distribution for ethical hacking.
  - **Vulnerable ISOs**: Used for exploitation and penetration testing exercises.
- **Gaming VM**: A dedicated VM for running Steam games, hosted on a NAS accessible from multiple devices (desktop PCs, MacBook Airs, etc.).

This setup provides an environment for hands-on learning in networking and cybersecurity while supporting entertainment needs.

---

### **Wi-Fi and Access Points**
The UniFi access points are configured with:

- **SSID Segmentation**: Each VLAN has a dedicated SSID (e.g., HomeWiFi, KidsNet, LabNet) for streamlined access.
- **Optimized Traffic Management**: Quality of Service (QoS) ensures gaming and streaming traffic receive priority.
- **Multiple Access Points**: Each VLAN is assigned specific APs to maintain network isolation and enhance performance.

---

### **Network Monitoring and Security**
- **Monitoring Tools**: The UniFi Controller provides comprehensive visibility into network performance and anomalies.
- **Firewall Rules**: Implemented to enforce secure communication while blocking unnecessary traffic.
- **Intrusion Detection/Prevention**: Configured using tools like Suricata to identify and mitigate threats proactively.

---

### **Gaming Setup**
Your gaming setup is optimized for performance:
- Steam is configured to run from a NAS, making it accessible across various devices within the home.
- The network ensures low latency and high bandwidth for seamless gaming experiences.

---

### **Future Expansion**
Considerations for future upgrades include:
- Adding VLANs for specific projects or environments, such as development or IoT experimentation.
- Deploying honeypots to analyze and learn from malicious traffic.
- Setting up a secure VPN for remote access to the lab.

This comprehensive home network lab provides a robust platform for experimenting with networking concepts, enhancing gaming experiences, and conducting hands-on cybersecurity training.

