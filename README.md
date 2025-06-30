# Task-5-Capture-and-Analyze-Network-Traffic-Using-Wireshark
# Task 5: Capture and Analyze Network Traffic Using Wireshark  


---

## 🎯 Objective  
Capture live network packets using Wireshark, identify protocols (TCP, TLS, DNS, etc.), and document key findings.  

---

## 📝 Deliverables  
1. Packet capture file: https://github.com/nainaisrat/Task-5-Capture-and-Analyze-Network-Traffic-Using-Wireshark/blob/main/.pcap%20file.pcapng
2. Analysis report: https://github.com/nainaisrat/Task-5-Capture-and-Analyze-Network-Traffic-Using-Wireshark/blob/main/Task%205%20report%20%20Capture%20and%20Analyze%20Network%20Traffic%20Using%20Wireshark.pdf
3. Wireshark filtering examples  

---

## 🔧 Methodology  
1. **Captured Traffic** for 60 seconds while:  
   - Browsing `chromewebstore.googleapis.com`  
   - Visiting Kaspersky sites (`ds.kaspersky.com`)  
   - Pinging `8.8.8.8`  
2. **Filtered Packets** in Wireshark using:  
   ```bash
   tcp.port == 443    # HTTPS traffic
   dns                # DNS queries
   tls                # TLS-encrypted data
   arp                # Local device discovery
