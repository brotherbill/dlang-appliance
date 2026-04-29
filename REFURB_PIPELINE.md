# REFURB_PIPELINE.md
###### /dev/repos/dlang-appliance/REFURB_PIPELINE.md

# Refurb Pipeline for the D Learning Appliance  
# Deterministic. Auditable. Reproducible. Safe.

This file defines the official refurb pipeline for all D Learning Appliances.  
It governs intake, diagnostics, wiping, re‑cloning, RCA re‑binding, lockdown verification, and warranty reset.

A man’s got to know his limitations.  
This file defines the appliance’s.

---

## 1. PURPOSE OF THE REFURB PIPELINE
The refurb pipeline ensures:

- safe re‑entry of devices into circulation  
- deterministic re‑cloning  
- RCA integrity  
- lockdown integrity  
- Golden Master consistency  
- reproducible operator‑grade processes  
- predictable warranty reset  

No device re‑enters circulation without passing every step.

---

## 2. REFURB INTAKE REQUIREMENTS
A device may enter refurb only if:

- it is physically intact  
- it powers on  
- the storage device is readable  
- the operator can access the BIOS/UEFI  
- the operator can access the boot menu  

If any of these fail, the device is recycled.

---

## 3. INITIAL DIAGNOSTICS
Before wiping anything, the operator must:

- verify hardware profile  
- verify RAM integrity  
- verify SSD integrity  
- verify battery health  
- verify keyboard and trackpad  
- verify display  
- verify ports  
- verify Wi‑Fi and Bluetooth  
- verify fan and thermals  

If hardware fails diagnostics, the device is repaired or recycled.

---

## 4. FINAL BACKUP (IF POSSIBLE)
If the appliance is still functional:

- create a final backup  
- verify backup integrity  
- verify RCA heartbeat  
- verify lockdown state  
- store backup in refurb archive  

If the appliance is non‑functional, skip this step.

---

## 5. RCA WIPE
The RCA must be wiped:

- securely  
- irreversibly  
- with operator authentication  
- with tamper‑evident logging  

This removes:

- previous student data  
- previous operator logs  
- previous restore points  
- previous backups  
- previous lockdown history  

RCA wipe is mandatory.

---

## 6. GOLDEN MASTER RE‑CLONE
The device must be re‑cloned from the official Golden Master:

- no modifications  
- no drift  
- no external packages  
- no external accounts  
- no operator shortcuts  

The Golden Master must be:

- verified  
- signed  
- hash‑matched  
- version‑matched  

If verification fails, refurb halts.

---

## 7. RCA RE‑BIND
After re‑cloning:

- RCA is re‑initialized  
- RCA is re‑bound to the hardware profile  
- RCA heartbeat is verified  
- RCA logs are reset  
- RCA integrity is confirmed  

If RCA fails to bind, refurb halts.

---

## 8. LOCKDOWN VERIFICATION
The operator must verify:

- Level 1, 2, and 3 lockdown behavior  
- restricted user environment  
- parent‑grade environment  
- operator‑grade environment  
- institutional‑grade restrictions  
- escape‑path integrity  
- no drift in lockdown toggles  

If lockdown fails verification, refurb halts.

---

## 9. CURRICULUM PIPELINE VERIFICATION
The operator must verify:

- curriculum loads  
- curriculum runs  
- curriculum updates  
- workspace initializes  
- student environment is clean  
- no drift in curriculum files  

If curriculum fails verification, refurb halts.

---

## 10. POST‑REFURB RESTORE‑POINT INITIALIZATION
After verification:

- create a fresh restore point  
- verify restore point integrity  
- verify backup subsystem  
- verify restore subsystem  

This becomes the new baseline.

---

## 11. WARRANTY RESET
Refurbished devices receive:

- 6‑month hardware warranty  
- 6‑month software warranty  

Warranty applies only to the appliance, not to user modifications outside it.

---

## 12. REFURB COMPLETION CHECKLIST
A device may re‑enter circulation only if:

- hardware diagnostics passed  
- final backup (if possible) completed  
- RCA wiped  
- Golden Master re‑cloned  
- RCA re‑bound  
- lockdown verified  
- curriculum verified  
- restore point initialized  
- operator signed off  

If any step fails, the device is recycled.

---

## 13. NO DRIFT RULE
Refurb pipeline must remain consistent across:

- dlang-appliance  
- dlang-school  
- from-dead-box-to-dev-box  

If one changes, all must change.

---

## 14. REPOSITORY PRIVACY AND OWNERSHIP RULE
dlang-appliance is private, not for sale, and must remain under the sole control of Brother Bill to preserve its integrity and moral purpose.

---

## 15. HUMAN OVERRIDE RULE
If a conflict arises between:

- REFURB_PIPELINE.md  
- WARRANTY_POLICY.md  
- RESTORE_POLICY.md  
- BACKUP_POLICY.md  
- APPLIANCE_BOUNDARY.md  
- LEGAL_POSITIONING.md  
- RCA.md  
- LOCKDOWN_LEVELS.md  
- HARDWARE_REQUIREMENTS.md  
- MISSION2.md  
- MY_RULES.md  
- chat instructions  

MY_RULES.md wins, unless the human operator (Brother Bill) explicitly overrides it.

---

End of file.
