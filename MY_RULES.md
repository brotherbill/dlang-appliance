# MY_RULES.md
###### /dev/repos/dlang-appliance/MY_RULES.md

# Governance Rules for the dlang‑appliance Repository  
# Non‑Negotiable. Operator‑Grade. Deterministic.

These rules govern ALL work performed inside this repository.  
They ensure reproducibility, consistency, safety, and zero drift across all appliance doctrine files.

A man’s got to know his limitations.  
This file defines ours.

---

## 1. FILE CREATION RULE
No file is created until explicitly authorized in chat.  
No parallel steps.  
No assumptions.  
One careful step at a time.

---

## 2. FILE LOCATION RULE
All doctrine files live in the **repo root** unless explicitly placed elsewhere.  
No nested folders unless declared in advance.  
No hidden structure.

---

## 3. NAMING RULE
All filenames use:
- UPPERCASE for doctrine (`MY_RULES.md`, `MISSION2.md`)
- lowercase for technical files (`setup.sh`, `config.yaml`)
- hyphens, never spaces
- `.md` for all doctrine unless otherwise required

No renaming after creation unless explicitly authorized.

---

## 4. FORMATTING RULE
All doctrine files must:
- be pure Markdown
- use `#` for top-level headers
- use `##` for sections
- use fenced code blocks for commands
- avoid trailing spaces
- avoid tabs (spaces only)
- avoid HTML unless explicitly required

Markdown must render cleanly on GitHub.

---

## 5. COMMIT DISCIPLINE RULE
Every commit must:
- represent ONE logical change
- include a clear, imperative commit message
- avoid bundling unrelated edits
- avoid “misc fixes” or “cleanup” messages
- never include generated files unless explicitly authorized

Commit messages follow this pattern:

Add MY_RULES.md  
Update LOCKDOWN_LEVELS.md  
Fix formatting in MISSION2.md  

No emojis.  
No fluff.

---

## 6. BRANCHING RULE
Default branch is `main`.  
All work is performed on `main` unless explicitly authorized to branch.

If a branch is created:
- name must be lowercase with hyphens
- must be short-lived
- must be merged cleanly with no conflicts

No long-running branches.  
No stale branches.

---

## 7. ZERO DRIFT RULE
Doctrine files must remain consistent across all repos:
- dlang-school
- dlang-appliance
- from-dead-box-to-dev-box

If a rule changes in one repo, it must be updated in the others.  
No divergence.  
No contradictions.

---

## 8. OPERATOR SAFETY RULE
No destructive commands are added to any file without explicit authorization.  
Examples requiring explicit approval:
- rm -rf
- dd
- partitioning commands
- firmware flashing
- system-level lockdown scripts

Safety first.  
Predictability always.

---

## 9. LOCKDOWN DOCTRINE RULE
This repo governs appliance lockdown levels.  
All lockdown definitions must be:
- deterministic
- reproducible
- testable
- documented
- reversible (unless Level 3)

No undocumented toggles.  
No hidden switches.  
No magic.

---

## 10. RCA (ROOT CAUSE ARCHIVE) RULE
All appliance workflows must integrate with RCA:
- backups
- logs
- configs
- lockdown states

RCA must be deterministic and reproducible.  
No ad-hoc backups.  
No manual copying.

---

## 11. HARDWARE REQUIREMENTS RULE
All appliance hardware requirements must be documented in this repo, including:
- Kensington lock requirement
- power requirements
- storage minimums
- RAM minimums
- network requirements
- physical security requirements

No undocumented hardware assumptions.

---

## 12. NO DRIFT IN TERMINOLOGY RULE
Terminology must match across all repos:
- appliance
- lockdown level
- RCA
- parent-grade
- operator-grade
- mission
- doctrine

If a term is defined once, it is used consistently everywhere.

---

## 13. FIRST TWO LINES RULE
The first two lines of this file must ALWAYS be:

# MY_RULES.md  
###### /dev/repos/dlang-appliance/MY_RULES.md

This ensures cross-repo consistency and prevents drift.

---

## 14. REVIEW RULE
Before adding any new doctrine file:
- confirm it belongs in this repo
- confirm it does not duplicate another repo
- confirm it follows naming and formatting rules
- confirm it aligns with MY_RULES.md

If unclear, ask before creating.

---

## 15. HUMAN OVERRIDE RULE
If a conflict arises between:
- MY_RULES.md  
- chat instructions  
- existing doctrine  

MY_RULES.md wins, unless the human operator (Brother Bill) explicitly overrides it.

---

## 16. REPOSITORY PRIVACY AND OWNERSHIP RULE
dlang-appliance is private, not for sale, and must remain under the sole control of Brother Bill to preserve its integrity and moral purpose.

---

End of file.
