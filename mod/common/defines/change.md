# change — Cross-File Diff Note (named parent paths only)

**Generated:** 2025-09-17 18:46:36 JST

## 1) Scope
**Artifacts used:**
- base6.zip (SHA1: `a4826e7795964d2d0a4ba8ae734035c593ebe502`)
- mod6.zip  (SHA1: `1697646ac82ddfbea5d796fd7142487ea4321124`)

**Files compared (base → mod):**
- 00_defines.txt — **needs change**

## 2) Global Summary
- Added blocks: **0**
- Removed blocks: **0**
- Moved within same file (content identical): **0**
- Moved across files (content identical): **0**
- Modified blocks (content changed, no move): **4**
- Moved+Modified within same file: **0**
- Moved+Modified across files: **0**
- Unchanged blocks: **14**

## 3) Block Order by File (Base → Mod)
### 00_defines.txt
**Base order:**
1. `NJominiMap#1`
2. `NCountry#1`
3. `NPolitics#1`
4. `NEconomy#1`
5. `NMilitary#1`
6. `NDiplomacy#1`
7. `NPowerBlocs#1`
8. `NPops#1`
9. `NPops#2`
10. `NEvents#1`
11. `NTechnology#1`
12. `NCharacters#1`
13. `NBattle#1`
14. `NWar#1`
15. `NTravelNetwork#1`
16. `NHarvestConditions#1`
17. `NText#1`
18. `NDebug#1`

**Mod order:**
1. `NJominiMap#1`
2. `NCountry#1`
3. `NPolitics#1`
4. `NEconomy#1`
5. `NMilitary#1`
6. `NDiplomacy#1`
7. `NPowerBlocs#1`
8. `NPops#1`
9. `NPops#2`
10. `NEvents#1`
11. `NTechnology#1`
12. `NCharacters#1`
13. `NBattle#1`
14. `NWar#1`
15. `NTravelNetwork#1`
16. `NHarvestConditions#1`
17. `NText#1`
18. `NDebug#1`

## 4) Modified — detailed diffs (named parent paths, adaptive context)
### File: **00_defines.txt** — Block: `NCountry#1` (base L17-L50)
#### Path: NCountry
_Tags: parameter-tweak_
```diff
  [L42] 	CONSTRUCTION_QUEUE_INCREMENT_CONTROL = 10 # Increment/Decrement used for buildings construction queue when holding down Ctrl
  [L43] 	WEEKS_TO_STORE_LOYALIST_RADICAL_STATISTICS = 52 # Number of weeks of statistics for loyalists/radicals that is stored and shown
- [L44] 	INCORPORATION_TIME_SAME_CULTURE = 2				# Years if the state is a Homeland of one of the country's primary cultures
- [L45] 	INCORPORATION_TIME_SAME_HERITAGE = 5			# Years if the state is a Homeland of a culture that matches of one of the country's primary cultures' Heritage traits
- [L46] 	INCORPORATION_TIME_SAME_TRAIT = 10				# Years if the state is a Homeland of a culture with any trait in common with a country's primary cultures
- [L47] 	INCORPORATION_TIME_NO_MATCH = 20				# Years if the state's Homeland cultures have nothing in common with the country's primary cultures
  ↑ inserted after base L43
+ [M44] 	INCORPORATION_TIME_SAME_CULTURE = 1				# Years if the state is a Homeland of one of the country's primary cultures
+ [M45] 	INCORPORATION_TIME_SAME_HERITAGE = 2			# Years if the state is a Homeland of a culture that matches of one of the country's primary cultures' Heritage traits
+ [M46] 	INCORPORATION_TIME_SAME_TRAIT = 5				# Years if the state is a Homeland of a culture with any trait in common with a country's primary cultures
+ [M47] 	INCORPORATION_TIME_NO_MATCH = 10				# Years if the state's Homeland cultures have nothing in common with the country's primary cultures
  [L48] 	JOURNAL_ENTRY_UPDATE_ACTIVE = 8					# Number of ticks between each update of Active (Possible) Journal Entries, can be overriden on journal entry type
  [L49] 	JOURNAL_ENTRY_UPDATE_INACTIVE = 28				# Number of ticks between each update of Inactive Journal Entries, can be overriden on journal entry type
```

### File: **00_defines.txt** — Block: `NEconomy#1` (base L303-L566)
#### Path: NEconomy
_Tags: parameter-tweak_
```diff
  [L436] 	BUILDING_WEEKS_BETWEEN_PAY_CHANGES_WHEN_UNPROFITABLE = 0 # Cooldown between changes in pay, so buildings don't overcompensate for a temporary change in circumstances. Only used when unprofitable.
  [L437] 	MIN_RAISE_TO_HIRE = 0.10					# The minimum required increase in wages for an employee to switch jobs (1.0 = +100% = x2)
- [L438] 	BASE_RESOURCE_DISCOVER_CHANCE = 0.02 		# Per day (1.0 = 1%)
  ↑ inserted after base L437
+ [M438] 	BASE_RESOURCE_DISCOVER_CHANCE = 0.2 		# Per day (1.0 = 1%)
  [L439] 	EMPLOYMENT_RESOURCE_DEPLETE_CHANCE = 0.005	# Multiplied by number of fully employed levels of the building
  [L440] 	RESOURCE_DISCOVER_MIN_FRACTION = 0.2		# Min fraction of resources that will be discovered for each successful roll
```

### File: **00_defines.txt** — Block: `NDiplomacy#1` (base L667-L1012)
#### Path: NDiplomacy
_Tags: parameter-tweak_
```diff
  [L888] 
  [L889] 	COLONY_PROVINCE_BASE_SCORE = 10
- [L890] 	COLONY_PROVINCE_COASTAL_SCORE = 60 # Replaces COLONY_BASE_SCORE for provinces with a coastline
  ↑ inserted after base L889
+ [M890] 	COLONY_PROVINCE_COASTAL_SCORE = 1000 # Replaces COLONY_BASE_SCORE for provinces with a coastline
  [L891] 	COLONY_PROVINCE_ADJACENCY_SCORE = 25 # How much will colonies prioritize adjacency to existing provinces when growing the colony
  [L892] 	COLONY_PROVINCE_NO_ADJACENCY_MULT = 0.1 # Multiply by this if no adjacencies at all
```

### File: **00_defines.txt** — Block: `NPops#1` (base L1044-L1279)
#### Path: NPops
_Tags: parameter-tweak_
```diff
  [L1208] 	COLONIZATION_RIGHTS_GROWTH_MULTIPLIER = 2.0			# Colonial growth AND max colonial growth are multiplied by this if you have colonization rights
  [L1209] 	COLONIAL_GROWTH_BASE_FACTOR = 0.00001				# Colonial growth generated by a state is this amount per 1000 population, multiplied by the Colonial Growth modifier in the state
- [L1210] 	MIN_BASE_COLONIAL_GROWTH = 0.005					# Country base colonial growth from population cannot be lower than this
  ↑ inserted after base L1209
+ [M1210] 	MIN_BASE_COLONIAL_GROWTH = 0.05					# Country base colonial growth from population cannot be lower than this
  [L1211] 	MAX_BASE_COLONIAL_GROWTH = 0.1						# Country base colonial growth from population cannot be higher than this
  [L1212] 	MAX_COLONIAL_GROWTH = 0.02							# Colonies can grow by this much at most per day
```
