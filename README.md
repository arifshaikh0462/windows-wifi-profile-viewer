# Windows Wi-Fi Profile Viewer 🔐

A Python script that retrieves saved Wi-Fi profiles and their stored passwords on **Windows systems** using the built-in `netsh` command.

> ⚠️ This project is intended for **educational purposes, personal recovery, and authorized system administration only**.

---

## 📌 Features

- Lists all saved Wi-Fi profiles on a Windows machine
- Displays stored Wi-Fi passwords (if available)
- Uses native Windows networking commands
- No external Python libraries required

---

## 🛠️ Requirements

- Windows OS
- Python 3.x
- Administrator privileges (recommended)

---

## 🚀 How It Works

The script internally executes the following Windows commands:

```bash
netsh wlan show profiles
netsh wlan show profile "PROFILE_NAME" key=clear
It parses the command output to extract:

Wi-Fi profile names

Stored passwords (Key Content)

▶️ Usage
Clone the repository:

bash
Copy code
git clone https://github.com/arifshaikh0462/windows-wifi-profile-viewer.git
Navigate to the project directory:

bash
Copy code
cd windows-wifi-profile-viewer
Run the script:

bash
Copy code
python wifipass.py

📷 Sample Output
markdown
Copy code
Home_Network                  |  mypassword123
Office_WiFi                   |  ********
Cafe_Free                     |

⚠️ Disclaimer
This tool is provided strictly for educational and authorized use only.

Do NOT use this script on networks you do not own or do not have permission to access.

Unauthorized access to computer networks is illegal.

The author is not responsible for misuse of this code.

📚 Learning Objectives
This project demonstrates:

Windows WLAN management using netsh

Python subprocess module usage

Parsing command-line output

Basic cybersecurity and network auditing concepts

📄 License
This project is licensed under the MIT License.

🤝 Contributions
Contributions, suggestions, and improvements are welcome.
If you find this project useful, consider giving it a ⭐!

