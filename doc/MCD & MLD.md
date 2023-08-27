
# Les entités : 

- TRAINER: code trainer, name,
- TEAM: code team, title, position
- POKEMON: code pokemon, name, nickname, level, image
- TYPE: code type, name, color

# Le MCD via MOCODO :

``````
TRAINER: code trainer, firstname, lastname, email, password
CREER, 0N TRAINER, 11 TEAM
TEAM: code team, title, position
AVOIR, 0N TEAM, 11 POKEMON
POKEMON: code pokemon, pokemon_name, nickname, level, image, position
APPARTIENT, 1N POKEMON, 1N TYPE
TYPE: code type, name, color
``````

# MLD 

**APPARTIENT** (<ins>_#code pokemon_</ins>, <ins>_#code type_</ins>)<br>
**POKEMON** (<ins>code pokemon</ins>, pokemon_name, nickname, level, image, position, _#code team_)<br>
**TEAM** (<ins>code team</ins>, title, position, _#code trainer_)<br>
**TRAINER** (<ins>code trainer</ins>, firstname, lastname, email, password)<br>
**TYPE** (<ins>code type</ins>, name, color)

