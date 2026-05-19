# Nudge System

## Teleporting a command block tower either up 1 block, down 1 block, or copy current block into above if there's air
### using xp orb raycast system to detect where you look

### visualization 
<div style="max-width: 35%; margin: 0 auto;">

17. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
16. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
15. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
14. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain-conditional.png" width="50"><br>
13. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
12. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain-conditional.png" width="50"><br>
11. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
10. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
9. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
8. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
7. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
6. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
5. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
4. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
3. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
2. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"><br>
1. <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/repeat.png" width="50"><br>

</div>

### Setup
``` 
/scoreboard objectives add nudge dummy
``` 

### Get item
``` 
/give @s snowball 1 4
``` 

### Command - make sure the conditional and unconditional is correct!

1. 🟪 Repeat : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] run titleraw @s actionbar {"rawtext":[{"translate":"%%2","with":{"rawtext":[{"selector":"@s[scores={nudge=0}]"},{"text":"§l§aMOVE UP§r"}]}},{"translate":"%%2","with":{"rawtext":[{"selector":"@s[scores={nudge=1}]"},{"text":"§l§bMOVE DOWN§r"}]}},{"translate":"%%2","with":{"rawtext":[{"selector":"@s[scores={nudge=2}]"},{"text":"§l§cCOPY BOTTOM§r"}]}}]}
``` 

2. 🟩 Chain : Unconditional : Always Active
```
/scoreboard players set @a[scores={nudge=3}] nudge 0
``` 

3. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] unless entity @e[name=nudge] run scoreboard players add @s nudge 1
``` 

4. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] at @s unless entity @e[name=nudge] run summon armor_stand nudge ~~3~
``` 

5. 🟩 Chain : Unconditional : Always Active
```
/effect @e[name=nudge] invisibility infinite 1 true
``` 

6. 🟩 Chain : Unconditional : Always Active
```
/execute as @a at @s run tp @e[name=nudge] ~~3~
``` 

7. 🟩 Chain : Unconditional : Always Active
```
/execute as @a unless entity @s[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] run kill @e[name=nudge]
``` 

8. 🟩 Chain : Unconditional : Always Active
```
/tag @e[type=xp_orb] add ex1
``` 

9. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] at @s anchored eyes if entity @e[type=snowball,r=2] run summon xp_orb ~~~ ~~
``` 

10. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[type=xp_orb,tag=!ex1] at @s run tp @s ^^^0.1 true
``` 

11. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=0}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 run clone ~~~ ~~100~ 0 0 0 replace move
``` 

12. 🟩 Chain : Conditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=0}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 run clone 0 0 0 0 100 0 ~~1~ replace move
``` 

13. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=1}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s positioned ^^^0.25 if block ~~-1~ air run clone ~~~ ~~100~ 0 0 0 replace move
``` 

14. 🟩 Chain : Conditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=1}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 if block ~~-1~ air run clone 0 0 0 0 100 0 ~~-1~ replace move
``` 

15. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4},scores={nudge=2}] at @s anchored eyes if entity @e[type=snowball,r=2] as @e[type=xp_orb,tag=!ex1] at @s rotated as @p positioned ^^^0.25 if block ~~1~ air run clone ~~~ ~~~ ~~1~
```

16. 🟩 Chain : Unconditional : Always Active
```
/execute as @a[hasitem={item=snowball,location=slot.weapon.mainhand,data=4}] run kill @e[type=snowball]
``` 

17. 🟩 Chain : Unconditional : Always Active
```
/kill @e[type=xp_orb,tag=!ex1]
``` 
