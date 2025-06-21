# 🛡️ Cyber Threat Intelligence Dashboard

A live Streamlit-based dashboard that automatically fetches and displays the latest **Indicators of Compromise (IOCs)** from the [Abuse.ch ThreatFox API](https://threatfox.abuse.ch/). Built as part of a cybersecurity internship project to demonstrate practical Threat Intelligence skills.

---

## 📸 Dashboard Interface

![CTI Dashboard](screenshots/CTI dashboard.png)

> *Screenshot: Live threat feed visualized using Streamlit*

---

## 📂 Sample Output

Here’s a sample of the data extracted and processed by the dashboard:

📄 [`cyber threat intelligence dashboard.csv`](data/cyber threat intelligence dashboard.csv)

- Contains over 200+ live IOCs
- Types: `ip:port`, `domain`, `url`
- Threat Categories: `botnet_cc`, `payload_delivery`, etc.

---

## ⚙️ Technologies Used

| Tool         | Purpose                       |
|--------------|-------------------------------|
| 🐍 Python     | Core programming language     |
| 📊 Streamlit  | Interactive dashboard         |
| 🌐 Requests   | REST API interaction          |
| 📄 Pandas     | Data parsing and display      |
| 📡 ThreatFox  | Source of real-time IOC data  |

---

## 💡 Features

- Live IOC retrieval from ThreatFox API
- Real-time table view in browser
- Exportable CSV data
- Error handling for failed requests or invalid JSON
- Structured codebase with `scripts/` and `dashboard/`

---

## 🧪 How to Run Locally

```bash
git clone https://github.com/YOUR_USERNAME/cyber-threat-intel-dashboard.git
cd cyber-threat-intel-dashboard

# Setup virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run the dashboard
streamlit run dashboard/app.py
