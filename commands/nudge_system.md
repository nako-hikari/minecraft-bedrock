# Nudge System

## Teleporting a command block tower either up 1 block, down 1 block, or copy current block into above if there's air
### using xp orb raycast system to detect where you look

### visualization 
<table style="max-width: 35%; margin: 0 auto; border-collapse: collapse; border: none; font-family: monospace;">
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">17.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">16.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">15.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">14.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain-conditional.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">13.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">12.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain-conditional.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">11.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">10.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">9.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">8.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">7.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">6.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">5.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">4.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">3.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">2.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
  <tr>
    <td style="padding: 0 var(--space-md) 0 0; text-align: right; vertical-align: middle; border: none; color: #5a5a66; font-weight: bold; font-size: 14px;">1.</td>
    <td style="padding: 0; line-height: 0; border: none;"><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/repeat.png" width="50" style="display: block; margin: 0; padding: 0;"></td>
  </tr>
</table>

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
