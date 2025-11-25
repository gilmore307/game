# change — Cross-File Diff Note (named parent paths only)

**Generated:** 2025-09-17 19:46:24 JST

## 1) Scope
**Artifacts used:**
- base11.zip (SHA1: `fc7b078d121b66388f06127633c4f79b43d7f5fa`)
- mod11.zip  (SHA1: `1a7e02c14bda815f209fe7593a195f3fcb7e89c6`)

**Files compared (base → mod):**
- 00_army_model.txt — **needs change**
- 00_economic_system.txt — **needs change**
- 00_internal_security.txt — **needs change**
- 00_policing.txt — **needs change**

## 2) Global Summary
- Added blocks: **0**
- Removed blocks: **0**
- Moved within same file (content identical): **0**
- Moved across files (content identical): **0**
- Modified blocks (content changed, no move): **8**
- Moved+Modified within same file: **2**
- Moved+Modified across files: **0**
- Unchanged blocks: **17**

## 3) Block Order by File (Base → Mod)
### 00_army_model.txt
**Base order:**
1. `modifier#1`
2. `can_impose#1`
3. `on_enact#1`
4. `ai_will_do#1`
5. `ai_enact_weight_modifier#1`
6. `law_professional_army#1`
7. `law_national_militia#1`
8. `law_mass_conscription#1`

**Mod order:**
1. `modifier#1`
2. `can_impose#1`
3. `on_enact#1`
4. `ai_will_do#1`
5. `ai_enact_weight_modifier#1`
6. `law_professional_army#1`
7. `law_national_militia#1`
8. `law_mass_conscription#1`

### 00_economic_system.txt
**Base order:**
1. `law_traditionalism#1`
2. `law_interventionism#1`
3. `law_agrarianism#1`
4. `law_industry_banned#1`
5. `law_extraction_economy#1`
6. `law_laissez_faire#1`
7. `law_cooperative_ownership#1`
8. `law_command_economy#1`

**Mod order:**
1. `law_traditionalism#1`
2. `law_interventionism#1`
3. `law_agrarianism#1`
4. `law_industry_banned#1`
5. `law_extraction_economy#1`
6. `law_laissez_faire#1`
7. `law_cooperative_ownership#1`
8. `law_command_economy#1`

### 00_internal_security.txt
**Base order:**
1. `ai_will_do#1`
2. `ai_enact_weight_modifier#1`
3. `law_national_guard#1`
4. `law_secret_police#1`
5. `law_guaranteed_liberties#1`

**Mod order:**
1. `ai_will_do#1`
2. `ai_enact_weight_modifier#1`
3. `law_secret_police#1`
4. `law_national_guard#1`
5. `law_guaranteed_liberties#1`

### 00_policing.txt
**Base order:**
1. `can_enact#1`
2. `ai_will_do#1`
3. `ai_enact_weight_modifier#1`
4. `law_local_police#1`
5. `law_dedicated_police#1`
6. `law_militarized_police#1`

**Mod order:**
1. `can_enact#1`
2. `ai_will_do#1`
3. `ai_enact_weight_modifier#1`
4. `law_local_police#1`
5. `law_dedicated_police#1`
6. `law_militarized_police#1`

## 4) Modified — detailed diffs (named parent paths, adaptive context)
### File: **00_army_model.txt** — Block: `modifier#1` (base L7-L16)
#### Path: modifier
_Tags: numeric-change_
```diff
  [L13] 		country_military_goods_cost_mult = -0.1
  [L14] 		state_building_barracks_max_level_add = 25
- [L15] 		state_building_conscription_center_max_level_add = 25
  ↑ inserted after base L14
+ [M15] 		state_building_conscription_center_max_level_add = 5
  [L16] 	}
```

### File: **00_army_model.txt** — Block: `law_professional_army#1` (base L65-L150)
#### Path: law_professional_army > modifier
_Tags: numeric-change_
```diff
  [L77] 		country_soldiers_pol_str_mult = 0.50
  [L78] 		state_building_barracks_max_level_add = 100
- [L79] 		state_building_conscription_center_max_level_add = 50
  ↑ inserted after base L78
+ [M79] 		state_building_conscription_center_max_level_add = 10
  [L80] 		unit_experience_gain_mult = 1.0
  [L81] 	}
```

### File: **00_army_model.txt** — Block: `law_national_militia#1` (base L152-L210)
#### Path: law_national_militia > modifier
_Tags: numeric-change_
```diff
  [L165] 		country_leverage_resistance_mult = 0.5
  [L166] 		state_building_barracks_max_level_add = 5
- [L167] 		state_building_conscription_center_max_level_add = 100
  ↑ inserted after base L166
+ [M167] 		state_building_conscription_center_max_level_add = 20
  [L168] 	}
  [L169] 	
```

### File: **00_army_model.txt** — Block: `law_mass_conscription#1` (base L212-L298)
#### Path: law_mass_conscription > modifier
_Tags: numeric-change_
```diff
  [L225] 		country_soldiers_pol_str_mult = 1
  [L226] 		state_building_barracks_max_level_add = 100
- [L227] 		state_building_conscription_center_max_level_add = 100
  ↑ inserted after base L226
+ [M227] 		state_building_conscription_center_max_level_add = 20
  [L228] 	}
  [L229] 
```

### File: **00_economic_system.txt** — Block: `law_industry_banned#1` (base L205-L304)
#### Path: law_industry_banned
_Tags: parameter-tweak_
```diff
  [L263] 					limit = {
  [L264] 						has_building = building_munition_plants
  [L265] 					}
- [L266] 					remove_building = building_munition_plants
  ↑ inserted after base L265
+ [M266] 					remove_building = building_arms_industry
  [L267] 				}
  [L268] 			}
  [L269] 		}
```
#### Path: law_industry_banned > limit
_Tags: parameter-tweak_
```diff
  [L261] 				}
  [L262] 				if = {
  [L263] 					limit = {
- [L264] 						has_building = building_munition_plants
  ↑ inserted after base L263
+ [M264] 						has_building = building_arms_industry
  [L265] 					}
  [L266] 					remove_building = building_munition_plants
  [L267] 				}
```

### File: **00_economic_system.txt** — Block: `law_extraction_economy#1` (base L306-L406)
#### Path: law_extraction_economy
_Tags: parameter-tweak_
```diff
  [L370] 					limit = {
  [L371] 						has_building = building_munition_plants
  [L372] 					}
- [L373] 					remove_building = building_munition_plants
  ↑ inserted after base L372
+ [M373] 					remove_building = building_arms_industry
  [L374] 				}
  [L375] 			}
  [L376] 		}
```
#### Path: law_extraction_economy > limit
_Tags: parameter-tweak_
```diff
  [L368] 				}
  [L369] 				if = {
  [L370] 					limit = {
- [L371] 						has_building = building_munition_plants
  ↑ inserted after base L370
+ [M371] 						has_building = building_arms_industry
  [L372] 					}
  [L373] 					remove_building = building_munition_plants
  [L374] 				}
```

### File: **00_internal_security.txt** — Block: `law_national_guard#1` (base L22-L63)
#### Path: law_national_guard > institution_modifier
_Tags: list-edit | logic-edit | misc-change_
```diff
  [L36] 
  [L37] 	institution = institution_home_affairs
  [L38] 	institution_modifier = {
- [L39] 		state_conscription_rate_add = 0.005
  ↑ inserted after base L38
+ [M76] 		country_revolution_progress_mult = -0.1
+ [M77] 		country_secession_progress_mult = -0.1
  [L40] 		political_movement_radicalism_add = -0.05
  [L41] 		state_harvest_condition_flood_impact_mult = -0.05
  [L42] 		state_harvest_condition_wildfire_impact_mult = -0.05
```
```diff
  [L38] 	institution_modifier = {
  [L39] 		state_conscription_rate_add = 0.005
  [L40] 		political_movement_radicalism_add = -0.05
- [L41] 		state_harvest_condition_flood_impact_mult = -0.05
- [L42] 		state_harvest_condition_wildfire_impact_mult = -0.05
- [L43] 		state_harvest_condition_extreme_winds_impact_mult = -0.05
- [L44] 		state_harvest_condition_drought_impact_mult= -0.05
- [L45] 	}
- [L46] 
- [L47] 	# Don't return to national guard we have something more advanced
- [L48] 	ai_will_do = {
- [L49] 		NOR = {
- [L50] 			has_law = law_type:law_secret_police
- [L51] 			has_law = law_type:law_guaranteed_liberties
- [L52] 		}
  [L53] 	}
  [L54] 
  [L55] 	ai_enact_weight_modifier = { #Petitions
```
#### Path: law_national_guard > modifier
_Tags: misc-change_
```diff
  [L30] 	}
  [L31] 
  [L32] 	modifier = {
  ↑ inserted after base L32
+ [M67] 		country_institution_home_affairs_max_investment_add = 2
+ [M68] 		state_building_conscription_center_max_level_add = 5
+ [M69] 		state_conscription_rate_add = 0.02
  [L33] 		country_officers_pol_str_mult = 0.5
  [L34] 		country_soldiers_pol_str_mult = 0.25
  [L35] 	}
```

### File: **00_internal_security.txt** — Block: `law_secret_police#1` (base L65-L98)
#### Path: law_secret_police > modifier
_Tags: misc-change_
```diff
  [L74] 
  [L75] 	modifier = {
- [L76] 		country_institution_home_affairs_max_investment_add = 2
  [L77] 		country_officers_pol_str_mult = 0.25
  [L78] 	}
```

### File: **00_internal_security.txt** — Block: `law_guaranteed_liberties#1` (base L100-L129)
#### Path: law_guaranteed_liberties > institution_modifier
_Tags: misc-change_
```diff
  [L117] 		state_radicals_from_political_movements_mult = -0.05
  [L118] 		state_loyalists_from_political_movements_mult = 0.05
  ↑ inserted after base L118
+ [M110] 		state_harvest_condition_flood_impact_mult = -0.05
+ [M111] 		state_harvest_condition_wildfire_impact_mult = -0.05
+ [M112] 		state_harvest_condition_extreme_winds_impact_mult = -0.05
+ [M113] 		state_harvest_condition_drought_impact_mult= -0.05
  [L119] 	}
  [L120] 	
```

### File: **00_policing.txt** — Block: `law_militarized_police#1` (base L209-L299)
#### Path: law_militarized_police > modifier
_Tags: misc-change_
```diff
  [L220] 	modifier = {
  [L221] 		country_institution_police_max_investment_add = 2
  ↑ inserted after base L221
+ [M222] 		state_building_conscription_center_max_level_add = 5
+ [M223] 		state_conscription_rate_add = 0.02
  [L222] 	}
  [L223] 
```
