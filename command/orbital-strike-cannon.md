# Orbital Strike Cannon

## Setup (Run in Chat)

```
/summon boat ~~~ 0 90
``` 
``` 
/summon boat ~~~ 180 -90
``` 
``` 
/tag @e[type=boat, r=5, c=2] add r
``` 


## Command Blocks

🟪 Unconditional • Always Active
``` 
/tag @e[type=xp_orb] add ex1
``` 

🟩 Unconditional • Always Active
``` 
/execute as @a at @s anchored eyes if entity @e[type=fishing_hook, r=3] run summon xp_orb ~~~ ~~
``` 

🟩 Unconditional • Always Active
``` 
/execute at @a if entity @e[type=fishing_hook, r=3] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[c=2] as @e[type=xp_orb,tag=!ex1] at @s run tp @s ^^^0.15 true
``` 

🟩 Unconditional • Always Active
``` 
/execute at @a if entity @e[type=fishing_hook, r=3] positioned 0 0 0 rotated as @e[tag=r] positioned ^1^^ rotated as @e[tag=r] rotated ~ 0 positioned ^^^1 rotated as @e[tag=r] positioned ^1.414^^ facing 0 0 0 positioned 0 0 0 positioned ^^^1 rotated as @e[tag=r] positioned ^1^^ facing 0 0 0 positioned 0 0 0 positioned ^^^1 facing 0 0 0 positioned 0 0 0 positioned ^^^1 rotated as @e[tag=r] positioned ^1^^ facing 0 0 0 positioned 0 0 0 positioned ^^^1 rotated as @e[tag=r] positioned ^^^1 rotated as @e[tag=r] positioned ^^^1.414 facing 0 0 0 positioned 0 0 0 positioned ^^^1 rotated as @e[tag=r] positioned ^^^1 facing 0 0 0 positioned 0 0 0 positioned ^^^1 as @e[type=xp_orb,tag=!ex1] positioned as @s positioned ^^^20 positioned ~~20~ facing entity @s feet positioned ^^^50 positioned ~~10000~ facing entity @s feet positioned as @s positioned ^^^-10000 positioned ~~-10000~ run summon tnt ~~60~
``` 

🟩 Unconditional • Always Active
``` 
/kill @e[type=xp_orb,tag=!ex1]
``` 

🟩 Unconditional • Always Active
``` 
/kill @e[type=fishing_hook]
```
