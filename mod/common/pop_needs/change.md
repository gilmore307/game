# change — Cross-File Diff Note (named parent paths only)

**Generated:** 2025-09-17 19:54:31 JST

## 1) Scope
**Artifacts used:**
- base12.zip (SHA1: `76e096d628ecd31c178dc43569910391e701fec6`)
- mod12.zip  (SHA1: `b82d784b5b9db0c7052e4c464b898800cefeac51`)

**Files compared (base → mod):**
- 00_pop_needs.txt — **needs change**

## 2) Global Summary
- Added blocks: **2**
- Removed blocks: **0**
- Moved within same file (content identical): **0**
- Moved across files (content identical): **0**
- Modified blocks (content changed, no move): **6**
- Moved+Modified within same file: **0**
- Moved+Modified across files: **0**
- Unchanged blocks: **8**

## 3) Block Order by File (Base → Mod)
### 00_pop_needs.txt
**Base order:**
1. `popneed_simple_clothing#1`
2. `popneed_crude_items#1`
3. `popneed_basic_food#1`
4. `popneed_heating#1`
5. `popneed_household_items#1`
6. `popneed_standard_clothing#1`
7. `popneed_services#1`
8. `popneed_intoxicants#1`
9. `popneed_luxury_drinks#1`
10. `popneed_free_movement#1`
11. `popneed_communication#1`
12. `popneed_luxury_food#1`
13. `popneed_luxury_items#1`
14. `popneed_leisure#1`

**Mod order:**
1. `popneed_simple_clothing#1`
2. `popneed_crude_items#1`
3. `popneed_basic_food#1`
4. `popneed_heating#1`
5. `popneed_household_items#1`
6. `popneed_standard_clothing#1`
7. `popneed_services#1`
8. `popneed_intoxicants#1`
9. `popneed_luxury_drinks#1`
10. `popneed_free_movement#1`
11. `popneed_communication#1`
12. `popneed_luxury_food#1`
13. `popneed_luxury_items#1`
14. `popneed_leisure#1`
15. `popneed_medication#1`
16. `popneed_education#1`

## 4) Modified — detailed diffs (named parent paths, adaptive context)
### File: **00_pop_needs.txt** — Block: `popneed_household_items#1` (base L134-L160)
#### Path: popneed_household_items
_Tags: list-edit | logic-edit | parameter-tweak_
```diff
  [L134] popneed_household_items = {
- [L135] 	default = furniture
  ↑ inserted after base L134
+ [M135] 	default = newspapers
+ [M136] 
+ [M137] 	entry = {
+ [M138] 		goods = newspapers
+ [M139] 		
+ [M140] 		weight = 0.5
+ [M141] 		max_supply_share = 1 
+ [M142] 		min_supply_share = 0.0
+ [M143] 	}	
  [L136] 
  [L137] 	entry = {
  [L138] 		goods = furniture
```
#### Path: popneed_household_items > entry
_Tags: logic-edit_
```diff
  [L156] 		weight = 0.5
  [L157] 		max_supply_share = 0.5
  [L158] 		min_supply_share = 0.0
- [L159] 	}	
  ↑ inserted after base L158
+ [M167] 	}
  [L160] }
```

### File: **00_pop_needs.txt** — Block: `popneed_intoxicants#1` (base L178-L212)
#### Path: popneed_intoxicants
_Tags: list-edit_
```diff
  [L201] 		max_supply_share = 0.75
  [L202] 		min_supply_share = 0.0
  [L203] 	}
- [L204] 	
  ↑ inserted after base L203
+ [M212] 
  [L205] 	entry = {
  [L206] 		goods = wine
  [L207] 		
```
#### Path: popneed_intoxicants > entry
_Tags: list-edit | numeric-change_
```diff
  [L196] 	
  [L197] 	entry = {
  [L198] 		goods = opium
- [L199] 		 
- [L200] 		weight = 1.5
  ↑ inserted after base L198
+ [M207] 		
+ [M208] 		weight = 1
  [L201] 		max_supply_share = 0.75
  [L202] 		min_supply_share = 0.0
  [L203] 	}
```
```diff
  [L205] 	entry = {
  [L206] 		goods = wine
  [L207] 		
- [L208] 		weight = 0.25
- [L209] 		max_supply_share = 0.25
  ↑ inserted after base L207
+ [M216] 		weight = 0.5
+ [M217] 		max_supply_share = 0.75
  [L210] 		min_supply_share = 0.0
  [L211] 	}
  [L212] }
```

### File: **00_pop_needs.txt** — Block: `popneed_luxury_drinks#1` (base L214-L240)
#### Path: popneed_luxury_drinks > entry
_Tags: numeric-change_
```diff
  [L234] 		goods = wine
  [L235] 		
- [L236] 		weight = 0.33
- [L237] 		max_supply_share = 0.33
  ↑ inserted after base L235
+ [M244] 		weight = 1
+ [M245] 		max_supply_share = 0.75
  [L238] 		min_supply_share = 0.0
  [L239] 	}
```

### File: **00_pop_needs.txt** — Block: `popneed_free_movement#1` (base L242-L260)
#### Path: popneed_free_movement
_Tags: list-edit | logic-edit_
```diff
  [L249] 		max_supply_share = 0.75
  [L250] 		min_supply_share = 0.0
  [L251] 	}
- [L252] 	
  ↑ inserted after base L251
+ [M260] 
+ [M261] 	entry = {
+ [M262] 		goods = clippers
+ [M263] 		
+ [M264] 		weight = 2
+ [M265] 		max_supply_share = 0.33
+ [M266] 		min_supply_share = 0.0
+ [M267] 	}
+ [M268] 
  [L253] 	entry = {
  [L254] 		goods = automobiles
  [L255] 		
```
```diff
  [L257] 		max_supply_share = 1.0
  [L258] 		min_supply_share = 0.0
  [L259] 	}
  ↑ inserted after base L259
+ [M276] 
+ [M277] 	entry = {
+ [M278] 		goods = steamers
+ [M279] 		
+ [M280] 		weight = 3
+ [M281] 		max_supply_share = 0.33
+ [M282] 		min_supply_share = 0.0
+ [M283] 	}
+ [M284] 
+ [M285] 	entry = {
+ [M286] 		goods = aeroplanes
+ [M287] 		
+ [M288] 		weight = 3
+ [M289] 		max_supply_share = 0.33
+ [M290] 		min_supply_share = 0.0
+ [M291] 	}
+ [M292] 
  [L260] }
```
#### Path: popneed_free_movement > entry
_Tags: numeric-change_
```diff
  [L253] 	entry = {
  [L254] 		goods = automobiles
  [L255] 		
- [L256] 		weight = 1.25
- [L257] 		max_supply_share = 1.0
  ↑ inserted after base L255
+ [M272] 		weight = 2
+ [M273] 		max_supply_share = 0.33
  [L258] 		min_supply_share = 0.0
  [L259] 	}
  [L260] }
```

### File: **00_pop_needs.txt** — Block: `popneed_luxury_items#1` (base L318-L352)
#### Path: popneed_luxury_items
_Tags: list-edit | logic-edit_
```diff
  [L342] 		min_supply_share = 0.1
  [L343] 	}
- [L344] 
- [L345] 	entry = {
- [L346] 		goods = radios
- [L347] 		
- [L348] 		weight = 1
- [L349] 		max_supply_share = 0.5
- [L350] 		min_supply_share = 0.0
- [L351] 	}
  [L352] }
```

### File: **00_pop_needs.txt** — Block: `popneed_leisure#1` (base L354-L428)
#### Path: popneed_leisure
_Tags: list-edit | logic-edit_
```diff
  [L367] 		
  [L368] 		weight = 4
  [L369] 		max_supply_share = 1.0
  [L370] 		min_supply_share = 0.0
  [L371] 	}
- [L372] 	
- [L373] 	entry = {
- [L374] 		goods = small_arms
- [L375] 		
- [L376] 		weight = 0.75
- [L377] 		max_supply_share = 0.25
- [L378] 		min_supply_share = 0.0
- [L379] 	}
- [L380] 	
- [L381] 	entry = {
- [L382] 		goods = aeroplanes
- [L383] 		
- [L384] 		weight = 1
- [L385] 		max_supply_share = 0.2
- [L386] 		min_supply_share = 0.0
- [L387] 	}
- [L388] 	
- [L389] 	entry = {
- [L390] 		goods = automobiles
- [L391] 		
- [L392] 		weight = 1
- [L393] 		max_supply_share = 0.25
- [L394] 		min_supply_share = 0.0
- [L395] 	}
- [L396] 	
- [L397] 	entry = {
- [L398] 		goods = radios
- [L399] 		
- [L400] 		weight = 1
- [L401] 		max_supply_share = 0.2
- [L402] 		min_supply_share = 0.0
- [L403] 	}
- [L404] 	
- [L405] 	entry = {
- [L406] 		goods = opium
- [L407] 		
- [L408] 		weight = 0.5
- [L409] 		max_supply_share = 0.5
- [L410] 		min_supply_share = 0.0
- [L411] 	}
- [L412] 	
- [L413] 	entry = {
- [L414] 		goods = clippers
- [L415] 		
- [L416] 		weight = 1
- [L417] 		max_supply_share = 0.25
- [L418] 		min_supply_share = 0.0
- [L419] 	}
- [L420] 	
- [L421] 	entry = {
- [L422] 		goods = steamers
- [L423] 		
- [L424] 		weight = 0.75
- [L425] 		max_supply_share = 0.25
- [L426] 		min_supply_share = 0.0
- [L427] 	}
  [L428] }
```
#### Path: popneed_leisure > entry
_Tags: list-edit | logic-edit | numeric-change_
```diff
  [L357] 	entry = {
  [L358] 		goods = services
  [L359] 		
- [L360] 		weight = 0.1
  ↑ inserted after base L359
+ [M385] 		weight = 0.5
  [L361] 		max_supply_share = 1.0
  [L362] 		min_supply_share = 0.0
  [L363] 	}
```
```diff
  [L362] 		min_supply_share = 0.0
  [L363] 	}
  [L364] 	
  ↑ inserted after base L364
+ [M390] 	entry = {
+ [M391] 		goods = books
+ [M392] 		
+ [M393] 		weight = 2
+ [M394] 		max_supply_share = 1.0
+ [M395] 		min_supply_share = 0.0
+ [M396] 	}
+ [M397] 
+ [M398] 	entry = {
+ [M399] 		goods = radios
+ [M400] 		
+ [M401] 		weight = 2
+ [M402] 		max_supply_share = 0.2
+ [M403] 		min_supply_share = 0.0
+ [M404] 	}
+ [M405] 
  [L365] 	entry = {
  [L366] 		goods = fine_art
  [L367] 		
```
