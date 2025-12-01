# Azure Honeypot Project 🐝


<p align="center">
  <img src="https://github.com/user-attachments/assets/dd970817-9540-4aa6-a7e3-4d89016002f5" width="900">
</p>


Honeypot project in Microsoft Azure to analyze real-world brute-force attacks using **Microsoft Sentinel**. This project simulates a **Security Operations Center (SOC)** and demonstrates threat detection, incident response, and visualization.

---

## 🚀 Project Overview
I deployed a Windows VM honeypot in Azure by intentionally exposing it to the public internet. Over a week, I monitored attacks and captured real-world brute-force attempts.  

**Key Observations (from workbook):**
- **Total failed logons:** 75,000+  
- **Unique attacking IPs:** 50+  
- **Top attacker locations:**
  - Jordanow (Poland) – 29.9K
  - Tilburg (Netherlands) – 24.1K
  - Lahore (Pakistan) – 22.3K
  - Ho Chi Minh City (Vietnam) – 12.4K
  - Maarn (Netherlands) – 7.54K
- **Other attacks** – 7.77K from various countries

---

## 🛠 Technologies Used
- Microsoft Azure
- Windows 10 VM
- Network Security Group (NSG) / Firewall
- Microsoft Sentinel (SIEM)
- Log Analytics Workspace
- Kusto Query Language (KQL)
- Map Workbooks & Dashboards

---

## ⚡ Setup Steps

1. **Azure Subscription & Resource Group** – create a subscription and resource group in your preferred region.  
2. **Virtual Network & VM** – deploy a Windows 10 VM and expose it to the public internet.  
3. **Honeypot Exposure** – configure NSG to allow inbound traffic, check EventID 4625 for failed logons.  
4. **Log Collection & Sentinel Integration** – create a Log Analytics Workspace, activate Microsoft Sentinel, install the Windows Security Events connector.  
5. **Data Analysis & Visualization** – run KQL queries and build a map workbook to visualize attacker locations and activity.  
6. **Custom Detection & Incident Response** – create a Sentinel Analytics Rule to detect brute-force attempts, investigate incidents, and block malicious IPs.

---

### 📈 Results (Top Locations)
| Location | Failed Logons |
|----------|---------------|
| Jordanow, Poland 🇵🇱 | 29,900 |
| Tilburg, Netherlands 🇳🇱 | 24,100 |
| Lahore, Pakistan 🇵🇰 | 22,300 |
| Ho Chi Minh City, Vietnam 🇻🇳 | 12,400 |
| Maarn, Netherlands 🇳🇱 | 7,540 |
| Other countries | 7,770 |

---

## 🎯 Learning Outcomes
- Hands-on experience building a cloud-based SOC environment.  
- Practical exposure to **real-world brute-force attacks**.  
- Experience with **Microsoft Sentinel, Log Analytics, and KQL** for detection and visualization.  
- Understanding of **incident response workflows** in the cloud.

---

## 🔗 References
- Microsoft Azure: [https://azure.microsoft.com](https://azure.microsoft.com)  
- Microsoft Sentinel Docs: [https://learn.microsoft.com/en-us/azure/sentinel/](https://learn.microsoft.com/en-us/azure/sentinel/)
