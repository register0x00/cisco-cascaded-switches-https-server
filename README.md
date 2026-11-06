# Cisco Cascaded Switch Topology with HTTPS Web Server

A Local Area Network (LAN) simulation engineered and tested in **Cisco Packet Tracer**. This project focuses on Layer 2 data propagation across a linear cascade of switches to access a secure centralized Web Server over HTTPS.

## 🌐 Network Topology
<img width="1920" height="1015" alt="2026-11-06_18-07-20" src="https://github.com/user-attachments/assets/a6736732-3633-4efb-9321-09c929d765d2" />

### ⚙️ Technical Layout & Behavior:
* **Cascaded Switch Backbone:** Integrated 4 **2960-24TT Switches** connected in a linear chain topology to simulate a multi-segment corporate floor environment.
* **Secure Web Server:** Configured a central **Server-PT** node hosted on `Switch2` running `HTTP/HTTPS` services listening on standard secure ports (TCP 443).
* **Flat Layer 2 Infrastructure:** All endpoints (`PC0` through `PC3`) and the server reside within a single Local Area Network sub-segment, allowing direct MAC-based delivery.
* **End-to-End Verification:** Verified network connectivity and encryption simulation by successfully requesting the server's webpage using the Cisco Web Browser utility on end-user workstations.

## 🛠️ Tools Used
* **Cisco Packet Tracer** (Simulation environment)
* **File format:** `.pkt`

## 🚀 How to Test
1. Download the `.pkt` file and open it in **Cisco Packet Tracer**.
2. Select any endpoint PC (e.g., `PC0` or `PC3`).
3. Navigate to **Desktop -> Web Browser**.
4. Enter the secure server address using its IP (e.g., `https://[Server_IP]`) to verify end-to-end data delivery across the switch cascade.

## ⌨️ Configuration Note
This layout does not require any manual CLI configuration since it operates strictly at Layer 2 using unconfigured plug-and-play switches. All communication between the endpoints and the HTTPS server works automatically out of the box.

