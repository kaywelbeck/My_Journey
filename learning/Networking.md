<div style="text-align: center;">
    <h1><u>NETWORKING</u></h1>
</div>

<h4><u>WHAT IS A NETWORK</u></h4>

---

<h4><u>OSI MODEL</u></h4>
The Open Systems Interconnections (OSI) model defines the standard for how computers share information over a network.

<div style="text-align: center;">
    <img src="https://www.imperva.com/learn/wp-content/uploads/sites/13/2020/02/OSI-7-layers.jpg.webp" alt="OSI 7 Layers" style="border: 2px solid black; padding: 5px;">
</div>


<h2 style="text-align: center;"><u>OSI MODEL</u></h2>

### **7. Application Layer**
- **Used by end-user software** such as web browsers and email clients.
- **Provides protocols** that allow software to send and receive information, presenting meaningful data to users.
- Examples of **application layer protocols** include **HTTP (Hypertext Transfer Protocol)**, **FTP (File Transfer Protocol)**, **POP (Post Office Protocol)**, **SMTP (Simple Mail Transfer Protocol)**, and **DNS (Domain Name System)**.

### **6. Presentation Layer**
- **Prepares data** for the application layer.
- Defines how two devices should **encode**, **encrypt**, and **compress data** for proper reception.
- Takes data from the application layer and prepares it for transmission over the session layer.

### **5. Session Layer**
- **Creates communication channels** called **sessions** between devices.
- Responsible for **opening**, **maintaining**, and **closing sessions** while data is being transferred.
- Can set **checkpoints** during data transfer; if interrupted, devices can resume from the last checkpoint.

### **4. Transport Layer**
- Takes data from the session layer and **breaks it into segments** for transmission.
- **Reassembles segments** on the receiving end into data usable by the session layer.
- Manages **flow control** (matches data rate to receiving device) and **error control** (checks and requests missing or incorrect data).

### **3. Network Layer**
- **Breaks up segments** into network packets and reassembles them at the destination.
- Responsible for **routing packets** by determining the best path across a physical network.
- Uses **network addresses** (typically **IP addresses**) to route packets to their destination node.

### **2. Data Link Layer**
- **Establishes and terminates connections** between two physically connected nodes on a network.
- Breaks packets into **frames** and transmits them from source to destination.
- Composed of two sub-layers:
  - **Logical Link Control (LLC)**: Identifies network protocols, performs error checking, and synchronizes frames.
  - **Media Access Control (MAC)**: Uses **MAC addresses** to connect devices and manage transmission permissions.

### **1. Physical Layer**
- Responsible for the **physical cable or wireless connection** between network nodes.
- Defines the **connector, electrical cable, or wireless technology** used for device connectivity.
- Handles the transmission of **raw data** as a series of **0s and 1s** and manages **bit rate control**.

---

### **Advantages of the OSI Model**
- **Helps determine** the required hardware and software to build a network.
- Aids in understanding and **communicating network processes** across a network.
- Facilitates **troubleshooting** by identifying issues at specific network layers, enabling focused problem-solving.
