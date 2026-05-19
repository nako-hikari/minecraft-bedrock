# Nudge System

## Teleporting a command block tower either up 1 block, down 1 block, or copy current block into above if there's air
### using xp orb raycast system to detect where you look

### visualization 
<div style="max-width: 35%; margin: 0 auto; display: flex; flex-direction: column; align-items: center; font-family: monospace;">
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">17.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">16.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">15.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">14.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain-conditional.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">13.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">12.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain-conditional.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">11.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">10.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">9.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">8.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">7.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">6.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">5.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">4.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">3.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">2.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
  <div style="display: flex; align-items: center; justify-content: flex-end; width: 100%; height: 50px; line-height: 0;">
    <span style="color: #5a5a66; font-weight: bold; font-size: 14px; margin-right: 12px; white-space: nowrap;">1.</span>
    <img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/repeat.png" width="50" height="50" style="display: block; margin: 0; padding: 0; border: none; object-fit: contain;">
    <div style="flex-grow: 1;"></div>
  </div>
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
