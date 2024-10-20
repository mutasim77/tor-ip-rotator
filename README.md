# Tor-IP-Rotator 🧅🔐
Tor-IP-Rotator is a Python script that automates the process of changing your IP address through the Tor network at specified intervals. This tool is designed for educational purposes to demonstrate concepts of anonymity, networking, and cybersecurity.

## Disclaimer ⚠️
This tool is for educational purposes only. Ensure you comply with all relevant laws and terms of service when using this script. The author is not responsible for any misuse or damages arising from the use of this tool.

## Prerequisites 🌀
- Python 3.6+
- Tor service installed and running
- `stem`, `requests`, and `colorama` Python libraries

## Installation 📡
1. Install Tor:
   - On macOS: `brew install tor`
   - On Ubuntu: `sudo apt-get install tor`

2. Clone this repository:
   ```
   git clone https://github.com/mutasim77/tor-ip-rotator.git
   cd tor-ip-rotator
   ```

3. Install required Python libraries:
   ```
   pip install -r requirements.txt
   ```

4. Configure Tor:
   Create or edit the torrc file (usually located at /usr/local/etc/tor/torrc on macOS or /etc/tor/torrc on Linux) and add:
   ```
   ControlPort 9051
   CookieAuthentication 1
   ```

5. Restart the Tor service:
   - On macOS: `brew services restart tor`
   - On Ubuntu: `sudo service tor restart`

## Usage 🦹
Run the script with Python:

```
python tor_ip_rotator.py [interval]
```

- `interval` (optional): Number of seconds between IP rotations (minimum 3, default 3)

Example:
```
python tor_ip_rotator.py 5
```

This will rotate your IP address every `5` seconds.

## Features 🧪
- Automatic IP rotation through Tor
- Customizable rotation interval
- Colored console output for better readability
- Displays current IP address after each rotation
- Counts and displays total number of rotations

## Contributing 🤝
Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/mutasim77/tor-ip-rotator/issues) if you want to contribute.

## License 📄
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
