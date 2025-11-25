# change — Cross-File Diff Note (named parent paths only)

**Generated:** 2025-09-17 19:04:56 JST

## 1) Scope
**Artifacts used:**
- base7.zip (SHA1: `67f99324b9e05ff01f953f8cda144d0a56467b3b`)
- mod7.zip  (SHA1: `17e385293a85f59ff391134bac4f0ad50c7fcfee`)

**Files compared (base → mod):**
- 02_obligation_actions.txt — **needs change**

## 2) Global Summary
- Added blocks: **0**
- Removed blocks: **0**
- Moved within same file (content identical): **0**
- Moved across files (content identical): **0**
- Modified blocks (content changed, no move): **2**
- Moved+Modified within same file: **0**
- Moved+Modified across files: **0**
- Unchanged blocks: **13**

## 3) Block Order by File (Base → Mod)
### 02_obligation_actions.txt
**Base order:**
1. `groups#1`
2. `unlocking_technologies#1`
3. `selectable#1`
4. `potential#1`
5. `possible#1`
6. `accept_effect#1`
7. `ai#1`
8. `redeem_obligation#1`

**Mod order:**
1. `groups#1`
2. `unlocking_technologies#1`
3. `selectable#1`
4. `potential#1`
5. `possible#1`
6. `accept_effect#1`
7. `ai#1`
8. `redeem_obligation#1`

## 4) Modified — detailed diffs (named parent paths, adaptive context)
### File: **02_obligation_actions.txt** — Block: `redeem_obligation#1` (base L418-L460)
#### Path: redeem_obligation > accept_effect
_Tags: misc-change_
```diff
  [L443] 		change_relations = { country = scope:target_country value = 30 }
  [L444] 		scope:target_country = { set_owes_obligation_to = { country = root setting = no } }
  ↑ inserted after base L444
+ [M445] 		change_infamy = -5
  [L445] 	}
  [L446] 	
```
