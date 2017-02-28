Ataraxia Server @ Pokémon Showdown
========================================================================

Navigation: [Ataraxia][1] | [PS Server repository][10] | [PS Client repository][2] | [PS Dex repository][3]

  [1]: http://ataraxia.psim.us/
  [2]: https://github.com/Zarel/Pokemon-Showdown-Client
  [3]: https://github.com/Zarel/Pokemon-Showdown-Dex
  [10]: https://github.com/Zarel/Pokemon-Showdown


Introduction
------------------------------------------------------------------------

This is the source code for the Pokémon Showdown server [Ataraxia][4], a website for Pokémon battling. Pokémon Showdown simulates singles, doubles and triples battles in all the games out so far (Generations 1 through 7).

This repository contains the files needed to set up your own Pokémon Showdown server.

You can use your own computer as a server, but for other people to connect to your computer, you'll need to expose a port (default is 8000 but you can choose a different one) to connect to, which sometimes requires [port forwarding][5] (note that this isn't possible on certain internet connections).

  [4]: http://ataraxia.psim.us/
  [5]: http://en.wikipedia.org/wiki/Port_forwarding


Installing
------------------------------------------------------------------------

(Requires Node.js 6+)

Pokémon Showdown requires you to have [Node.js][6] installed, 6.x or later.

```bash
$ git clone https://github.com/Finnyfinfin/Ataraxia.git
cd spacialgaze && npm install
node app.js
```

  [6]: https://nodejs.org/

Configuring your server
------------------------------------------------------------------------

You will probably want to configure your servers settings to your liking.
Heres some of the configurations you can change in `config/config.js`

- port - The port to run the server on.

- serverIp - The ip of your server, used to parse custom avatars.

- tellrank - The minimum rank to use /tell for offline messaging.

Setting up an Administrator account
------------------------------------------------------------------------

Once your server is up, you probably want to make yourself an Administrator (~) on it.

### config/usergroups.csv

To become an Administrator, create a file named `config/usergroups.csv` containing

    USER,~

Replace `USER` with the username that you would like to become an Administrator. Do not put a space between the comma and the tilde.

This username must be registered. If you do not have a registered account, you can create one using the Register button in the settings menu (it looks like a gear) in the upper-right of Pokémon Showdown.

Once you're an administrator, you can promote/demote others easily with the `/globaladmin`, `/globalleader`, `/globalmod`, etc commands.

License
------------------------------------------------------------------------

Ataraxia's and Pokémon Showdown's server is distributed under the terms of the [MIT License][9].

  [9]: https://github.com/Finnyfinfin/Ataraxia/blob/master/LICENSE


Maintainers
------------------------------------------------------------------------

This server is brought to you and maintained by the following people:

Owner

[Finny](https://github.com/Finnyfinfin)

Contributor

[Top Doggo](https://github.com/KevinMech)


Special thanks

- [HoeenCoder](https://github.com/HoeenCoder) and [Mystifi](https://github.com/Mystifi)
- See http://pokemonshowdown.com/credits
