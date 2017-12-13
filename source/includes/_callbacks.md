# Events

## OnLoad

* Called when a script is loaded.

``` lua
function OnLoad()
    __PrintTextGame("OnLoad works")
end
```

## OnTick

* Trigger every tick.

``` lua
function OnTick()
    __PrintTextGame("OnTick works")
end
```

## OnUpdate

* Trigger every screen updates.

``` lua
function OnUpdate()
    __PrintTextGame("OnUpdate works")
end
```

## OnDraw

* Trigger every screen updates.

``` lua
function OnDraw()
    __PrintTextGame("OnDraw works")
end
```

## OnUpdateBuff

* Trigger everytime a buff is updated.

Parameter | Type 
--------- | ------- 
[source](https://shulepin.github.io/ToirAPI/#onevent-unit) | table 
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table 
[buff](https://shulepin.github.io/ToirAPI/#onevent-buff) | table 
stacks | number 

``` lua
function OnUpdateBuff(source, unit, buff, stacks)
        __PrintTextGame(string.format(
                "Source Name: %s | Unit Name: %s | Apply Buff: %s | Stacks: %d",
                source.CharName, unit.CharName, buff.Name, stacks
        ))
end
```

## OnRemoveBuff

* Trigger everytime a buff is removed.

Parameter | Type 
--------- | ------- 
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table 
[buff](https://shulepin.github.io/ToirAPI/#onevent-buff) | table 

``` lua
function OnRemoveBuff(unit, buff)
        __PrintTextGame(string.format(
                "Unit Name: %s | Buff Removed: %s",
                unit.CharName, buff.Name
        ))
end
```

## OnProcessSpell

* Trigger when someone cast anything.

Parameter | Type 
--------- | ------- 
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description
[spell](https://shulepin.github.io/ToirAPI/#onevent-spell) | table | description

``` lua
function OnProcessSpell(unit, spell)
        __PrintTextGame(string.format(
                "Unit Name: %s Cast %s Windup: %d, Animation Time: %d",
                unit.CharName, spell.Name, spell.Delay, spell.AnimationTime
        ))
end
```

## OnCreateObject

* Trigger everytime a new object is created.

Parameter | Type 
--------- | ------- 
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description

``` lua
function OnCreateObject(unit)
        __PrintTextGame(string.format(
                "Created Object: %s",
                unit.Name
        ))
end
```

## OnDeleteObject

* Trigger everytime an object is deleted.

Parameter | Type 
--------- | ------- 
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description

``` lua
function OnDeleteObject(unit)
        __PrintTextGame(string.format(
                "Deleted Object: %s",
                unit.Name
        ))
end
```

## OnWndMsg

* Trigger When you click on Mouse/Keyboard with msg and keys.

Parameter | Type 
--------- | ------- 
message | number 
key | number 

``` lua
function OnWndMsg(message, key)
        __PrintTextGame(string.format(
                "Message: %d | Key: %d",
                message, key
        ))
end
```

## OnDoCast

* Trigger when the spell cast is done (after windup).

Parameter | Type 
--------- | ------- 
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table 
[spell](https://shulepin.github.io/ToirAPI/#onevent-spell) | table 

``` lua
function OnDoCast(unit, spell)
        __PrintTextGame(string.format(
                "Unit Name: %s Cast %s Windup: %d, Animation Time: %d",
                unit.CharName, spell.Name, spell.Delay, spell.AnimationTime
        ))
end
```

## OnPlayAnimation

* Trigger everytime when someone make an animation

Parameter | Type 
--------- | ------- 
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table 
animation | string 

``` lua
function OnPlayAnimation(unit, animation)
        __PrintTextGame(string.format(
                "Unit Name: %s | Animation: %s",
                unit.CharName, animation
        ))
end
```