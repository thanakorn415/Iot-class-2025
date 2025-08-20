# 📄 Debian Installation Report for IoT, MQTT, Kafka Course

> Students must complete all sections of this form during Debian installation and submit it upon completion.

---

## 🔧 General Information

| Title                  | Value                                               |
| -----------------------| --------------------------------------------------- |
| Full Name              | Thanakorn Thanakarn|
| Student ID              | 6510301023 |
| Installation Date      | 11 Jan 2025 |


---

## 🖥️ Device Information

- 💻 **Device Model / Type**: VM
- 🧬 **Firmware Type**:  
  - [ ] UEFI  
  - [x] BIOS  
- 🏷️ **Installation Type**:  
  - [] Physical PC  
  - [x] Virtual Machine (VM)

---

## 🗂️ Custom Partitioning

| Partition     | Size   | Filesystem | Mount Point           | Notes              |
|---------------|--------|------------|------------------------|--------------------|
| `/boot`       | 512MB  | ext4       | `/boot`                | For boot loader    |
| `swap`        | 1GB    | swap       | -                      | Swap space         |
| `/` or others | 19GB   | ext4       |    `/`                 | Root filesystem    |


| `udev`        | 1.9G   | udev       | `/dev`                 | Devicefiles                  |
| `tmpfs`       | 392M   | tmpfs      | `/run`                 | Temporary runtime files       |
| `/dev/sda1`   | 31G    | ext4       | `/`                    | Root filesystem               |
| `tmpfs`       | 2.0G   | tmpfs      | `/dev/shm`             | Shared memory (RAM-based)     |
| `tmpfs`       | 5.0M   | tmpfs      | `/run/lock`            | Lock files                    |
| `tmpfs`       | 392M   | tmpfs      | `/run/user/1000`       | User session temporary files  |



---

## 🌐 Network Configuration (Static IP)

| Title                   | Value                                               |
| ------------------------| --------------------------------------------------- |
| Network Interface Name  | enp0s18     |
| IP Address              | 172.30.15.36 |
| Netmask                 | 255.255.255.0 |
| Gateway                 | 172.30.15.68 |
| DNS                     | 172.16.46.254 |

---

## 🖧 Hostname

- 🖥️ **Hostname Set**: FDT6510301023

---

## 👤 User Account

- 👨‍💻 **Username Created**: thanakorn
- 🔐 **Is a Root Password Set?**:  1234
  - [X] Yes  
  - [ ] No

---

## ✅ Additional Problems Notes (if any)

> _____________________________________________________________________  
> _____________________________________________________________________  
> _____________________________________________________________________

