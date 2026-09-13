# 🛜 Windows Wi-Fi Profile Extractor

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

A Python automation script built to query the Windows WLAN command-line utility (`netsh`), extract saved wireless network profiles, parse security keys, and display plaintext Wi-Fi credentials.

---

## 🚀 Key Functionalities

| Feature | Description |
| :--- | :--- |
| **Profile Enumeration** | Executes system commands via the `subprocess` module to parse all saved Wi-Fi SSID profiles on a Windows machine[cite: 16]. |
| **Security Validation** | Filters out unsecured or open networks by checking individual profile security keys[cite: 16]. |
| **Credential Retrieval** | Automatically queries profiles with the `key=clear` argument to extract and structure plaintext passwords[cite: 16]. |

## 🛠️ Technical Implementation

* **Subprocess Automation:** Leverages Python's native `subprocess` library to capture standard output streams from native Windows networking tools[cite: 16].
* **Regular Expressions:** Uses the `re` module to locate specific regex patterns, extracting profile names and passwords directly from command-line outputs[cite: 16].
* **Data Structuring:** Automatically maps retrieved SSIDs and credentials into structured Python dictionaries before printing[cite: 16].

## 📦 Getting Started

### Prerequisites

* Windows operating system (with wireless networking capabilities).
* Python 3.x installed on your system.

### Installation & Execution

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/norafrank-official/windows-wifi-extractor.git](https://github.com/norafrank-offcial/windows-wifi-extractor.git)
   cd your-repo-name
