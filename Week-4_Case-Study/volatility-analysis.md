## 📄 3. `volatility-analysis.md`

```markdown
# Volatility Memory Forensics - RAM Analysis

## 🧪 Evidence: memory.dmp

Captured using DumpIt after the ransomware simulation.

---

## Setup
- Tool: Volatility 2.6
- Profile: Win10x64_18362

---

## Key Commands Used

### 1. Identify Profile
```bash
volatility -f memory.dmp imageinfo

###2.Check for Malware Injection
bash

volatility -f memory.dmp --profile=Win10x64_18362 malfind

###3. List Processes
bash

volatility -f memory.dmp --profile=Win10x64_18362 pslist

###4. Network Connections
bash

volatility -f memory.dmp --profile=Win10x64_18362 netscan

###5.Command History

volatility -f memory.dmp --profile=Win10x64_18362 cmdscan