# change — Cross-File Diff Note (named parent paths only)

**Generated:** 2025-09-17 19:28:37 JST

## 1) Scope
**Artifacts used:**
- base10.zip (SHA1: `6893101b7a7b85ab7b2a7fa874a30dde0ccf0c89`)
- mod10.zip  (SHA1: `ce79107c6d7a4a1a2baec7f43eda873bb738c155`)

**Files compared (base → mod):**
- 00_establish_colonial_administration.txt — **needs change**
- 00_technology_production.txt — **needs change**
- 00_war_crimes.txt — **needs change**
- 02_russia.txt — **needs change**

## 2) Global Summary
- Added blocks: **0**
- Removed blocks: **0**
- Moved within same file (content identical): **0**
- Moved across files (content identical): **0**
- Modified blocks (content changed, no move): **4**
- Moved+Modified within same file: **0**
- Moved+Modified across files: **0**
- Unchanged blocks: **37**

## 3) Block Order by File (Base → Mod)
### 00_establish_colonial_administration.txt
**Base order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `immediate#1`

**Mod order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `immediate#1`

### 00_technology_production.txt
**Base order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `complete#1`
4. `on_complete#1`
5. `je_mechanized_farming#1`
6. `je_atmospheric_engine#1`
7. `je_plastics#1`
8. `je_radio#1`
9. `je_dynamite#1`
10. `je_combustion_engines#1`
11. `je_railroads#1`
12. `je_telephone#1`
13. `je_whaling#1`
14. `je_pumpjacks#1`
15. `je_electrical_generation#1`
16. `je_steam_engines#1`

**Mod order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `complete#1`
4. `on_complete#1`
5. `je_mechanized_farming#1`
6. `je_atmospheric_engine#1`
7. `je_plastics#1`
8. `je_radio#1`
9. `je_dynamite#1`
10. `je_combustion_engines#1`
11. `je_railroads#1`
12. `je_telephone#1`
13. `je_whaling#1`
14. `je_pumpjacks#1`
15. `je_electrical_generation#1`
16. `je_steam_engines#1`

### 00_war_crimes.txt
**Base order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `complete#1`
4. `on_complete#1`
5. `je_munitions_factories#1`

**Mod order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `complete#1`
4. `on_complete#1`
5. `je_munitions_factories#1`

### 02_russia.txt
**Base order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `immediate#1`
4. `complete#1`
5. `on_complete#1`
6. `invalid#1`
7. `je_caucasian_war#1`
8. `je_circassian_expulsions#1`
9. `je_caucasian_war_circassia#1`
10. `je_caucasian_war_imamate#1`
11. `je_pacify_the_steppes#1`
12. `je_the_last_kazakh_khan#1`
13. `je_conquest_of_central_asia#1`
14. `je_great_reformer#1`
15. `je_great_reforms_serfdom#1`
16. `je_great_reforms_military#1`
17. `je_great_reforms_bureaucratic#1`

**Mod order:**
1. `is_shown_when_inactive#1`
2. `possible#1`
3. `immediate#1`
4. `complete#1`
5. `on_complete#1`
6. `invalid#1`
7. `je_caucasian_war#1`
8. `je_circassian_expulsions#1`
9. `je_caucasian_war_circassia#1`
10. `je_caucasian_war_imamate#1`
11. `je_pacify_the_steppes#1`
12. `je_the_last_kazakh_khan#1`
13. `je_conquest_of_central_asia#1`
14. `je_great_reformer#1`
15. `je_great_reforms_serfdom#1`
16. `je_great_reforms_military#1`
17. `je_great_reforms_bureaucratic#1`

## 4) Modified — detailed diffs (named parent paths, adaptive context)
### File: **00_establish_colonial_administration.txt** — Block: `possible#1` (base L19-L25)
#### Path: possible > institution_investment_level
_Tags: logic-edit_
```diff
  [L23] 		}
  [L24] 		has_technology_researched = civilizing_mission
  ↑ inserted after base L24
+ [M25] 		institution_investment_level = {
+ [M26] 			institution = institution_colonial_affairs
+ [M27] 			value >= 3
+ [M28] 		}
  [L25] 	}
```

### File: **00_technology_production.txt** — Block: `je_dynamite#1` (base L247-L337)
#### Path: je_dynamite > complete > OR > any_scope_building > filter
_Tags: parameter-tweak_
```diff
  [L276] 			any_scope_building = {
  [L277] 				custom_tooltip = je_shortform_building_munition_plants_tooltip
  [L278] 				filter = {
- [L279] 					is_building_type = building_munition_plants
  ↑ inserted after base L278
+ [M279] 					is_building_type = building_arms_industry
  [L280] 				}
  [L281] 				percent > 0.75
  [L282] 				cash_reserves_ratio >= 0.25
```
#### Path: je_dynamite > possible > any_scope_building > OR
_Tags: parameter-tweak_
```diff
  [L259] 		has_technology_researched = dynamite
  [L260] 		any_scope_building = {
  [L261] 			OR = {
- [L262] 				is_building_type = building_munition_plants
  ↑ inserted after base L261
+ [M262] 				is_building_type = building_arms_industry
  [L263] 				is_building_type = building_iron_mine
  [L264] 				is_building_type = building_coal_mine
  [L265] 				is_building_type = building_lead_mine
```

### File: **00_war_crimes.txt** — Block: `je_munitions_factories#1` (base L44-L81)
#### Path: je_munitions_factories > complete > any_scope_building
_Tags: parameter-tweak_
```diff
  [L60] 
  [L61] 	complete = {
  [L62] 		any_scope_building = {
- [L63] 			is_building_type = building_munition_plants
  ↑ inserted after base L62
+ [M63] 			is_building_type = building_arms_industry
  [L64] 			cash_reserves_ratio > 0.25
  [L65] 			weekly_profit > 0
  [L66] 			occupancy >= 0.5
```
#### Path: je_munitions_factories > possible > any_scope_building
_Tags: parameter-tweak_
```diff
  [L54] 	possible = {
  [L55] 		has_technology_researched = percussion_cap
  [L56] 		any_scope_building = {
- [L57] 			is_building_type = building_munition_plants
  ↑ inserted after base L56
+ [M57] 			is_building_type = building_arms_industry
  [L58] 		}
  [L59] 	}
  [L60] 
```

### File: **02_russia.txt** — Block: `je_great_reforms_military#1` (base L1073-L1156)
#### Path: je_great_reforms_military > complete > any_scope_building
_Tags: parameter-tweak_
```diff
  [L1128] 		}
  [L1129]         any_scope_building = {
- [L1130]             is_building_type = building_munition_plants
  ↑ inserted after base L1129
+ [M1130]             is_building_type = building_arms_industry
  [L1131]             level >= 3
  [L1132]         }
```
