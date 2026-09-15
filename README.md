# WebX — Website Reconnaissance & Intelligence Toolkit

WebX is a web reconnaissance and intelligence toolkit that collects useful information about a website from a single interface. It helps security researchers and cybersecurity enthusiasts gather information about a target website during the reconnaissance phase.

## Project Structure

* `frontend/` – React + Vite frontend providing the web-based dashboard.
* `backend/` – Python Flask backend that performs website analysis and information gathering.

## Running the Project

### 1. Start the Backend API

```powershell
cd backend
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python app.py
```

The backend runs on:

```text
http://127.0.0.1:8000
```

### 2. Start the Frontend

```powershell
cd frontend
npm install
npm run dev
```

Then open the local Vite URL shown in the terminal.

## Key Features

* 🌐 **Website Information** – Collects important information related to a given website.
* 🔍 **WHOIS Information** – Provides domain registration details such as registrar, creation date, and expiry date.
* 🌍 **IP & Geolocation** – Finds the website's IP address, location, ISP, organization, and ASN information.
* 🛠️ **Technology Detection** – Identifies technologies, web servers, frameworks, CDN/WAF services, and other technologies used by the website.
* 🔐 **SSL/TLS Information** – Provides certificate details, issuer, validity, protocols, cipher information, and SANs.
* 🌐 **DNS Information** – Retrieves DNS records including A, AAAA, MX, TXT, and NS records.
* 📧 **Email Security** – Checks SPF and DMARC configurations.
* 📋 **Security Headers** – Checks important HTTP security headers configured on the website.
* 🔗 **Redirect Analysis** – Shows HTTP response time and redirect chains.
* 📄 **Security Files** – Checks files such as `robots.txt` and `security.txt`.
* 🔌 **Port Scanning** – Scans commonly used ports to identify potentially available services.
* 🎣 **Phishing Analysis** – Performs basic heuristic checks for suspicious domain characteristics.
* 📊 **Security Summary** – Provides a summarized view of the collected website information.
* 📥 **Report Export** – Allows the collected information to be exported for further analysis.

## Purpose

WebX is mainly designed for the **reconnaissance phase of cybersecurity**. Instead of manually collecting information from different tools and sources, WebX brings commonly useful website intelligence into one place.

The collected information can help security researchers understand a website's infrastructure, technologies, DNS configuration, security settings, and publicly available domain information before performing further security analysis.

## Technology Stack

* **Frontend:** React.js, Vite
* **Backend:** Python, Flask
* **Security & Reconnaissance:** WHOIS, DNS, SSL/TLS analysis, port scanning, technology fingerprinting

## 👨‍💻 Author

**Prasad Nalla**
*Cybersecurity Enthusiast & Full-Stack Developer*

## 📄 License

This project is licensed under the MIT License.
