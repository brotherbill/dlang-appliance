# RESTORE_POLICY.md
###### /dev/repos/dlang-appliance/RESTORE_POLICY.md

# Restore Policy for the D Learning Appliance  
# Deterministic. Safe. Parent‑Grade. Operator‑Grade. Institutional‑Grade.

This file defines the official restore policy for all D Learning Appliances.  
It governs what can be restored, who may restore it, when restore points are created, and how restore operations are verified.

A man’s got to know his limitations.  
This file defines the appliance’s.

---

## 1. PURPOSE OF THE RESTORE POLICY
The restore policy ensures:

- curriculum continuity  
- workspace recovery  
- RCA integrity  
- safe rollback of system changes  
- predictable behavior across lockdown levels  
- parent‑grade safety  
- operator‑grade authority  
- institutional‑grade immutability  

Restore operations must be deterministic, auditable, and safe.

---

## 2. RESTORE TYPES
The appliance supports five restore types:

### 2.1 Curriculum Restore
Restores curriculum state only.  
Safe for parents and students.

### 2.2 Workspace Restore
Restores the student’s workspace.  
Safe for parents and students.

### 2.3 Full Appliance Restore
Restores the entire appliance to a previous known‑good state.  
Operator‑only.

### 2.4 Pre‑Update Restore
Rollback point created before system updates.

### 2.5 Pre‑Lockdown‑Change Restore
Rollback point created before lockdown level changes.

---

## 3. RESTORE PERMISSIONS BY LOCKDOWN LEVEL
### Level 1 — Parent‑Grade
Allowed:
- curriculum restore  
- workspace restore  

Forbidden:
- full appliance restore  
- RCA restore  
- lockdown restore  

### Level 2 — Operator‑Grade
Allowed:
- curriculum restore  
- workspace restore  
- full appliance restore  
- pre‑update restore  
- pre‑lockdown‑change restore  

Forbidden:
- RCA restore without operator authentication  

### Level 3 — Institutional
Allowed:
- curriculum restore  
- workspace restore  

Forbidden:
- all manual restores  
- all operator‑remote restores  
- all full appliance restores  
- all network‑based restores  

Level 3 restores require **physical operator presence**.

---

## 4. RESTORE SAFETY RULES
All restore operations must:

- verify backup integrity  
- verify RCA heartbeat  
- verify lockdown level  
- verify hardware profile  
- verify tamper‑evident seals (Level 3)  
- log the restore event  
- generate a new restore point before applying changes  

No destructive restore may occur without operator approval.

---

## 5. RESTORE POINT CREATION
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

## 6. RESTORE VERIFICATION
After a restore, the appliance must:

1. verify RCA heartbeat  
2. verify lockdown state  
3. verify hardware profile  
4. verify curriculum integrity  
5. verify workspace integrity  
6. log the restore event  
7. generate a post‑restore snapshot  

No restore is considered complete until verification passes.

---

## 7. FAILURE HANDLING
If a restore fails:

1. RCA logs the failure  
2. System attempts rollback to previous restore point  
3. If rollback fails, operator alert is generated  
4. Level 3 devices require physical operator intervention  

No silent failures.

---

## 8. REFURB PIPELINE INTEGRATION
During refurb:

- a final restore point is created  
- RCA wipe is performed  
- Golden Master is re‑cloned  
- RCA is re‑bound  
- restore schedule is re‑initialized  

No device re‑enters circulation without a clean restore baseline.

---

## 9. NO DRIFT RULE
Restore policy must remain consistent across:

- dlang-appliance  
- dlang-school  
- from-dead-box-to-dev-box  

If one changes, all must change.

---

## 10. REPOSITORY PRIVACY AND OWNERSHIP RULE
dlang-appliance is private, not for sale, and must remain under the sole control of Brother Bill to preserve its integrity and moral purpose.

---

## 11. HUMAN OVERRIDE RULE
If a conflict arises between:

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
