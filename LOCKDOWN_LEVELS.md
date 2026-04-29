# LOCKDOWN_LEVELS.md
###### /dev/repos/dlang-appliance/LOCKDOWN_LEVELS.md

# Lockdown Levels for the D Learning Appliance  
# Deterministic. Testable. Parent‑Grade. Operator‑Grade. Institutional‑Grade.

This file defines the three official lockdown levels for the D Learning Appliance.  
Each level is deterministic, reproducible, testable, and suitable for assembly‑line production.

A man’s got to know his limitations.  
These are the appliance’s.

---

## 1. OVERVIEW
The appliance supports three lockdown levels:

1. Level 1 — Parent‑Grade  
2. Level 2 — Operator‑Grade  
3. Level 3 — Institutional  

Each level defines:

- allowed actions  
- forbidden actions  
- required hardware  
- RCA requirements  
- reversibility  
- verification steps  

No undocumented toggles.  
No hidden switches.  
No drift.

---

## 2. LEVEL 1 — PARENT‑GRADE
### Allowed
- Curriculum access  
- VS Code (restricted extensions)  
- D toolchain  
- RCA backups  
- Parent account with admin rights  
- Student account with restricted rights  
- Controlled updates  

### Forbidden
- Package installs  
- System settings changes  
- Browser drift  
- External accounts  
- USB write access  

### Hardware Requirements
- Kensington lock recommended  
- Stable power  
- No loose peripherals  

### RCA Requirements
- Daily backup  
- Curriculum progress logs  
- Lockdown state logs  

### Reversibility
- Fully reversible by operator  
- Parent‑grade reset allowed  

### Verification
- Parent account functions  
- Student account restricted  
- RCA operational  
- No escape paths  

---

## 3. LEVEL 2 — OPERATOR‑GRADE
### Allowed
- Curriculum access  
- VS Code (no extension installs)  
- D toolchain  
- RCA mandatory  
- Operator account only  

### Forbidden
- All package installs  
- All system settings  
- All browser drift  
- All external accounts  
- All USB access  
- All removable storage  

### Hardware Requirements
- Kensington lock required  
- Cable routing with no slack  
- Fixed anchor point  

### RCA Requirements
- Mandatory logs  
- Mandatory backups  
- Mandatory lockdown verification  

### Reversibility
- Reversible only by operator  
- Parent cannot unlock  

### Verification
- No package managers  
- No removable media  
- No system settings access  
- RCA heartbeat present  

---

## 4. LEVEL 3 — INSTITUTIONAL
### Allowed
- Curriculum access only  
- RCA local‑only mode  
- Operator‑only maintenance  

### Forbidden
- Internet  
- USB  
- Package installs  
- System settings  
- External accounts  
- Removable media  
- Any escape path  
- Any inbound/outbound connections  

### Hardware Requirements
- Kensington lock mandatory  
- Steel‑braided cable  
- Fixed anchor point  
- Tamper‑evident seals  

### RCA Requirements
- Local‑only  
- Immutable logs  
- No cloud sync  

### Reversibility
- Not reversible by parent  
- Not reversible by student  
- Only reversible by operator with physical access  

### Verification
- Air‑gapped  
- No network interfaces active  
- No removable storage  
- RCA local‑only verified  

---

## 5. A‑LA‑CARTE OPTIONS
These toggles may be applied to any level:

- Allow VS Code extensions  
- Allow GitHub access  
- Allow SSH outbound  
- Allow SSH inbound  
- Allow browser  
- Allow specific URLs  
- Allow specific ports  
- Allow specific apps  
- Allow package installs  
- Allow system updates  
- Allow USB read‑only  
- Allow USB write  

All toggles must be documented and justified.

---

## 6. TESTING AND VERIFICATION
Each lockdown level must pass:

- operator verification  
- RCA verification  
- hardware verification  
- escape‑path audit  
- reproducibility test  

No appliance ships without passing all tests.

---

## 7. NO DRIFT RULE
Lockdown definitions must remain consistent across:

- dlang-appliance  
- dlang-school  
- from-dead-box-to-dev-box  

If one changes, all must change.

---

## 8. REPOSITORY PRIVACY AND OWNERSHIP RULE
dlang-appliance is private, not for sale, and must remain under the sole control of Brother Bill to preserve its integrity and moral purpose.

---

## 9. HUMAN OVERRIDE RULE
If a conflict arises between:

- LOCKDOWN_LEVELS.md  
- MISSION2.md  
- HARDWARE_REQUIREMENTS.md  
- RCA.md  
- MY_RULES.md  
- chat instructions  

MY_RULES.md wins, unless the human operator (Brother Bill) explicitly overrides it.

---

End of file.
