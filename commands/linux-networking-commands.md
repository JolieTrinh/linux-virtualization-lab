# Essential Linux System & Network Administration Commands

A curated list of core Linux CLI utilities used for system inspection, network diagnostics, process management, and service control during hands-on lab environments.

---

## System Information

* `whoami`
  > Displays the current logged-in username.
* `hostname`
  > Shows the system's network name.
* `hostnamectl`
  > Provides detailed system architecture, OS version, kernel release, and hostname details.
* `uname -a`
  > Prints complete system information, including kernel version and system architecture.

---

## Networking & Port Diagnostics

* `ip addr`
  > Displays all network interfaces, assigned IPv4/IPv6 addresses, and connection states.
* `ip -br addr`
  > Shows a brief, one-line summary of network interfaces and their IP addresses.
* `ip route`
  > Displays the IP routing table and default gateway configurations.
* `ping <IP_or_Domain>`
  > Tests Layer 3 network reachability and latency to a destination host.
* `sudo ss -tulpn`
  > Displays active listening sockets, open ports, and associated running processes (`-t` TCP, `-u` UDP, `-l` Listening, `-p` Process, `-n` Numeric IPs/Ports).

---

## Process Monitoring

* `ps aux`
  > Displays a detailed snapshot of all currently running processes across all users.
* `top`
  > Provides a real-time dynamic view of active system processes, CPU usage, and memory consumption.

---

## System Resource Utilization

* `free -h`
  > Displays total, used, and available RAM and Swap space in human-readable format (e.g., MB/GB).
* `df -h`
  > Displays storage disk space usage across all mounted filesystems in human-readable units.

---

## 🛠 Service Management

* `systemctl status ssh`
  > Checks the operational state (active/running, inactive, or disabled) of the OpenSSH daemon.