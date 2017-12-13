# Global Functions

## IncludeFile

Parameter | Type 
--------- | ------- 
fileName | string 

## GetScriptPath

* Returns the path to the Scripts folder

## SetLuaCombo

Parameter | Type 
--------- | ------- 
state | boolean

## SetLuaHarass

Parameter | Type 
--------- | ------- 
state | boolean


## SetLuaLaneClear

Parameter | Type 
--------- | ------- 
state | boolean


## SetLuaBasicAttackOnly

Parameter | Type 
--------- | ------- 
state | boolean


## SetLuaMoveOnly

Parameter | Type 
--------- | ------- 
state | boolean

## GetDistance2D

Parameter | Type 
--------- | ------- 
x1 | number
z1 | number
x2 | number
z2 | number

## SetEvade

Parameter | Type 
--------- | ------- 
state | boolean

## GetEvade

## SetPrintErrorLog

Parameter | Type 
--------- | ------- 
state | boolean


## GetKeyPress

Parameter | Type 
--------- | ------- 
key | number

## GetKeyCode

## IsDodging

## IsTyping

## IsWall

Parameter | Type 
--------- | ------- 
x | number
y | number
z | number

## GetMousePos

```lua
local x, y, z = GetMousePos()
```

## GetCursorPos

```lua
local x, y = GetCursorPos()
```

## GetMousePosX
## GetMousePosY
## GetMouserPosZ
## GetTimeGame
## GetTickCount
## GetLatency

## UpSpellLevel

Parameter | Type 
--------- | ------- 
spellIndex | number

## Setting_IsComboUseQ
## Setting_IsComboUseW
## Setting_IsComboUseE
## Setting_IsComboUseR
## Setting_IsHarassUseQ
## Setting_IsHarassUseW
## Setting_IsHarassUseE
## Setting_IsHarassUseR
## Setting_IsLaneClearUseQ
## Setting_IsLaneClearUseW
## Setting_IsLaneClearUseE
## Setting_IsLaneClearUseR

## CanCast

Parameter | Type 
--------- | ------- 
spellIndex | number

## CastSpellTarget

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number

## CastSpellToPos

Parameter | Type 
--------- | ------- 
x | number
z | number
spellIndex | number

## CastSpellToPos_2

Parameter | Type | Description
--------- | ------- | -----------
x1 | number | start position
z1 | number | start position
x2 | number | end position
z2 | number | end position
spellIndex | number | spell index

## CastSpellToPredictionPos

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number
distantPrediction | number

## ReleaseSpellToPos

Parameter | Type 
--------- | ------- 
x | number
z | number
spellIndex | number

## ReleaseSpellToPredictionPos

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number
distantPrediction | number

## ReleaseSpellToPredictionPos_2

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number
distantPrediction | number

## CastSpellTargetByName

Parameter | Type 
--------- | ------- 
pObject | number
spellName | string

## GetSpellIndexByName

Parameter | Type 
--------- | ------- 
spellName | string

## GetSpellNameByIndex

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number

## GetSpellLevel

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number

## GetCDSpell

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number

## GetCDExpiresSpell

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number

## GetAmmoSpell

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number

## GetToggleSpell

Parameter | Type 
--------- | ------- 
pObject | number
spellIndex | number

## BasicAttack

Parameter | Type 
--------- | ------- 
pObject | number

## GetWindupBA

Parameter | Type 
--------- | ------- 
pObject | number

## GetCDBA

Parameter | Type 
--------- | ------- 
pObject | number

## GetCDExpiresBA

Parameter | Type 
--------- | ------- 
pObject | number

## GetAADamageHitEnemy

Parameter | Type 
--------- | ------- 
pObjectEnemy | number

## GetSpellCasting

Parameter | Type 
--------- | ------- 
pObject | number

## GetName_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetOwnerID_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetTargetID_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetSrcPos_Cast

Parameter | Type 
--------- | ------- 
pSpellCasting | number

```lua
local x, y, z = GetSrcPos_Cast(pSpellCasting)
```

## GetSrcPosX_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetSrcPosY_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetSrcPosZ_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetDestPos_Cast

Parameter | Type 
--------- | ------- 
pSpellCasting | number

```lua
local x, y, z = GetDestPos_Cast(pSpellCasting)
```

## GetDestPosX_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetDestPosY_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetDestPosZ_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetCursorPos_Cast

Parameter | Type 
--------- | ------- 
pSpellCasting | number

```lua
local x, y, z = GetCursorPos_Cast(pSpellCasting)
```

## GetCursorPosX_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetCursorPosY_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetCursorPosZ_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetDelay_Casting)

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## GetTime_Casting

Parameter | Type 
--------- | ------- 
pSpellCasting | number

## SearchAllChamp

* Return array pObjChamp:
pObjChamp[1], pObjChamp[2], pObjChamp[3] ... pObjChamp[10]
		
## GetAllObjectAroundAnObject

* Return array pObject(include: pObjChamp, pObjMinion, pObjTurret, ...):					
pObject[1], pObject[2], pObject[3] ... pObject[500]

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## GetAllUnitAroundAnObject
* Return table "pUnit": pUnit[1], pUnit[2], pUnit[3] ... pUnit[300]

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## GetEnemyChampCanKillFastest
* Return EnemyChamp can kill fastest by AD-damage

Parameter | Type 
--------- | ------- 
range | number

## GetEnemyChampCanKillFastest_AP
* Return EnemyChamp can kill fastest by AP-damage

Parameter | Type 
--------- | ------- 
range | number

## GetEnemyChampNearest
* Return EnemyChamp nearest
	
Parameter | Type 
--------- | ------- 
range | number

## GetEnemyChampMinHP
* Return EnemyChamp MinHP

Parameter | Type 
--------- | ------- 
range | number

## GetEnemyChampCCAroundObject
* Return EnemyChamp CC around pObject 

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## CountEnemyChampAroundObject
* Return count EnemyChamp around pObject 

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## CountAllyChampAroundObject
* Return count AllyChamp around pObject

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## CountEnemyMinionAroundObject
* Return count EnemyMinion around pObject 

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## CountEnemyTurretAroundObject
* Return count EnemyTurret around pObject 

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## GetEnemyMinionAroundObject

Parameter | Type 
--------- | ------- 
pObject | number
range | number

## GetJungleMonster

Parameter | Type 
--------- | ------- 
range | number

## CountObjectCollision

Parameter | Type | Description
--------- | ------- | -----------
mode | number | 0 - enemy minion, 1 - enemy minion or champ, 2 - enemy champ
pObjEnemy | number | enemy pointer
x1 | number | start position
z1 | number | start position
x2 | number | end position
z2 | number | end position
width | number | the width
range | number | the range
radius | number | the radius

## GetLastBATick
## CanMove
## CanAttack

## MoveToPos

Parameter | Type 
--------- | ------- 
x | number
z | number

## IsMoving

Parameter | Type 
--------- | ------- 
pObject | number

## IsDashing

Parameter | Type 
--------- | ------- 
pObject | number

## GetDestPos

Parameter | Type 
--------- | ------- 
pObject | number

```lua
local x,y,z = GetDestPos(pObject)
```

## GetMoveDestPointPosX

Parameter | Type 
--------- | ------- 
pObject | number

## GetMoveDestPointPosY

Parameter | Type 
--------- | ------- 
pObject | number

## GetMoveDestPointPosZ

Parameter | Type 
--------- | ------- 
pObject | number

## GetPredPos

Parameter | Type 
--------- | ------- 
pObject | number
distance | number

```lua
local x,y,z = GetPredPos(pObject, nDistant)
```

## GetPredictionPosX

Parameter | Type 
--------- | ------- 
pObject | number
distance | number

## GetPredictionPosY

Parameter | Type 
--------- | ------- 
pObject | number
distance | number

## GetPredictionPosZ

Parameter | Type 
--------- | ------- 
pObject | number
distance | number

## BlockMove
## UnBlockMove

## GetItemByID

Parameter | Type 
--------- | ------- 
itemID | number

## GetItemID

Parameter | Type 
--------- | ------- 
slotItem | number

## BuyItem

Parameter | Type 
--------- | ------- 
itemID | number

## DrawCircleGame

Parameter | Type 
--------- | ------- 
x | number
y | number
z | number
radius | number
color | number

## DrawLineGame

Parameter | Type 
--------- | ------- 
x1 | number
y1 | number
z1 | number
x2 | number
y2 | number
z2 | number
radius | number

## GetHealthBarPos

Parameter | Type 
--------- | ------- 
pObject | number

```lua
local a,b =  GetHealthBarPos(pObj)
```

## WorldToMiniMap

Parameter | Type 
--------- | ------- 
x | number
y | number
z | number

```lua
local a,b =  WorldToMiniMap(x, y, z)
```

## WorldToScreen

Parameter | Type 
--------- | ------- 
x | number
y | number
z | number

```lua
local a,b =  WorldToScreen(x, y, z)
```

## DrawLineD3DX

Parameter | Type 
--------- | ------- 
x1 | number
y1 | number
x2 | number
z2 | number
width | number
color | number

## DrawBorderBoxD3DX

Parameter | Type 
--------- | ------- 
x | number
y | number
width | number
height | number
thickness | number
color | number

## DrawTextD3DX

Parameter | Type 
--------- | ------- 
x | number
y | number
text | string
color | number
fontHeight | number

## GetAllBuffNameActive
* Return array Buff Name: pBuffName[1], pBuffName[2], pBuffName[3] ... pBuffName[60]

Parameter | Type 
--------- | ------- 
pObject | number

## GetBuffName

Parameter | Type 
--------- | ------- 
pBuff | number

## GetBuffByName

Parameter | Type 
--------- | ------- 
pObject | number
buffName | string

## GetBuffType

Parameter | Type 
--------- | ------- 
pObject | number
buffName | string

## CountBuffByType 

Parameter | Type 
--------- | ------- 
pObject | number
buffType | number 

## GetBuffTimeBegin

Parameter | Type 
--------- | ------- 
pObject | number
buffName | string

## GetBuffTimeEnd

Parameter | Type 
--------- | ------- 
pObject | number
buffName | string

## GetBuffStack

Parameter | Type 
--------- | ------- 
pObject | number
buffName | string

## GetBuffCount

Parameter | Type 
--------- | ------- 
pObject | number
buffName | string