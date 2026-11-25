# Field Pokédex — No. 021 to 120

A Pokédex web page built with HTML, CSS and JavaScript that reads its data from [PokeAPI](https://pokeapi.co/):

```
GET https://pokeapi.co/api/v2/pokemon/?offset=20&limit=100
```

For each of the 100 Pokémon in that list, the page also requests its `/pokemon/{id}` record (types, stats,
abilities, height, weight, artwork, animated 3D sprites) and its `/pokemon-species/{id}` record
(category, Pokédex description, habitat, catch rate, what it evolves from).

## Features

- Search by name or number, filter by type, sort by number, name, base stat total, weight, height or speed
- Card backgrounds use both type colours for dual-type Pokémon
- Detail panel with artwork, description, facts, base stats on the 0–255 scale and abilities
- Small animated 3D model with buttons to turn it around and show the shiny colours
- Works on phones (the detail panel slides up from the bottom) and in light or dark mode

## Files

| File | What it is |
|---|---|
| `index.html` | The page: layout, styles and the code that calls PokeAPI |
| `data.js` | A saved copy of the same PokeAPI data, shown first and used if the API can't be reached |
| `sprites/` | Saved copies of the artwork and 3D sprites used with `data.js` |

Live data from PokeAPI is kept in the browser for 24 hours so the page doesn't repeat the 201 requests on every visit.

## Run it

Open `index.html` in a browser, or visit the GitHub Pages site for this repository.

Pokémon and its names are trademarks of Nintendo, Game Freak and Creatures. Fan-made, not affiliated.
