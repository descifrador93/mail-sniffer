
# Mail Sniffer

This is a simple Python script for sniffing network traffic to detect potential email credentials being sent in plaintext. It utilizes the scapy library for packet sniffing and dissection.

## Requirements
`Python 3.x`
`A Linux Machine`
`scapy`

## Usage
- Clone the repository or download the `mail_sniffer.py` file.
- Install scapy using -
```shell
pip install scapy
```


## How it Works

The script listens for TCP traffic on ports commonly used for email protocols (110, 25, and 143). When it captures a packet containing payload data, it checks if the payload contains the strings "user" or "pass", indicating potential email credentials. If found, it prints the destination IP address and the payload content.

## Disclaimer

This script is for educational purposes only. Sniffing network traffic may be illegal or unethical in certain circumstances. Always ensure you have proper authorization before using this tool.
    