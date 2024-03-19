## Welcome to this amazing project !

You arrive in a new mission. This is where your travel begins.
Your client want to create a custom front application where he'll could find, a lot of information about ... Pokemon
In fact, that client he's a nerd and a huge fan about that little monsters. 

Your mission, create that application.

### Specifications :
- Application should have a menu with two main tab : Pokemon list, Random Team. By default, pokemon list should be the open tab
- The client authorizes the use of components library like Material, Bootstrap or Clarity (or other)

#### 1 - Menu
Without menu, no navigation.
Create your own menu with two tabs "Pokemon list" and "random team"

#### 2 - Pokemon List

On that tab, the client wants :
- a table of all Pokemon with that columns :
    - pokedexId
    - name
    - generationId
    - image
- a form search
- an editable sort (by default on pokedexId) on all columns (except image)

When you click on a pokemon, you'll be redirect on page with specifics informations on that pokemon :
- types
- resistances types
- evolution(s)
- déveolution
Be careful, that page could be shared and return the same result at refresh.

#### 3 - Random Team
On that tab, the client wants :
- cards of random pokemon team
- he would like to be able to specify some criteria for his team :
    - type (multiple) optionnal
    - generation 1 to 8 (multiple) optionnal
    - number of pokemon : 1 to 6 (by default 6)
- he would like to see his team's defensive coverage on a right panel

### Useful links

The customer is nice and provides you with a list of routes to use (and only these).
- GET https://pokebuildapi.fr/api/v1/pokemon
- GET https://pokebuildapi.fr/api/v1/pokemon/{pokemonId}
- GET https://pokebuildapi.fr/api/v1/types
- POST https://pokebuildapi.fr/api/v1/team/defensive-coverage/v2
    - input : { [pokemonId: number]: ""}[] (ex: [{1: ""}, {2: ""}])

