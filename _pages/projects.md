---
layout: archive
title: "Fun Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /projects
---

{% include base_path %}

Picross
------
I enjoy coding small games in my free time. To teach myself RShiny, I created a version of my favorite puzzle game, Picross.

[App hosted on Shinyapps](https://hbwaddel.shinyapps.io/Picross/) : [Github repository](https://github.com/hbwddl/rshiny-picross)

Shut the Box
------
This is another small game I coded in Rshiny. It's a one-player dice game.

[App hosted on Shinyapps](https://hbwaddel.shinyapps.io/Shut-the-Box/) : [Github repository](https://github.com/hbwddl/Shut-the-Box)

Pokemon Type Checking Utility
------
I've enjoyed playing Pokémon for a long time. I put together a utility where you can check Pokémon "type" effectiveness in Rshiny.

[App hosted on Shinyapps](https://hbwaddel.shinyapps.io/typechecker/) : [Github repository](https://github.com/hbwddl/PokemonTypeChecker)

woRdle()
------
Keeping up with the early 2022 zeitgeist by making a wordle clone in R: [Github repository](https://github.com/hbwddl/woRdle)

{% for post in site.posts reversed %}
  {% include archive-single.html %}
{% endfor %}
