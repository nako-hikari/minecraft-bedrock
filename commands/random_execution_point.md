# Random Execution Point

## randomize the execution point in an area around the target entity

basically scattering something like a particle in an area around entity 

### Setup
```
/summon armor_stand ~~~ 0 0
```
```
/summon armor_stand ~~~ 180 0
```
``` 
/summon boat ~~~ 0 90
```
```
/summon boat ~~~ 0 -90
```
#### tag those entity with "rdm"
```
/tag @e[type=!player, r=10, c=4] add rdm
```


### then go here : [rnd command value autofill]https://nako-hikari.github.io/minecraft-bedrock/tools/rnd_command_autofill.html)

go to the page and insert your diameter value on the top box
pick a particle, or you can leave it empty if you want to use your own command
and the final command will appear on the bottom, ready to copy

### how to use
make sure the entity from the setup is present

🟪 Repeat : Unconditional: Always Active
[ paste the command ]
and then choose the point
you can replace the "execute as @a" with the entity you want to be the middle point
leave it as it is if you want the middle point to be every player

it can be player @p / @a
or any entity that you want @e[ ]

and dont forget to fill the command at the end


command template [just a template, you can copy the finished version from the page above]
```
execute as @a at @s rotated as @e[tag=rdm,type=armor_stand] positioned ^^^a/64 rotated as @e[tag=rdm,type=armor_stand] positioned ^^^a/32 rotated as @e[tag=rdm,type=armor_stand] positioned ^^^a/16 rotated as @e[tag=rdm,type=armor_stand] positioned ^^^a/8 rotated as @e[tag=rdm,type=armor_stand] positioned ^^^a/4 rotated as @r[tag=rdm,type=armor_stand] positioned ^a/64^^ rotated as @r[tag=rdm,type=armor_stand] positioned ^a/32^^ rotated as @r[tag=rdm,type=armor_stand] positioned ^a/16^^ rotated as @r[tag=rdm,type=armor_stand] positioned ^a/8^^ rotated as @r[tag=rdm,type=armor_stand] positioned ^a/4^^ rotated as @r[tag=rdm,type=boat] positioned ^^^a/64 rotated as @r[tag=rdm,type=boat] positioned ^^^a/32 rotated as @r[tag=rdm,type=boat] positioned ^^^a/16 rotated as @r[tag=rdm,type=boat] positioned ^^^a/8 rotated as @r[tag=rdm,type=boat] positioned ^^^a/4 if entity @s[r=a/2] run [your command here]
```
