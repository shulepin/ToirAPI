# Events

## OnLoad()

* Called when a script is loaded.

``` lua
function OnLoad()
    __PrintTextGame("OnLoad works")
end
```

## OnTick()

* Trigger every tick.

``` lua
function OnTick()
    __PrintTextGame("OnTick works")
end
```

## OnUpdate()

* Trigger every screen updates.

``` lua
function OnUpdate()
    __PrintTextGame("OnUpdate works")
end
```

## OnDraw()

* Trigger every screen updates.

``` lua
function OnDraw()
    __PrintTextGame("OnDraw works")
end
```

## OnUpdateBuff(unit, buff, stacks)

* Trigger Everytime a buff is Updated.

Parameter | Type | Description
--------- | ------- | -----------
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description
[buff](https://shulepin.github.io/ToirAPI/#onevent-buff) | table | description
stacks | number | description

``` lua
function OnUpdateBuff(unit, buff, stacks)
    --
end
```

## OnRemoveBuff(unit, buff)

* Trigger Everytime a buff is Removed.

Parameter | Type | Description
--------- | ------- | -----------
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description
[buff](https://shulepin.github.io/ToirAPI/#onevent-buff) | table | description

``` lua
function OnRemoveBuff(unit, buff)
    --
end
```

## OnProcessSpell(unit, spell)

* Trigger when Someone Cast Anything.

Parameter | Type | Description
--------- | ------- | -----------
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description
[spell](https://shulepin.github.io/ToirAPI/#onevent-spell) | table | description

``` lua
function OnProcessSpell(unit, spell)
    --
end
```

## OnCreateObject(unit)

* Trigger everytime a new object is Created.

Parameter | Type | Description
--------- | ------- | -----------
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description

``` lua
function OnCreateObject(unit)
    --
end
```

## OnDeleteObject(unit)

* Trigger everytime an object is Deleted.

Parameter | Type | Description
--------- | ------- | -----------
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description

``` lua
function OnDeleteObject(unit)
    --
end
```

## OnWndMsg(message, key)

* Trigger When You Click on Mouse/Keyboard with msg and keys.

Parameter | Type | Description
--------- | ------- | -----------
message | number | description
key | number | description

``` lua
function OnWndMsg(message, key)
    --
end
```

## OnDoCast(unit, spell)

* Trigger when the Spell Cast is done (after windup).

Parameter | Type | Description
--------- | ------- | -----------
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description
[spell](https://shulepin.github.io/ToirAPI/#onevent-spell) | table | description

``` lua
function OnDoCast(unit, spell)
    --
end
```

## OnPlayAnimation(unit, animation)

* Trigger Everytime when someone make an animation

Parameter | Type | Description
--------- | ------- | -----------
[unit](https://shulepin.github.io/ToirAPI/#onevent-unit) | table | description
animation | string | description

``` lua
function OnPlayAnimation(unit, animation)
    --
end
```