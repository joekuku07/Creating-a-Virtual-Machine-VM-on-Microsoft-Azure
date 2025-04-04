# Creating-a-Virtual-Machine-VM-on-Microsoft-Azure

### **Prerequisites for Creating an Azure VM**  

1. **Azure Account** – Active subscription (Free-tier or Pay-As-You-Go).  
2. **Resource Group** – Organize resources efficiently.  
3. **VM Configuration** – Choose OS (Windows/Linux), VM size, and authentication (SSH key/password).  
4. **Networking** – Setup Virtual Network, Public IP, and necessary ports (SSH 22, RDP 3389).  
5. **Storage** – Select OS disk type (Standard SSD/Premium SSD) and add data disks if needed.  
6. **Access Tools** – Use **RDP (Windows)** or **SSH (Linux)** for remote access.  
7. **Budget & Monitoring** – Track costs and enable Azure Monitor.  
8. **Backup & Security** – Use Azure Backup and configure security settings.  

Creating a Virtual Machine (VM) on **Microsoft Azure** for your **GitHub project** involves several steps. Here’s a **step-by-step guide** to get you started:

---

### **Step 1: Log in to Azure Portal**
1. Go to [Azure Portal](https://portal.azure.com/).
2. Sign in with your **Microsoft account**.
   
![Screenshot 2025-04-02 at 10 29 49 am](https://github.com/user-attachments/assets/31743760-9715-49c9-9ce6-77c07463608a)

---

### **Step 2: Create a New Virtual Machine**
In the **Azure Portal**, click on **"Virtual Machines"** from the left menu.
1. Click **"Create"** →
2. **"Azure Virtual Machine"**.
   
![Screenshot 2025-04-02 at 11 23 40 am](https://github.com/user-attachments/assets/4933de61-9204-4f1d-933e-6d45ee446957)

---

### **Step 3: Configure Basic Settings**
1. **Subscription**: Select your **Azure subscription**.
2. **Resource Group**: Click **"Create new"** (if you don’t have one) and name it (e.g., `GitHubProjectRG`).
3. **Virtual Machine Name**: Enter a name (e.g., `GitHubVM`).
4. **Region**: Select the **nearest data center** for best performance.
5. **Availability Options**: Choose **"No infrastructure redundancy required"** (unless needed).
![Screenshot 2025-04-02 at 12 59 48 pm](https://github.com/user-attachments/assets/dc74c5c5-1c90-4754-b65f-88a0fd36e7ab)

6. **Image**: Select an **OS**:
   - **Windows** (e.g., Windows Server 2022)
   - **Linux** (e.g., Ubuntu 22.04 LTS)
7. **Size**: Choose an appropriate **VM size** (e.g., `Standard_B2s` for small workloads).
8. **Authentication**:
   - **SSH Public Key (for Linux)**
   - **Password (for Windows)**
![Screenshot 2025-04-02 at 11 33 19 am](https://github.com/user-attachments/assets/f7b2c27f-3417-4a59-886c-e4807bf78427)

---

### **Step 4: Configure Networking**
1. Under the **"Networking"** tab:
   - **Virtual Network**: Select default or create a new one.
   - **Subnet**: Choose the default subnet.
   - **Public IP**: Select "Enabled" or "Create" to access via the internet.
   - **Inbound Port Rules**: Allow necessary ports:
     - **Linux**: Allow **SSH (port 22)**
     - **Windows**: Allow **RDP (port 3389)**
     - **Web Server**: Allow **HTTP (port 80), HTTPS (port 443)** if needed.
![Screenshot 2025-04-02 at 1 01 01 pm](https://github.com/user-attachments/assets/c2c3f6cc-c433-4e91-83ae-08c817e2200e)
![Screenshot 2025-04-02 at 1 28 37 pm](https://github.com/user-attachments/assets/393fd849-75ae-4877-8638-11404e4ca18a)

---

### **Step 5: Configure Storage and Disks**
1. **OS Disk Type**: Choose **Standard SSD** or **Premium SSD**.
2. **Additional Disks**: Add extra storage if required.
![Screenshot 2025-04-02 at 11 34 42 am](https://github.com/user-attachments/assets/bcbae5ed-d7bc-4da5-a12f-1c36fa7f654e)

---

### **Step 6: Review and Create**
1. Click **"Review + Create"**.
2. Review your configurations.
3. Click **"Create"** to deploy the VM.
 ![Screenshot 2025-04-02 at 1 31 13 pm](https://github.com/user-attachments/assets/08f7cad6-bb52-4fc7-a1bc-412fa9c5d6c3)
![Screenshot 2025-04-02 at 1 17 03 pm](https://github.com/user-attachments/assets/8b7373b0-82c2-41e4-aae7-d8cde6409312)

---
