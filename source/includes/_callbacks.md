# Callback Functions

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

## UpdateBuff(unit, buff, stacks)

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