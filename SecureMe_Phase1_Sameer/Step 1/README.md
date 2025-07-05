# 🔐 Cybersecurity Practical Lab Tasks

This repository includes hands-on tasks based on the **CIA Triad** and **IAAAA** (Identity, Authentication, Authorization, Accountability, Audit Trail) model — essential foundations in cybersecurity.

---

## 🔷 CIA TRIAD TASKS

### 1️⃣ Confidentiality — GPG Encryption
- 🔒 Encrypted `demo.txt` using `gpg` (symmetric encryption)
- Ensured data confidentiality by protecting content with a passphrase
- Verified encryption using `gpg -d demo.txt.gpg`

### 2️⃣ Integrity — File Hash Verification with `sha256sum`
- Generated SHA-256 hash of a file before and after editing
- Used `sha256sum demo.txt` to ensure file was not tampered with
- Demonstrated how hashing provides data integrity verification

### 3️⃣ Availability — Simulate DoS using `hping3` and Apache
- Hosted a static web server using Apache
- Simulated a DDoS attack using `hping3`
- Observed and documented availability threats and Apache logs during the flood

---

## 🛡️ IAAAA SECURITY MODEL TASKS

### 1️⃣ Identity + Authorization — Linux Users and Permissions
- Created users with `useradd`, assigned passwords
- Controlled access to files using `chmod`
- Added a user to the `sudo` group using `usermod`
- **Learning Outcome**: Distinction between user identity and resource-level authorization

### 2️⃣ Authentication — SSH Key-Based Login
- Generated key pairs using `ssh-keygen`
- Configured server (`sshd_config`) for public key authentication
- Verified passwordless SSH login using authorized key
- **Learning Outcome**: Secure authentication without using passwords

### 3️⃣ Accountability — Sudo Logging with `sudoers` and `rsyslog`
- Enabled sudo command logging via `Defaults logfile="/var/log/sudo.log"`
- Verified privileged actions were recorded in the log
- Optional redirection using custom rsyslog config
- **Learning Outcome**: All privileged actions were traceable to users

### 4️⃣ Audit Trail — Log File Analysis (`journalctl` on Kali)
- Analyzed user login, logout, and sudo actions using:
  ```bash
  journalctl | grep "session opened"
  journalctl | grep "sudo"
  journalctl | grep "Failed password"

