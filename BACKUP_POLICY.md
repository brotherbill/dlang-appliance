# BACKUP_POLICY.md
###### /dev/repos/dlang-appliance/BACKUP_POLICY.md

# Backup Policy for the D Learning Appliance  
# Deterministic. Predictable. Parent‑Grade. Operator‑Grade. Institutional‑Grade.

This file defines the official backup policy for all D Learning Appliances.  
It governs frequency, retention, encryption, verification, and failure handling across all lockdown levels.

A man’s got to know his limitations.  
This file defines the appliance’s.

---

## 1. PURPOSE OF THE BACKUP POLICY
The backup policy ensures:

- curriculum continuity  
- workspace preservation  
- RCA integrity  
- deterministic restore operations  
- parent‑grade safety  
- operator‑grade auditability  
- institutional‑grade immutability  

Backups must be predictable, testable, and reproducible.

---

## 2. BACKUP TYPES
The appliance supports three categories of backups:

### 2.1 Daily Backups
Performed automatically once per day.

Includes:
- curriculum state  
- student workspace  
- RCA metadata  
- configuration snapshot  

### 2.2 Event‑Driven Backups
Triggered automatically before:

- system updates  
- lockdown level changes  
- restore operations  
- refurb intake  
- RCA wipe  

### 2.3 Manual Backups
Allowed only for:

- Level 1 (Parent‑Grade)  
- Level 2 (Operator‑Grade)  

Forbidden for Level 3 (Institutional).

---

## 3. BACKUP FREQUENCY
### Level 1 — Parent‑Grade
- Daily backup  
- Event‑driven backups  
- Optional manual backup  

### Level 2 — Operator‑Grade
- Daily backup  
- Event‑driven backups  
- Manual backup allowed only by operator  

### Level 3 — Institutional
- Daily backup  
- Event‑driven backups  
- No manual backups  
- No cloud sync  

---

## 4. BACKUP RETENTION
Retention periods are:

- **30 days** for Level 1  
- **60 days** for Level 2  
- **90 days** for Level 3  

Older backups are pruned automatically.

---

## 5. BACKUP STORAGE LOCATIONS
### Level 1
- local encrypted storage  
- optional cloud sync  

### Level 2
- local encrypted storage only  
- no cloud sync  

### Level 3
- local encrypted storage only  
- air‑gapped  
- no network interfaces active  

---

## 6. ENCRYPTION REQUIREMENTS
All backups must be:

- encrypted at rest  
- encrypted in transit (Level 1 cloud sync only)  
- signed with RCA verification hash  
- tamper‑evident  

Level 3 backups must be immutable.

---

## 7. BACKUP VERIFICATION
Every backup must pass:

- integrity check  
- hash verification  
- RCA heartbeat confirmation  
- lockdown state confirmation  

If verification fails, the backup is discarded and re‑attempted.

---

## 8. FAILURE HANDLING
If a backup fails:

1. RCA logs the failure  
2. System retries once  
3. If retry fails, operator alert is generated  
4. Level 3 devices require physical operator intervention  

No silent failures.

---

## 9. RESTORE POINT CREATION RULES
A restore point must be created:

- before updates  
- before lockdown changes  
- before RCA wipe  
- before refurb intake  
- before full restore operations  

Restore points must be:

- encrypted  
- signed  
- verified  
- immutable (Level 3)  

---

## 10. PARENT‑GRADE VS OPERATOR‑GRADE BEHAVIOR
### Parent‑Grade (Level 1)
- parents may trigger manual backups  
- parents may restore curriculum/workspace  
- parents may not access RCA internals  

### Operator‑Grade (Level 2)
- operators may trigger manual backups  
- operators may restore any subsystem  
- RCA logs all operator actions  

### Institutional (Level 3)
- no manual backups  
- no manual restores  
- operator must be physically present  

---

## 11. REFURB PIPELINE INTEGRATION
During refurb:

1. Final backup created  
2. RCA wipe performed  
3. Hardware diagnostics logged  
4. Golden Master re‑clone  
5. RCA re‑bind  
6. Backup schedule re‑initialized  

No device re‑enters circulation without a clean backup baseline.

---

## 12. NO DRIFT RULE
Backup policy must remain consistent across:

- dlang-appliance  
- dlang-school  
- from-dead-box-to-dev-box  

If one changes, all must change.

---

## 13. REPOSITORY PRIVACY AND OWNERSHIP RULE
dlang-appliance is private, not for sale, and must remain under the sole control of Brother Bill to preserve its integrity and moral purpose.

---

## 14. HUMAN OVERRIDE RULE
If a conflict arises between:

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
