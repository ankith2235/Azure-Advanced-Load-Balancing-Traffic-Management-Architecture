# Azure Advanced Load Balancing & Traffic Management Architecture

## 📌 Project Overview

This project demonstrates the implementation of **advanced Azure networking, load balancing, and traffic management concepts**. It covers local and global load balancing, path-based routing, DNS configuration, and secure access to virtual machines using Azure-native services.

The goal of this project is to design a **highly available, scalable, and secure Azure infrastructure** following real-world cloud architecture best practices.

---

## 🛠️ Technologies & Services Used

* Azure Virtual Machines (Ubuntu)
* Apache2 Web Server
* Azure Load Balancer (Layer 4)
* Azure Application Gateway (Layer 7)
* Azure DNS
* Azure Traffic Manager
* Azure Bastion
* Azure Virtual Network (VNet)

---

## 📂 Tasks Performed

### 🔹 Task 1: Deploy Virtual Machines & Azure Load Balancer

* Deployed **2 Ubuntu Virtual Machines**
* Installed **Apache2** web server on both VMs
* Modified `index.html`:

  * VM1 displays: `This is VM1`
  * VM2 displays: `This is VM2`
* Configured **Azure Load Balancer** to distribute traffic evenly between VM1 and VM2

✅ Result: Traffic is balanced across both VMs

---

### 🔹 Task 2: Application Gateway with Path-Based Routing

* Created an **Azure Application Gateway**
* Configured **path-based routing**:

  * `/vm1` → VM1
  * `/vm2` → VM2

✅ Result: Requests are routed based on URL paths

---

### 🔹 Task 3: DNS Configuration for Virtual Machines

* Assigned **public IP addresses** to both VMs
* Created **DNS records** for each VM
* Verified access using DNS names instead of IP addresses

✅ Result: VMs are accessible using DNS names

---

### 🔹 Task 4: Multi-Region Load Balancing using Traffic Manager

* Deployed **2 VMs in different Azure regions**
* Configured **Azure Traffic Manager**
* Enabled **geographic load balancing**

✅ Result: Users are routed to the nearest regional VM

---

### 🔹 Task 5: Secure VM Access using Bastion Host

* Deployed a **VM without a public IP address**
* Configured **Azure Bastion** in the VNet
* Accessed the private VM securely via Azure Portal

✅ Result: Secure VM access without exposing public IPs

---

## 🧠 Key Learnings

* Difference between **Layer 4 and Layer 7 load balancing**
* Path-based routing using Application Gateway
* Global traffic management with Azure Traffic Manager
* DNS configuration and name resolution
* Secure access to private resources using Bastion

---

## 🎯 Use Case

This project is suitable for:

* Junior DevOps / Cloud Engineer roles
* Azure networking hands-on labs
* Resume and GitHub portfolio showcase

---

## 👤 Author

**Ankith Ajith Kumar**
MCA Graduate | DevOps & Cloud Enthusiast

---

## 📎 Future Enhancements

* Enable HTTPS with SSL certificates
* Add monitoring using Azure Monitor
* Automate deployment using Terraform or ARM templates
