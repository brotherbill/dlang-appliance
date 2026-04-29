# RCA.md
###### /dev/repos/dlang-appliance/RCA.md

# RCA — Root Cause Archive  
# Deterministic. Reproducible. Parent‑Grade. Operator‑Grade. Institutional‑Grade.

The Root Cause Archive (RCA) is the appliance’s internal record of truth.  
It stores the logs, backups, restore points, lockdown states, and configuration snapshots required to support, repair, refurbish, and validate the appliance.

A man’s got to know his limitations.  
RCA defines the appliance’s.

---

## 1. PURPOSE OF RCA
RCA exists to provide:

- deterministic support  
- reproducible troubleshooting  
- parent‑grade transparency  
- operator‑grade auditability  
- institutional‑grade immutability  

RCA is the backbone of:

- warranty validation  
- subscription validation  
- lockdown verification  
- refurb pipeline  
- support escalation  
- restore operations  

No appliance ships without RCA.

---

## 2. WHAT RCA STORES
### 2.1 Logs
- curriculum progress logs  
- system event logs  
- lockdown verification logs  
- RCA heartbeat logs  
- hardware diagnostics logs  

### 2.2 Backups
- curriculum state  
- student workspace  
- RCA metadata  
- configuration snapshots  

### 2.3 Restore Points
- pre‑update restore points  
- pre‑lockdown‑change restore points  
- pre‑refurb restore points  

### 2.4 Lockdown State
- current lockdown level  
- applied toggles  
- verification results  

### 2.5 Hardware Profile
- CPU/RAM/storage profile  
- MAC addresses  
- serial numbers  
- Kensington lock verification  

RCA stores **no personal data** beyond the three parent fields.

---

## 3. WHAT RCA NEVER STORES
RCA must never store:

- passwords  
- browser history  
- external account tokens  
- personal documents  
- personal photos  
- personal messages  
- unencrypted sensitive data  

RCA is a support archive, not a surveillance system.

---

## 4. RCA BINDING PROCESS
Every appliance must bind to RCA during assembly:

1. Generate unique RCA ID  
2. Register hardware profile  
3. Register lockdown level  
4. Register parent fields  
5. Initialize logs  
6. Initialize backup schedule  
7. Initialize restore point structure  

No appliance is considered “born” until RCA binding completes.

---

## 5. BACKUP MODEL
### 5.1 Daily Backups
- curriculum state  
- student workspace  
- RCA metadata  

### 5.2 Event‑Driven Backups
- before updates  
- before lockdown changes  
- before restore operations  

### 5.3 Backup Retention
- 30 days for Level 1  
- 60 days for Level 2  
- 90 days for Level 3  

### 5.4 Backup Storage
- local encrypted storage  
- optional cloud sync (Level 1 only)  
- no cloud sync for Level 2 or Level 3  

---

## 6. RESTORE MODEL
### 6.1 Types of Restore
- curriculum restore  
- workspace restore  
- full appliance restore  
- pre‑update restore  
- pre‑lockdown‑change restore  

### 6.2 Restore Safety
- no destructive restore without operator approval  
- parent‑grade restore limited to curriculum and workspace  
- Level 3 restore requires physical operator presence  

### 6.3 Restore Verification
- logs updated  
- lockdown state re‑verified  
- hardware re‑verified  
- RCA heartbeat confirmed  

---

## 7. LOG STRUCTURE
Logs follow a strict structure:

- timestamp (UTC)  
- subsystem  
- event type  
- event details  
- operator or system origin  
- verification hash  

Logs must be:

- append‑only  
- tamper‑evident  
- reproducible  

Level 3 logs must be immutable.

---

## 8. LOCKDOWN INTEGRATION
### Level 1
- logs parent‑grade actions  
- verifies restricted student account  
- verifies safe defaults  

### Level 2
- logs operator actions  
- verifies no package installs  
- verifies no removable media  
- verifies no system settings access  

### Level 3
- logs all events  
- verifies air‑gap  
- verifies no active interfaces  
- verifies tamper‑evident seals  

RCA is the enforcement backbone for all lockdown levels.

---

## 9. REFURB PIPELINE INTEGRATION
RCA governs refurb:

1. Intake  
2. RCA wipe  
3. Hardware diagnostics  
4. Lockdown reset  
5. Golden Master re‑clone  
6. RCA re‑bind  
7. Verification  
8. Reassignment or recycling  

No device re‑enters circulation without full RCA wipe and re‑bind.

---

## 10. WARRANTY AND SUBSCRIPTION INTEGRATION
RCA validates:

- warranty eligibility  
- subscription status  
- support history  
- hardware authenticity  
- lockdown compliance  

If RCA is missing or corrupted, warranty is void.

---

## 11. NO DRIFT RULE
RCA doctrine must remain consistent across:

- dlang-appliance  
- dlang-school  
- from-dead-box-to-dev-box  

If one changes, all must change.

---

## 12. REPOSITORY PRIVACY AND OWNERSHIP RULE
dlang-appliance is private, not for sale, and must remain under the sole control of Brother Bill to preserve its integrity and moral purpose.

---

## 13. HUMAN OVERRIDE RULE
If a conflict arises between:

- RCA.md  
- HARDWARE_REQUIREMENTS.md  
- LOCKDOWN_LEVELS.md  
- MISSION2.md  
- MY_RULES.md  
- chat instructions  

MY_RULES.md wins, unless the human operator (Brother Bill) explicitly overrides it.

---

End of file.
