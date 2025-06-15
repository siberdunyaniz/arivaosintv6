# ARIVA OsintV6 - Open Source Intelligence Tool

**ARIVA OsintV6** is a powerful and user-friendly open-source intelligence (OSINT) tool designed to gather information from various sources, including IP addresses, phone numbers, domain names, and more. This tool is built with Python and supports both **Kali Linux** and **Termux** environments, making it versatile for security researchers, penetration testers, and OSINT enthusiasts.

With a sleek, animated interface and multilingual support (English and Turkish), ARIVA OsintV6 provides a seamless experience for users to perform tasks such as IP geolocation, phone number lookup, WHOIS queries, and random password generation.

---

## Features

- **IP Address Lookup**: Retrieve detailed information about an IP address, including geolocation, ASN, network name, and more using the IPWhois and ipapi.co APIs.
- **Phone Number Lookup**: Extract details about phone numbers, including country, operator, and validity status, using the `phonenumbers` library.
- **WHOIS Lookup**: Query domain names to fetch WHOIS data such as registrar, creation date, expiration date, and contact emails.
- **Random Password Generator**: Generate secure random passwords with customizable lengths.
- **Multilingual Support**: Choose between English and Turkish interfaces.
- **Animated CLI Interface**: Enjoy a visually appealing terminal experience with animated banners and color-coded output using the `pystyle` library.
- **Cross-Platform Compatibility**: Works seamlessly on **Kali Linux**, **Termux**, and other Python-supported environments.
- **Automatic Dependency Installation**: The tool automatically checks and installs required Python modules.

---

## Prerequisites

Before installing and running ARIVA OsintV6, ensure you have the following:

### For Kali Linux
- **Python 3.x** (usually pre-installed on Kali Linux)
- **pip** (Python package manager)
- **Git** (to clone the repository)
- A stable internet connection for installing dependencies and performing lookups
- Basic terminal knowledge

### For Termux
- **Python 3.x** (installable via Termux package manager)
- **pip** (Python package manager)
- **Git** (to clone the repository)
- A stable internet connection
- Storage permissions granted for Termux (to save files and install packages)

### Common Requirements
- Python libraries: `requests`, `phonenumbers`, `ipwhois`, `whois`, `fake_useragent`, `pystyle`
- The tool will automatically install these dependencies during the first run.

---

## Installation

Follow the steps below to install and set up ARIVA OsintV6 on your system.

### On Kali Linux

1. **Update Your System**
   Ensure your system is up-to-date to avoid compatibility issues.
   ```bash
   sudo apt update && sudo apt upgrade -y
   ```

2. **Install Git and Python**
   If not already installed, install Git and Python.
   ```bash
   sudo apt install git python3 python3-pip -y
   ```

3. **Clone the Repository**
   Clone the ARIVA OsintV6 repository from GitHub.
   ```bash
   git clone https://github.com/ArivaTools/arivaosintv6.git
   cd arivaosintv6
   ```

4. **Run the Tool**
   Execute the Python script to start the tool. It will automatically install any missing dependencies.
   ```bash
   python3 arivaosintv6
   ```

### On Termux

1. **Update Termux Packages**
   Update the Termux package manager to ensure you have the latest packages.
   ```bash
   pkg update && pkg upgrade -y
   ```

2. **Install Required Tools**
   Install Git, Python, and other necessary tools.
   ```bash
   pkg install git python -y
   ```

3. **Grant Storage Permissions**
   Allow Termux to access storage for saving files and installing packages.
   ```bash
   termux-setup-storage
   ```

4. **Clone the Repository**
   Clone the ARIVA OsintV6 repository from GitHub.
   ```bash
   git clone https://github.com/ArivaTools/arivaosintv6.git
   cd arivaosintv6
   ```

5. **Run the Tool**
   Start the tool, and it will automatically install missing dependencies.
   ```bash
   python3 arivaosintv6.py
   ```

---

## Usage

Once the tool is installed and running, follow these steps to use it:

1. **Select Language**
   Upon launching the tool, you will be prompted to choose a language:
   - `1` for English
   - `2` for Turkish

2. **Main Menu**
   After selecting a language, the main menu will display the following options:
   - `1. IP Address Info + GeoIP`: Perform an IP address lookup.
   - `2. Phone Number Info`: Lookup details for a phone number.
   - `3. WHOIS Lookup`: Query WHOIS data for a domain.
   - `4. Random Password Generator`: Generate a secure password.
   - `5. Exit`: Quit the tool.

3. **Interacting with the Tool**
   - Enter the number corresponding to your desired option.
   - Follow the prompts to input data (e.g., IP address, phone number, or domain name).
   - The tool will display results in a color-coded, easy-to-read format.
   - Press `Enter` to return to the main menu after each operation.

4. **Example Commands**
   - For IP lookup: Enter a valid IP address (e.g., `8.8.8.8`).
   - For phone lookup: Enter a phone number in international format (e.g., `+905xxxxxxxxx`).
   - For WHOIS lookup: Enter a domain name (e.g., `google.com`).
   - For password generation: Specify the desired password length (e.g., `12`).

---

## Troubleshooting

If you encounter issues while installing or running ARIVA OsintV6, try the following:

- **Dependency Installation Fails**
  - Ensure you have a stable internet connection.
  - Manually install dependencies using pip:
    ```bash
    pip install requests phonenumbers ipwhois whois fake_useragent pystyle
    ```
  - For Termux, ensure storage permissions are granted.

- **Module Not Found Error**
  - Run the tool again; it will attempt to reinstall missing modules.
  - Alternatively, install the missing module manually (e.g., `pip install <module_name>`).

- **API Request Errors**
  - Some lookups (e.g., IP geolocation) require internet access. Verify your connection.
  - Check if the API services (e.g., ipapi.co) are operational.

- **Tool Crashes**
  - Ensure you are using Python 3.x (check with `python3 --version`).
  - Update your Python environment and dependencies:
    ```bash
    pip install --upgrade pip
    pip install --upgrade requests phonenumbers ipwhois whois fake_useragent pystyle
    ```

---

## Contributing

Contributions to ARIVA OsintV6 are welcome! If you’d like to contribute, please follow these steps:

1. Fork the repository on GitHub.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Submit a pull request with a clear description of your changes.

Please ensure your code follows the existing style and includes appropriate comments for clarity.

---

## Credits

- **Developed by**: @ArivaTools
- **GitHub**: [github.com/ArivaTools](https://github.com/ArivaTools)
- **Telegram Channel**: [t.me/ArivaTools](https://t.me/ArivaTools)
- **Contributor**: @AtahanArslan

Special thanks to the open-source community for providing the libraries used in this project.

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Disclaimer

ARIVA OsintV6 is intended for educational and ethical purposes only. The developers are not responsible for any misuse or illegal activities conducted with this tool. Always obtain proper authorization before performing OSINT activities on any target.

---

**Happy OSINT Hunting with ARIVA OsintV6!**  
Join our Telegram channel for updates and support: [t.me/ArivaTools](https://t.me/ArivaTools)