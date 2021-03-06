![Arganium](/artwork/arganium%20logo.png?raw=true "Arganium")

Arganium is a cooperative hacking shooter.  It blends old-school first person shooting and modern hacker CTF.  In this repo you'll find everything you need to get started playing, building, and modifying Arganium.  More extensive information on the gameplay, design, and components is located in the [wiki](https://github.com/frozenfoxx/arganium/wiki).

# Layout
* __artwork:__ various artwork related to the project.
* __assets:__ all game assets created for Arganium.  This directory is the source for the *arganium.pk3* archive that's used to launch Arganium.
* __certain:__ contains the Zandronum wrapper Certain which allows control of a Zandronum game server.
* __gloom:__ contains the Rails-based web interface *Gloom* which Arganium uses to interact with Certain.
* __levels:__ submitted levels for Arganium.  These all have to follow the conventions in the documentation but are otherwise ready to play.

# Requirements
* [Bootstrap](http://getbootstrap.com) 3
* [Rails](http://rubyonrails.org) 5.0+
* [Ruby](https://www.ruby-lang.org) 2.0+
* [Zandronum](https://zandronum.com/) 3.0+

# How to Play
* Clone this repository
* Configure system according to the [Development Environment](https://github.com/frozenfoxx/arganium/wiki/Development-Environment) guide.
* Place all desired challenges in the `challenges` directory and place desired levels in the `levels` directories.
* Change into the Gloom directory.
* Run `./setup` to configure your game
 * Alternatively place a YML configuration file in the Gloom directory.
* Run `./setup <configname>.yml` to set up the Rails server.
* Run `rails server` to start the server.
* Have Control team players connect to *http://\<server socket\>/* with their web browsers.
* Have Marine team players connect to the Zandronum server with the appropriate *level wad* (supplied in `levels` directory) and *arganium.pk3* (supplied in the `assets` directory).
* The game is live!  Gameplay is detailed in the [wiki](https://github.com/frozenfoxx/arganium/wiki/Gameplay).

# Community
* [Freenode](https://freenode.net/) IRC chatroom:  #arganium

# Legal
Arganium is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. Arganium is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
