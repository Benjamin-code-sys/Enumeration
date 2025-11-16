# Post-Compromise Enumeration (Windows & Linux)

After gaining a low-privilege foothold during an authorized assessment, the goal of post-compromise enumeration is to understand the host’s context, identify misconfigurations, and map safe escalation paths. 

There are various tools we can leverage for this including the following:  
• WinPEAS  
• SeatBelt  
• WinEnum  
Although this tools prove useful for this, they can often be misleading sometimes and we should always double check on information we aren't sure about. Furthermore they are heavily signatured by most AV engine.

---

## 🟦 Windows Post-Compromise Enumeration

### 🔹 What to Focus On
- **System Info:** OS version, patch level, installed programs, EDR/AV presence.  
- **Users & Groups:** Current user, group memberships, active sessions.  
- **Processes & Services:** Running processes, service configs, scheduled tasks.  
- **File System:** Writable directories, weak ACLs, sensitive files.  
- **Network:** Listening ports, outbound connections, mapped drives.

### 🔹 Key Enumeration Tools

#### **WinPEAS**
- Automated privilege-escalation indicator scanner.  
- Highlights weak permissions, misconfigurations, services, tasks, environment data, and more.

#### **Seatbelt**
- Modular C# auditing tool.  
- Enumerates system info, user contexts, installed software, browser artifacts, and security-relevant settings.

#### **WinEnum**
- Lightweight host-information collector.  
- Quick snapshot of users, services, processes, tasks, and network configuration.

---

## 🔴 Linux Post-Compromise Enumeration

### 🔹 What to Focus On
- **System Details:** Kernel version, distro, installed packages, running modules.  
- **Users & Privileges:** Current user, groups, sudo rules, last logins.  
- **Services & Cron Jobs:** Systemd units, daemons, cron tasks, startup scripts.  
- **File System:** Writable paths, SUID/SGID binaries, sensitive configs in `/etc` and home directories.  
- **Network:** Listening sockets, active connections, routing table, reachable hosts.

---

This section provides a concise overview suitable for quick reference during enumeration phases of authorized security assessments.

