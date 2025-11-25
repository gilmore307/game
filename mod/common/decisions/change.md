# change — Cross-File Diff Note (named parent paths only)

**Generated:** 2025-09-17 18:40:35 JST

## 1) Scope
**Artifacts used:**
- base5.zip (SHA1: `28057247c8ad854f400e1e7b68d217a101642cf5`)
- mod5.zip  (SHA1: `d6945e4d5dcf1731b2deebf1d473688a81f9adce`)

**Files compared (base → mod):**
- antarctica_expedition_decision.txt — **needs change**
- central_africa_expedition_decision.txt — **needs change**
- congo_expedition_decision.txt — **needs change**
- niger_river_expedition_decision.txt — **needs change**
- west_america_expidition_decision.txt — **needs change**

## 2) Global Summary
- Added blocks: **0**
- Removed blocks: **0**
- Moved within same file (content identical): **0**
- Moved across files (content identical): **0**
- Modified blocks (content changed, no move): **15**
- Moved+Modified within same file: **0**
- Moved+Modified across files: **0**
- Unchanged blocks: **5**

## 3) Block Order by File (Base → Mod)
### antarctica_expedition_decision.txt
**Base order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

**Mod order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

### central_africa_expedition_decision.txt
**Base order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

**Mod order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

### congo_expedition_decision.txt
**Base order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

**Mod order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

### niger_river_expedition_decision.txt
**Base order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

**Mod order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

### west_america_expidition_decision.txt
**Base order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

**Mod order:**
1. `is_shown#1`
2. `possible#1`
3. `when_taken#1`
4. `ai_chance#1`

## 4) Modified — detailed diffs (named parent paths, adaptive context)
### File: **antarctica_expedition_decision.txt** — Block: `is_shown#1` (base L2-L10)
#### Path: is_shown
_Tags: logic-edit_
```diff
  [L6] 			is_ai = no
  [L7] 			NOT = { has_variable = ai_expedition_cooldown }
  [L8] 		}
- [L9] 		has_technology_researched = sea_lane_strategies
  ↑ inserted after base L8
+ [M9] 		institution_investment_level = {
+ [M10] 			institution = institution_colonial_affairs
+ [M11] 			value >= 3
+ [M12] 		}
  [L10] 	}
```
#### Path: is_shown > NOT
_Tags: logic-edit_
```diff
  [L2] 	is_shown = {
- [L3] 		NOT = { has_global_variable = south_pole_reached }		
- [L4] 		NOT = { has_variable = on_expedition }		
  ↑ inserted after base L2
+ [M3] 		NOT = { has_global_variable = south_pole_reached }	
+ [M4] 		NOT = { has_variable = on_expedition }	
  [L5] 		OR = {
  [L6] 			is_ai = no
  [L7] 			NOT = { has_variable = ai_expedition_cooldown }
```

### File: **antarctica_expedition_decision.txt** — Block: `possible#1` (base L11-L17)
#### Path: possible
_Tags: misc-change_
```diff
  [L11] 	possible = {
  [L12] 		is_at_war = no
  ↑ inserted after base L12
+ [M17] 		has_interest_marker_in_region = region_la_plata
  [L13] 		any_scope_character = {
  [L14] 			has_role = admiral
  [L15] 			count >= 3
```
#### Path: possible > institution_investment_level
_Tags: logic-edit_
```diff
  [L12] 		is_at_war = no
  [L13] 		any_scope_character = {
  [L14] 			has_role = admiral
  [L15] 			count >= 3
  [L16] 		}
  ↑ inserted after base L16
+ [M22] 		institution_investment_level = {
+ [M23] 			institution = institution_colonial_affairs
+ [M24] 			value >= 3
+ [M25] 		}
+ [M26] 		calc_true_if = {
+ [M27] 			amount >= 3
+ [M28] 			owns_entire_state_region = STATE_RIO_NEGRO
+ [M29] 			owns_entire_state_region = STATE_LA_PAMPA
+ [M30] 			owns_entire_state_region = STATE_SANTA_FE
+ [M31] 			owns_entire_state_region = STATE_CORRIENTES
+ [M32] 			owns_entire_state_region = STATE_TUCUMAN
+ [M33] 			owns_entire_state_region = STATE_CHACO
+ [M34] 			owns_entire_state_region = STATE_BUENOS_AIRES
+ [M35] 			owns_entire_state_region = STATE_ALTO_PARAGUAY
+ [M36] 			owns_entire_state_region = STATE_BAJO_PARAGUAY
+ [M37] 			owns_entire_state_region = STATE_SOUTH_ATLANTIC_ISLANDS
+ [M38] 			owns_entire_state_region = STATE_LOS_RIOS
+ [M39] 			owns_entire_state_region = STATE_ARAUCANIA
+ [M40] 			owns_entire_state_region = STATE_PATAGONIA
+ [M41] 			owns_entire_state_region = STATE_SANTIAGO
+ [M42] 		}
  [L17] 	}
```

### File: **antarctica_expedition_decision.txt** — Block: `when_taken#1` (base L18-L37)
#### Path: when_taken
_Tags: logic-edit | parameter-tweak_
```diff
  [L22] 			}
  [L23] 			trigger_event = { id = cold.101 popup = yes }
- [L24] 			set_variable = on_expedition
  ↑ inserted after base L23
+ [M51] 			set_variable = {
+ [M52] 				name = on_expedition
+ [M53] 				value = yes
+ [M54] 			}
  [L25] 		}
  [L26] 		else = {
```

### File: **central_africa_expedition_decision.txt** — Block: `is_shown#1` (base L2-L10)
#### Path: is_shown
_Tags: logic-edit_
```diff
  [L7] 			NOT = { has_variable = ai_expedition_cooldown }
  [L8] 		}		
- [L9] 		has_technology_researched = colonization
  ↑ inserted after base L8
+ [M9] 		institution_investment_level = {
+ [M10] 			institution = institution_colonial_affairs
+ [M11] 			value >= 3
+ [M12] 		}
  [L10] 	}
```

### File: **central_africa_expedition_decision.txt** — Block: `possible#1` (base L12-L23)
#### Path: possible
_Tags: misc-change_
```diff
  [L12] 	possible = {
  [L13] 		is_at_war = no		
  [L14] 		has_interest_marker_in_region = region_zanj
- [L15] 		has_technology_researched = quinine
  [L16] 		any_scope_character = {
  [L17] 			OR = {
  [L18] 				has_role = general
```
#### Path: possible > institution_investment_level
_Tags: logic-edit_
```diff
  [L20] 			}	
  [L21] 			count >= 3
  [L22] 		}
  ↑ inserted after base L22
+ [M25] 		institution_investment_level = {
+ [M26] 			institution = institution_colonial_affairs
+ [M27] 			value >= 3
+ [M28] 		}
+ [M29] 		calc_true_if = {
+ [M30] 			amount >= 1
+ [M31] 			owns_entire_state_region = STATE_ZANZIBAR
+ [M32] 			owns_entire_state_region = STATE_LINDI
+ [M33] 			owns_entire_state_region = STATE_MOCAMBIQUE
+ [M34] 			owns_entire_state_region = STATE_TANGANYIKA
+ [M35] 			owns_entire_state_region = STATE_SOUTH_MADAGASCAR
+ [M36] 			owns_entire_state_region = STATE_NORTH_MADAGASCAR
+ [M37] 			owns_entire_state_region = STATE_INDIAN_OCEAN_TERRITORY
+ [M38] 			owns_entire_state_region = STATE_KAZEMBE
+ [M39] 			owns_entire_state_region = STATE_KENYA
+ [M40] 			owns_entire_state_region = STATE_RIFT_VALLEY
+ [M41] 			owns_entire_state_region = STATE_UGANDA
+ [M42] 		}
  [L23] 	}
```

### File: **central_africa_expedition_decision.txt** — Block: `when_taken#1` (base L25-L44)
#### Path: when_taken
_Tags: logic-edit | parameter-tweak_
```diff
  [L29] 			}
  [L30] 			trigger_event = { id = expedition_events.501 popup = yes }
- [L31] 			set_variable = on_expedition
  ↑ inserted after base L30
+ [M51] 			set_variable = {
+ [M52] 				name = on_expedition
+ [M53] 				value = yes
+ [M54] 			}
  [L32] 		}
  [L33] 		else = {
```

### File: **congo_expedition_decision.txt** — Block: `is_shown#1` (base L2-L10)
#### Path: is_shown > NOT
_Tags: logic-edit_
```diff
  [L2] 	is_shown = {		
- [L3] 		NOT = { has_variable = on_expedition }		
- [L4] 		has_technology_researched = colonization
  [L5] 		NOT = { has_global_variable = congo_river_explored }
  [L6] 		OR = {
  [L7] 			is_ai = no
```
```diff
  [L3] 		NOT = { has_variable = on_expedition }		
  [L4] 		has_technology_researched = colonization
  [L5] 		NOT = { has_global_variable = congo_river_explored }
  ↑ inserted after base L5
+ [M4] 		NOT = { has_variable = on_expedition }
  [L6] 		OR = {
  [L7] 			is_ai = no
  [L8] 			NOT = { has_variable = ai_expedition_cooldown }
```
#### Path: is_shown > OR
_Tags: logic-edit_
```diff
  [L6] 		OR = {
  [L7] 			is_ai = no
  [L8] 			NOT = { has_variable = ai_expedition_cooldown }
- [L9] 		}		
  ↑ inserted after base L8
+ [M8] 		}	
+ [M9] 		institution_investment_level = {
+ [M10] 			institution = institution_colonial_affairs
+ [M11] 			value >= 3
+ [M12] 		}	
  [L10] 	}
```

### File: **congo_expedition_decision.txt** — Block: `possible#1` (base L12-L23)
#### Path: possible
_Tags: logic-edit_
```diff
  [L19] 			}	
  [L20] 			count >= 3
  [L21] 		}
- [L22] 		has_technology_researched = quinine
  ↑ inserted after base L21
+ [M25] 		institution_investment_level = {
+ [M26] 			institution = institution_colonial_affairs
+ [M27] 			value >= 3
+ [M28] 		}
+ [M29] 		calc_true_if = {
+ [M30] 			amount >= 1
+ [M31] 			owns_entire_state_region = STATE_BAS_CONGO
+ [M32] 			owns_entire_state_region = STATE_CONGO
+ [M33] 			owns_entire_state_region = STATE_KASAI
+ [M34] 			owns_entire_state_region = STATE_EQUATEUR
+ [M35] 			owns_entire_state_region = STATE_CONGO_ORIENTALE
+ [M36] 			owns_entire_state_region = STATE_UBANGI_SHARI
+ [M37] 			owns_entire_state_region = STATE_NORTH_ANGOLA
+ [M38] 			owns_entire_state_region = STATE_EAST_ANGOLA
+ [M39] 			owns_entire_state_region = STATE_SOUTH_ANGOLA
+ [M40] 			owns_entire_state_region = STATE_ZAMBIA
+ [M41] 			owns_entire_state_region = STATE_GABON
+ [M42] 			owns_entire_state_region = STATE_SOUTH_CAMEROON
+ [M43] 			owns_entire_state_region = STATE_KATANGA
+ [M44] 		}
  [L23] 	}
```

### File: **congo_expedition_decision.txt** — Block: `when_taken#1` (base L25-L44)
#### Path: when_taken
_Tags: logic-edit | parameter-tweak_
```diff
  [L29] 			}
  [L30] 			trigger_event = { id = expedition_events.601 popup = yes }
- [L31] 			set_variable = on_expedition
  ↑ inserted after base L30
+ [M53] 			set_variable = {
+ [M54] 				name = on_expedition
+ [M55] 				value = yes
+ [M56] 			}
  [L32] 		}
  [L33] 		else = {
```

### File: **niger_river_expedition_decision.txt** — Block: `is_shown#1` (base L2-L10)
#### Path: is_shown > NOT
_Tags: logic-edit_
```diff
  [L2] 	is_shown = {
- [L3] 		NOT = {  has_variable = on_expedition }	
- [L4] 		has_technology_researched = colonization
  [L5] 		NOT = { has_global_variable = niger_river_explored }
  [L6] 		OR = {
  [L7] 			is_ai = no
```
```diff
  [L3] 		NOT = {  has_variable = on_expedition }	
  [L4] 		has_technology_researched = colonization
  [L5] 		NOT = { has_global_variable = niger_river_explored }
  ↑ inserted after base L5
+ [M4] 		NOT = { has_variable = on_expedition }
  [L6] 		OR = {
  [L7] 			is_ai = no
  [L8] 			NOT = { has_variable = ai_expedition_cooldown }
```
#### Path: is_shown > OR
_Tags: logic-edit_
```diff
  [L6] 		OR = {
  [L7] 			is_ai = no
  [L8] 			NOT = { has_variable = ai_expedition_cooldown }
- [L9] 		}		
  ↑ inserted after base L8
+ [M8] 		}	
+ [M9] 		institution_investment_level = {
+ [M10] 			institution = institution_colonial_affairs
+ [M11] 			value >= 3
+ [M12] 		}
  [L10] 	}
```

### File: **niger_river_expedition_decision.txt** — Block: `possible#1` (base L12-L23)
#### Path: possible
_Tags: misc-change_
```diff
  [L12] 	possible = {
  [L13] 		is_at_war = no
  [L14] 		has_interest_marker_in_region = region_niger
- [L15] 		has_technology_researched = quinine
  [L16] 		any_scope_character = {
  [L17] 			OR = {
  [L18] 				has_role = general
```
#### Path: possible > institution_investment_level
_Tags: logic-edit_
```diff
  [L18] 				has_role = general
  [L19] 				has_role = admiral
  [L20] 			}
  [L21] 			count >= 3
  [L22] 		}
  ↑ inserted after base L22
+ [M25] 		institution_investment_level = {
+ [M26] 			institution = institution_colonial_affairs
+ [M27] 			value >= 3
+ [M28] 		}
+ [M29] 		calc_true_if = {
+ [M30] 			amount >= 3
+ [M31] 			owns_entire_state_region = STATE_NIGERIA
+ [M32] 			owns_entire_state_region = STATE_NIGER_DELTA
+ [M33] 			owns_entire_state_region = STATE_YORUBA_STATES
+ [M34] 			owns_entire_state_region = STATE_OUTER_HAUSALAND
+ [M35] 			owns_entire_state_region = STATE_HAUSALAND
+ [M36] 			owns_entire_state_region = STATE_EAST_HAUSALAND
+ [M37] 			owns_entire_state_region = STATE_BORNU
+ [M38] 			owns_entire_state_region = STATE_BENIN
+ [M39] 			owns_entire_state_region = STATE_TOGO
+ [M40] 			owns_entire_state_region = STATE_DAHOMEY
+ [M41] 			owns_entire_state_region = STATE_NIGER
+ [M42] 			owns_entire_state_region = STATE_CHAD
+ [M43] 			owns_entire_state_region = STATE_NORTH_CAMEROON
+ [M44] 			owns_entire_state_region = STATE_WADDAI
+ [M45] 			owns_entire_state_region = STATE_NIGERIA
+ [M46] 		}
  [L23] 	}
```

### File: **niger_river_expedition_decision.txt** — Block: `when_taken#1` (base L25-L44)
#### Path: when_taken
_Tags: logic-edit | parameter-tweak_
```diff
  [L29] 			}
  [L30] 			trigger_event = { id = expedition_events.1 popup = yes }
- [L31] 			set_variable = on_expedition
  ↑ inserted after base L30
+ [M55] 			set_variable = {
+ [M56] 				name = on_expedition
+ [M57] 				value = yes
+ [M58] 			}
  [L32] 		}
  [L33] 		else = {
```

### File: **west_america_expidition_decision.txt** — Block: `is_shown#1` (base L2-L14)
#### Path: is_shown
_Tags: misc-change_
```diff
  [L5] 			has_global_variable = oregon_trail_mapped
  [L6] 			has_global_variable = great_salt_lake_mapped
  [L7] 	    }	
- [L8] 		has_technology_researched = colonization
  [L9] 		NOT = {  has_variable = on_expedition }
  [L10] 		OR = {
  [L11] 			is_ai = no
```
#### Path: is_shown > OR
_Tags: logic-edit_
```diff
  [L10] 		OR = {
  [L11] 			is_ai = no
  [L12] 			NOT = { has_variable = ai_expedition_cooldown }
- [L13] 		}				
  ↑ inserted after base L12
+ [M12] 		}	
+ [M13] 		institution_investment_level = {
+ [M14] 			institution = institution_colonial_affairs
+ [M15] 			value >= 3
+ [M16] 		}	
  [L14] 	}
```

### File: **west_america_expidition_decision.txt** — Block: `possible#1` (base L16-L27)
#### Path: possible
_Tags: misc-change_
```diff
  [L16] 	possible = {
  [L17] 		has_interest_marker_in_region = region_pacific_coast	
  [L18] 		is_at_war = no
- [L19] 		has_technology_researched = quinine
  [L20] 		any_scope_character = {
  [L21] 			OR = {
  [L22] 				has_role = general
```
#### Path: possible > institution_investment_level
_Tags: logic-edit_
```diff
  [L24] 			}
  [L25] 			count >= 3
  [L26] 		}
  ↑ inserted after base L26
+ [M29] 		institution_investment_level = {
+ [M30] 			institution = institution_colonial_affairs
+ [M31] 			value >= 3
+ [M32] 		}
+ [M33] 		calc_true_if = {
+ [M34] 			amount >= 3
+ [M35] 			owns_entire_state_region = STATE_CALIFORNIA
+ [M36] 			owns_entire_state_region = STATE_BAJA_CALIFORNIA
+ [M37] 			owns_entire_state_region = STATE_WASHINGTON
+ [M38] 			owns_entire_state_region = STATE_OREGON
+ [M39] 			owns_entire_state_region = STATE_IDAHO
+ [M40] 			owns_entire_state_region = STATE_NEVADA
+ [M41] 			owns_entire_state_region = STATE_UTAH
+ [M42] 			owns_entire_state_region = STATE_ARIZONA
+ [M43] 			owns_entire_state_region = STATE_ALASKA
+ [M44] 			owns_entire_state_region = STATE_YUKON_TERRITORY
+ [M45] 			owns_entire_state_region = STATE_BRITISH_COLUMBIA
+ [M46] 		}
  [L27] 	}
```

### File: **west_america_expidition_decision.txt** — Block: `when_taken#1` (base L29-L48)
#### Path: when_taken
_Tags: logic-edit | parameter-tweak_
```diff
  [L33] 			}
  [L34] 			trigger_event = { id = expedition_events.200 popup = yes }
- [L35] 			set_variable = on_expedition
  ↑ inserted after base L34
+ [M55] 			set_variable = {
+ [M56] 				name = on_expedition
+ [M57] 				value = yes
+ [M58] 			}
  [L36] 		}
  [L37] 		else = {
```
