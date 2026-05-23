# Shooting fireball when you crouch 

## setup visualization 
<div style="max-width: 35%; margin: 0 auto;">
<ol reversed start="3">
  <li><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"></li>
  <li><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"></li>
  <li><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/repeat.png" width="50"></li>
</ol>
</div>

## setup
### 1. 🟪 Repeat : Unconditional: Always Active
``` 
/tp @n[type=fireball] ~~3~
``` 

### 2. 🟩 Chain : Conditional : Always Active
``` 
/Kill @e[type=ghast]
``` 

### 3. 🟩 Chain : Conditional : Always Active
``` 
/structure save fireball ~~0.5~ ~~~ true disk false
```

### Spawn a ghast
``` 
/summon ghast
``` 

### go to survival mode and wait until the ghast died
``` 
/gamemode s
``` 
#### and your setup is done


## command visualization 
<div style="max-width: 35%; margin: 0 auto;">
<ol reversed start="4">
  <li><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"></li>
  <li><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"></li>
  <li><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/chain.png" width="50"></li>
  <li><img src="https://raw.githubusercontent.com/nako-hikari/support-files/main/assets/minecraft/repeat.png" width="50"></li>
</ol>
</div>

## commands
### 1. 🟪 Repeat : Unconditional : Always Active : Tick=5
```
/execute as @a at @s unless entity @s[y=~1.5, dy=0] run structure load fireball ~~~
```

### 2. 🟩 Chain : Unconditional : Always Active
```
/execute as @a at @s anchored eyes run tp @e[type=fireball, tag=!hit, r=3] ^^^1
```

### 3. 🟩 Chain : Unconditional : Always Active
```
/execute as @a at @s run damage @n[type=fireball, tag=!hit] 0 none entity @s
```

### 4. 🟩 Chain : Unconditional : Always Active
```
/tag @e[type=fireball] add hit
```

