# Honeypot | Microsoft Sential Map | SEIM

### Summary:

---

The objective of this lab is to grasp the process of collecting honeypot attack logs, querying this data within a SIEM framework, and presenting it in a comprehensible format. Specifically, the data will be visualized on a world map, showcasing event counts and geolocations to facilitate easy understanding and analysis of such information.

SIEM, short for Security Information and Event Management System, serves as a crucial tool for organizations in identifying, analyzing, and mitigating security threats proactively to safeguard business operations. This system gathers event log data from diverse network sources like Firewalls, IDS/IPS, and Identity solutions, empowering security professionals to oversee, prioritize, and address potential threats promptly. Conversely, a honeypot acts as a security strategy by setting up a virtual trap in a controlled environment to attract attackers. It's essentially an intentionally compromised system used to study attack methods, assess various threats, and enhance security protocols.

### Learning Objectives:

---

* Configuration & Deploy Azure tools like virtual machine, Log analytics workspace, Azure Sentinel.
* Hands-on experience and working of Microsoft's Azure Sentinel SIEM tool.
* Understand Windows Security Event logs
* Display attack data on a dashboard with Workbooks (World Map)

### Tools Used:

---

* **Azure Cloud**: Used to deploy Windows virtual machine and Log analytics workspace.
* **Azure Sentinel(SIEM)**: Used for Mapping the failed RDP logins using the log files.
* **Custom PowerShell script**: This script would allow us to fetch logs from EventViewer in Windows.
* **Ipgeolocation.io**: API which allows to get geolocation from IP address.
* **RDP**: Windows Remote Desktop Protocols allows us to connect to the VM and configure to open up the Fire wall.

### Log File Overview:

---

Running the Custom Powershell scipt would provide us the logs containing the geo location, ip address, timestamp and the username they are trying to use.

Credits to **Josh Madakor([Github](https://github.com/joshmadakor1/Sentinel-Lab/tree/main))** for providing the custom powershell script which allows the fetch the geo location, ip address, timestamp, username from Windows Event Viewer where event Id = 4625 (unsuccessful logons).

![1711469311731](image/README/1711469311731.png)

### World Map of Incoming attack after 30 mins since the machine started (Built custom logs including geodata)

---

![1711470157656](image/README/1711470157656.png)


### World Map of Incoming Attack after 8 hours (Built custom Logs including geodata)

---

![1711470238339](image/README/1711470238339.png)
