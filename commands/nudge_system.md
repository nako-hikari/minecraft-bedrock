# Nudge System

## Teleporting a command block tower either up 1 block, down 1 block, or copy current block into above if there's air
### using xp orb raycast system to detect where you look


### Setup
``` 
/scoreboard objectives add nudge dummy
``` 

### Get item
``` 
/give @s snowball 1 4
``` 

### Command - make sure the conditional and unconditional is correct!

🟪 Repeat : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] run titleraw @s actionbar {"rawtext":[{"translate":"%%2","with":{"rawtext":[{"selector":"@s[scores={nudge=0}]"},{"text":"§l§aMOVE UP§r"}]}},{"translate":"%%2","with":{"rawtext":[{"selector":"@s[scores={nudge=1}]"},{"text":"§l§bMOVE DOWN§r"}]}},{"translate":"%%2","with":{"rawtext":[{"selector":"@s[scores={nudge=2}]"},{"text":"§l§cCOPY BOTTOM§r"}]}}]}
``` 

🟩 Chain : Unconditional : Always Active
```
/scoreboard players set @a[scores={nudge=3}] nudge 0
``` 

🟩 Chain : Unconditional : Always Active
```
/kill @e[type=xp_orb,tag=!ex1]
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] run kill @e[type=snowball]
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] unless entity @e[name=nudge] run scoreboard players add @s nudge 1
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] at @s unless entity @e[name=nudge] run summon armor_stand nudge ~~3~
``` 

🟩 Chain : Unconditional : Always Active
```
/effect @e[name=nudge] invisibility infinite 1 true
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a at @s run tp @e[name=nudge] ~~3~
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a unless entity @s[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] run kill @e[name=nudge]
``` 

🟩 Chain : Unconditional : Always Active
```
/tag @e[type=xp_orb] add ex1
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] at @s anchored eyes if entity @e[type=snowball,r=2] run summon xp_orb ~~~ ~~
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[type=xp_orb,tag=!ex1] at @s run tp @s ^^^0.1 true
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=0}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 run clone ~~~ ~100~ 000 replace move
``` 

🟩 Chain : Conditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=0}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 run clone 0 0 0 0 100 0 ~~1~ replace move
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=1}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s positioned ^^^0.25 if block ~~-1~ air run clone ~~~ ~100~ 000 replace move
``` 

🟩 Chain : Conditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=1}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 if block ~~-1~ air run clone 0 0 0 0 100 0 ~~-1~ replace move
``` 

🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=2}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 if block ~~1~ air run clone ~~~ ~~~ ~~1~
```
