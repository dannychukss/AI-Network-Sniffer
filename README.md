# AI-Powered Network Sniffer

## Objective
The AI Network Sniffer project aimed to build a custom, programmatically driven utility to capture, parse, and analyze live network traffic. The primary focus was to monitor packet data in real-time, identify anomalous or malicious IP addresses using automated intelligence, and instantly broadcast alerts to defenders. This hands-on project was designed to deepen practical knowledge of socket programming, packet structures, and automated incident response logic.

### Skills Learned
Through this project, I gained hands-on experience with:
- **Network Security:** Implemented defensive boundaries by identifying structural anomalies in passing data streams, enforcing baseline monitoring, and evaluating secure versus insecure protocol behaviors.

- **Packet Analysis:** Developed logic to capture raw network sockets and parse core protocol headers (including TCP, UDP, and ICMP) to inspect packet sizes, flags, and source/destination pathways.

- **Threat Intelligence:** Engineered automated API integration with VirusTotal to cross-reference extracted IP data against globally updated malicious signatures and reputation datasets.

- **Security Monitoring:** Established continuous visibility over network segments by logging live telemetry data into indexed CSV baselines for active auditing and pattern tracking.

- **Machine Learning in Cybersecurity:** Utilized classification models to dynamically evaluate live traffic metrics, training the system to differentiate standard behavior from automated DDoS patterns or brute-force attempts.

- **SOC Operations:** Maintained a bird's-eye view of security environments by combining live log analysis, geographic tracking, and automated SMTP email alert logic to notify defenders of critical thresholds.

- **Flask Web Development:** Architected an interactive, backend-driven administrative dashboard to display real-time security telemetry, incoming data feeds, and model classifications visually.

### Tools Used
- **Python:** Core programming language for socket data parsing, traffic logic, and ML model execution.
- **Flask:** Lightweight framework used to build and serve the live web-based SOC dashboard.
- **VirusTotal API:** Integrated threat intelligence stream used to cross-reference IPs against known malicious datasets.
- **Scikit-Learn / Machine Learning Frameworks:** Utilized for building and applying the threat classification models.
- **SMTP / Email Protocols:** Configured to handle programmatic, automated security alert dispatches.

### Core Features

- **Real-time Packet Sniffing & Traffic Analysis:** Implements raw socket connections in Python to capture, intercept, and process live layer-3 and layer-4 network data as it traverses local interfaces.

- **Protocol Detection (TCP, UDP, ICMP):** Dynamically parses network headers to isolate and categorize traffic by protocol, enabling structural inspection of packet behaviors and payloads.

- **Machine Learning-Based Threat Classification:** Utilizes a trained classification model to evaluate live traffic signatures on the fly, accurately distinguishing benign user behavior from potentially hostile payloads.

- **DDoS & Suspicious Traffic Detection:** Monitors packet velocity, volume metrics, and repeating packet strings to identify and flag anomalies characteristic of Distributed Denial of Service (DDoS) and brute-force attacks.

- **VirusTotal Threat Intelligence Integration:** Programmatically extracts source and destination IP addresses from captured packets and cross-references them via API against global threat intelligence feeds.

- **GeoIP Tracking for Source Analysis:** Resolves public IP structures into geographic locations, providing valuable spatial context on external traffic sources and threat origins.

- **Automated Email Alert System:** Features an automated SMTP alerting module that triggers instant email notifications to infrastructure administrators the moment high-risk thresholds are crossed.

- **Flask-Powered Live SOC Dashboard:** Provides a responsive, web-based central management console to visualize streaming telemetry, protocol breakdowns, and current classification models visually.

- **CSV Logging for Auditing & Model Training:** Streamlines data operations by continuously appending parsed packet data to structural CSV files, providing historical logs for incident auditing and subsequent model tuning.


## Steps


*Ref 1: Launching the Sniffer and Flask SOC Dashboard*
<img width="1600" height="900" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/a9f59809-74ba-4c18-a122-5bd3f982d21f" />
_This screenshot shows the initial bootup sequence of the sniffer script and the live initialization of the local Flask web framework._




<img width="1600" height="900" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/19f298d6-1dd5-47e7-b54d-f96149c66c0c" />


<img width="1170" height="1379" alt="IMG_2375" src="https://github.com/user-attachments/assets/03d0112b-aed8-49e0-843b-73098adb7b48" />


<img width="1170" height="1361" alt="IMG_2376" src="https://github.com/user-attachments/assets/b897ffab-c0d3-4131-818e-1485ee9d2fb4" />


<img width="1170" height="2532" alt="IMG_2374" src="https://github.com/user-attachments/assets/89f1dfa2-4793-4a3a-96cf-31e3055b0095" />



---

*Ref 2: Real-time Traffic Ingestion and Threat Intelligence Flags*

<img width="1600" height="900" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/b236034f-6f3e-409c-b14a-89eb08fd3f8c" />


<img width="1600" height="900" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/366c1709-785e-4188-ad04-fd9306a1b554" />

_Here, the sniffer is actively capturing TCP and UDP streams. The system automatically queries the VirusTotal API when an unfamiliar external IP is detected, logging the results to our CSV file._

---

*Ref 3: Automated Email Alert Triggered by DDoS Simulation*
![Email Alert Notification](https://github.com/YOUR_GITHUB_USERNAME/repo/assets/image-link-3.png)
_When traffic thresholds are breached (simulating a DDoS scenario), the script immediately executes an SMTP routine to dispatch an automated security alert directly to the administrator's mailbox._

---

### 📺 Video Demonstration
[![Watch the Demo](https://img.shields.io/badge/▶_Watch_Project_Demo_on_LinkedIn-0072b1?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/posts/chuks-daniel_cybersecurity-socanalyst-blueteam-activity-7466411795642130434-HRoA?utm_source=share&utm_medium=member_ios&rcm=ACoAAF68i9cBQ3sKIg1Z8O-VvnmusZZxm6zb-Qw)

_Click the badge above to watch a full video walk-through of the AI Network sniffer capturing live traffic, identifying threats, and triggering alerts._
