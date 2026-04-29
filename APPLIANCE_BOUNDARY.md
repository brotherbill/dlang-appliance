# APPLIANCE_BOUNDARY.md
###### /dev/repos/dlang-appliance/APPLIANCE_BOUNDARY.md

# Appliance Boundary Definition  
# The User Owns the Hardware.  
# The Appliance Is the Managed Environment.

This file defines the boundary between the general‑purpose computer owned by the user and the D Learning Appliance installed on that computer.  
The distinction is critical for warranty, support, liability, and doctrinal clarity.

A man’s got to know his limitations.  
This file defines the appliance’s.

---

## 1. HARDWARE OWNERSHIP
The user owns the physical device.

They may:

- install any operating system  
- dual‑boot  
- replace the SSD  
- replace the RAM  
- install any software  
- modify the filesystem  
- wipe the drive  
- use the device for any purpose  

The hardware is theirs.  
Their rights are unrestricted.

---

## 2. WHAT THE APPLIANCE IS
The D Learning Appliance is:

- a managed environment  
- a controlled curriculum platform  
- a deterministic software stack  
- a reproducible Golden Master image  
- an RCA‑bound system  
- a lockdown‑governed environment  
- a supportable, testable, auditable subsystem  

The appliance is **not** the hardware.  
It is a **software environment** running on the hardware.

---

## 3. WHAT THE APPLIANCE IS NOT
The appliance is **not**:

- the entire computer  
- the user’s personal OS  
- the user’s personal files  
- the user’s personal applications  
- the user’s personal accounts  
- the user’s personal data  
- the user’s personal environment  

The appliance is a **contained system** with its own rules, boundaries, and warranty.

---

## 4. WARRANTY BOUNDARY
The warranty applies to:

- the appliance  
- the Golden Master image  
- the curriculum pipeline  
- the RCA system  
- the lockdown system  
- the operator‑grade assembly  
- the deterministic environment  

The warranty does **not** apply to:

- user‑installed software  
- user‑modified OS  
- user‑modified filesystem  
- external accounts  
- drift  
- tampering  
- wiping the appliance  
- replacing the appliance with another OS  

If the user modifies the general‑purpose computer outside the appliance, the appliance warranty is void.

---

## 5. SUPPORT BOUNDARY
Support covers:

- appliance defects  
- curriculum defects  
- RCA defects  
- lockdown defects  
- Golden Master defects  
- operator‑grade assembly defects  

Support does **not** cover:

- Ubuntu issues outside the appliance  
- Windows issues outside the appliance  
- user‑installed packages  
- malware  
- filesystem corruption  
- external accounts  
- unauthorized modifications  

Support is for the appliance, not the entire computer.

---

## 6. USER FREEDOM
The user may:

- exit the appliance  
- use the computer normally  
- install any software  
- browse the web  
- use external accounts  
- develop software  
- play games  
- run VMs  
- do anything they want  

Their freedom is unrestricted **outside** the appliance.

Inside the appliance, the doctrine applies.

---

## 7. APPLIANCE INTEGRITY RULE
The appliance must remain:

- deterministic  
- reproducible  
- auditable  
- lockdown‑consistent  
- RCA‑consistent  
- Golden‑Master‑consistent  

If the user breaks appliance integrity, the warranty is void.

---

## 8. NO DRIFT RULE
The appliance boundary must remain consistent across:

- dlang-appliance  
- dlang-school  
- from-dead-box-to-dev-box  

If one changes, all must change.

---

## 9. REPOSITORY PRIVACY AND OWNERSHIP RULE
dlang-appliance is private, not for sale, and must remain under the sole control of Brother Bill to preserve its integrity and moral purpose.

---

## 10. HUMAN OVERRIDE RULE
If a conflict arises between:

- APPLIANCE_BOUNDARY.md  
- WARRANTY_POLICY.md  
- RESTORE_POLICY.md  
- BACKUP_POLICY.md  
- RCA.md  
- LOCKDOWN_LEVELS.md  
- HARDWARE_REQUIREMENTS.md  
- MISSION2.md  
- MY_RULES.md  
- chat instructions  

MY_RULES.md wins, unless the human operator (Brother Bill) explicitly overrides it.

---

End of file.
