
# 📡 Network Security Project

## 📖 Overview
This project demonstrates the design and implementation of a secure enterprise network.  
The network was built using **subnetting, OSPF with authentication, ACLs, SSH, VPN, AAA, and Zone-Based Firewall (ZBF)** to achieve connectivity, scalability, and strong security measures.  

---

## 🎯 Objectives
- Implement an efficient **IP subnetting scheme**.  
- Configure **OSPF routing** with authentication for secure routing updates.  
- Enable **SSH** for secure device management.  
- Establish a **site-to-site VPN** for encrypted communication.  
- Apply **Zone-Based Firewall (ZBF)** policies for traffic control.  
- Secure access using **ACLs**.  
- Implement **AAA (local and server-based)** for authentication, authorization, and accounting.  

---

## 🖼️ Network Design
- Logical and physical topology diagrams (see `/diagrams`).  
- Subnetting plan with IP addressing scheme.  
- OSPF area design (single Area 0).  

---

## ⚙️ Implementation
1. **Subnetting** – Divided the IP block into LAN, WAN, and DMZ subnets.  
2. **OSPF** – Configured dynamic routing with MD5 authentication.  
3. **SSH** – Enabled secure remote access with RSA key pairs.  
4. **VPN** – Configured site-to-site IPsec VPN between HQ and Branch.  
5. **ZBF** – Applied firewall rules between INSIDE, OUTSIDE, and DMZ zones.  
6. **ACLs** – Used standard and extended ACLs to filter traffic.  
7. **AAA** – Implemented local AAA and simulated server-based RADIUS authentication.  

---

## 🔍 Testing & Verification
- **Connectivity** verified with `ping` and `traceroute`.  
- **OSPF neighbors** confirmed with `show ip ospf neighbor`.  
- **ACLs** tested with allowed/denied traffic.  
- **VPN** verified with `show crypto session`.  
- **SSH** tested with login to router from LAN host.  
- **AAA** verified using local and RADIUS authentication.  
- **ZBF** tested with permitted and blocked traffic flows.  

---

## 🚧 Challenges & Solutions
- **OSPF neighbors not forming** → Fixed by matching area IDs and enabling authentication on both sides.  
- **ACL blocking legitimate traffic** → Refined ACL rules and used sequence numbers.  
- **VPN tunnel not coming up** → Corrected access-list for interesting traffic.  
- **SSH login failures** → Fixed by setting local user credentials and domain name.  

---

## ✅ Conclusion
- Designed and implemented a secure and scalable network.  
- Verified connectivity, routing, and security policies.  
- Met all project objectives successfully.  

**Future Improvements:**  
- Add redundancy (HSRP/VRRP).  
- Integrate IPS/IDS for advanced threat detection.  
- Extend VPN to support remote access users.  


---

## 📂 Repository Structure
