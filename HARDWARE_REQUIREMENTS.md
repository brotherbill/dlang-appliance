# HARDWARE_REQUIREMENTS.md
###### /dev/repos/dlang-appliance/HARDWARE_REQUIREMENTS.md

# Hardware Requirements for the D Learning Appliance  
# Deterministic. Testable. Parent‑Grade. Operator‑Grade. Institutional‑Grade.

This file defines the approved hardware, minimum specifications, physical security requirements, and refurb acceptance criteria for all D Learning Appliances.

A man’s got to know his limitations.  
This file defines the appliance’s.

---

## 1. APPROVED DEVICE CLASSES
Only the following device classes may be used as appliances:

- Mini PCs with x86_64 architecture  
- Fanless or low‑noise designs preferred  
- Integrated GPU acceptable (no discrete GPU required)  
- Must support secure boot  
- Must support UEFI firmware  
- Must support hardware‑level device locking  

No laptops.  
No tablets.  
No ARM devices unless explicitly approved in doctrine.

---

## 2. MINIMUM HARDWARE SPECIFICATIONS
All appliances must meet or exceed:

- **CPU:** 4‑core x86_64  
- **RAM:** 8 GB minimum (16 GB preferred)  
- **Storage:** 256 GB SSD minimum  
- **Network:** Gigabit Ethernet + Wi‑Fi  
- **Ports:**  
  - 2× USB‑A  
  - 1× USB‑C (optional)  
  - 1× HDMI or DisplayPort  
- **Power:** External power brick or internal PSU with stable output  

No spinning disks.  
No eMMC storage.  
No unstable power supplies.

---

## 3. PHYSICAL SECURITY REQUIREMENTS
Every appliance must support:

- **Kensington lock slot** (mandatory for Level 2 and Level 3)  
- **Steel‑braided cable lock**  
- **Fixed anchor point**  
- **Cable routing with no slack**  
- **Tamper‑evident seals** (Level 3 only)  

If the device cannot be physically secured, it cannot ship.

---

## 4. POWER REQUIREMENTS
All appliances must:

- use grounded power  
- avoid shared power strips in institutional settings  
- support surge protection  
- maintain stable voltage under load  
- include cable strain relief  

Power instability is grounds for refurb rejection.

---

## 5. STORAGE REQUIREMENTS
Storage must be:

- SSD only  
- 256 GB minimum  
- 512 GB preferred for operator‑grade deployments  
- partitionable for RCA  
- capable of secure wipe  

No hybrid drives.  
No SD‑card‑based systems.  
No USB‑boot appliances.

---

## 6. RAM REQUIREMENTS
RAM must be:

- 8 GB minimum  
- 16 GB preferred  
- non‑ECC acceptable for home use  
- ECC recommended for institutional use  

RAM must pass memory diagnostics before shipping.

---

## 7. NETWORK REQUIREMENTS
All appliances must support:

- Gigabit Ethernet  
- 2.4 GHz and 5 GHz Wi‑Fi  
- MAC address logging for RCA  
- deterministic network configuration  

Level 3 appliances must support:

- network disablement  
- air‑gap mode  
- no active interfaces unless operator‑enabled  

---

## 8. PERIPHERAL REQUIREMENTS
Required peripherals:

- wired keyboard  
- wired mouse  
- HDMI or DisplayPort cable  
- power supply  
- Kensington lock + cable  

Optional peripherals:

- USB headset  
- USB microphone  
- USB webcam  

Wireless peripherals are discouraged for Level 2 and forbidden for Level 3.

---

## 9. REFURB ACCEPTANCE CRITERIA
A returned appliance enters refurb only if:

- chassis is intact  
- ports are functional  
- power is stable  
- SSD passes diagnostics  
- RAM passes diagnostics  
- Kensington lock slot is undamaged  
- no signs of tampering (Level 3)  

If any requirement fails, the device is recycled.

---

## 10. NO DRIFT RULE
Hardware requirements must remain consistent across:

- dlang-appliance  
- dlang-school  
- from-dead-box-to-dev-box  

If one changes, all must change.

---

## 11. HUMAN OVERRIDE RULE
If a conflict arises between:

- HARDWARE_REQUIREMENTS.md  
- LOCKDOWN_LEVELS.md  
- MISSION2.md  
- MY_RULES.md  
- chat instructions  

**MY_RULES.md wins**, unless the human operator (Brother Bill) explicitly overrides it.

---

End of file.
