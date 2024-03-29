# Terraria with usefull PlugIns on your own tShock Server

Let's play [Terraria](http://terraria.org/) with some usefull Plugins on your own [tShock](https://tshock.co) (served by [docker](https://www.docker.com/). ;-)

**Feel free to use it directly or fork it for you own server configuration**

The project itself is licensed under the [Apache 2.0][] and the [CC-BY 4.0][] licenses (see [Copyright and Licenses](#copyright-and-licenses) for more informations).

Contributions [welcome](#contributing).

## Overview

![licence](https://img.shields.io/badge/licence-Apache%202.0-blue.svg)
![tshock version](https://img.shields.io/badge/tshock-v4.3.26-green.svg)
![terraria api version](https://img.shields.io/badge/TerrariaAPI-2.1-lightgrey.svg)
![terraria version](https://img.shields.io/badge/terraria-1.3.5.3-brightgreen.svg)

## Table of contents

* [Motivation](#motivation)
* [Quick start](#quick-start)
* [Versioning](#versioning)
* [Issues](#issues)
* [Contributing](#contributing)
* [Authors](#authors)
* [Copyright and Licenses](#copyright-and-licenses)

## Motivation

**I don't wanted to reinvent the wheel with every new repository I create**,
so I use this template as a common starting point for my projects.

## Quick start

Clone this repo or get the `docker-compose` file from this repo:

````
mkdir tshock
cd tshock

curl -O https://raw.githubusercontent.com/kuetemeier/docker-tshock/master/docker-compose.yml

docker-compose up
````

Data will be saved to the volume defined in `docker-compose.yml` (default: `$HOME/.local/share/Terraria`).

## Plugins

### Permabuffs

- https://tshock.co/xf/index.php?resources/permabuffs.5/

### GHOST PLUGIN (VANISH) 1.1

#### Description

"A plugin that allows admins to become invisible and undetectable on command. While in ghost mode, admins don't appear on the player list, in the player count, they can chat, use commands, see others, and whisper other players."

#### Commands

````
/ghost
````

#### Links

- https://tshock.co/xf/index.php?resources/ghost-plugin-vanish.217/
- https://github.com/DannyDan77/Ghost

### House Regions Plugin

#### Description

This plugin provides players on TShock driven Terraria servers the possibility of defining houses in which other players can not alter any tiles. It accomplishes this by utilizing TShock's region system, i.e. this plugin simply wraps the region system functionality with an easy to use and more restricted interface designed for regular users.

For quick usage and for the sake of usabilitiy house regions are kept entirely unnamed, when being defined two points to mark the region boundaries are sufficient. To change parameters of a house region later, like adding shared players or groups, the player must simply stand in the region they want to change and execute the related house commands. The maximum amount of house regions per user, several size restrictions, and whether house regions can overlap with regular TShock regions can be configured.

Warning: TShock regions defined through this plugin are named in the format "*H_User:HouseIndex" thus, if you manually define a TShock region with this name format, this plugin will treat the region just like a house.

#### Commands

````
/house
/house commands
/house summary
/house info
/house define
/house resize <up|down|left|right> <amount>
/house share <user>
/house unshare <user>
/house shareGroup <group>
/house unshareGroup <group>
/house delete
/house scan
/house reloadconfig
````
To get more information about a command type /<command> help ingame.

#### Permissions

````
houseregions.define Can define new or resize existing houses.
houseregions.delete Can delete existing houses.
houseregions.share Can share houses.
houseregions.sharewithgroups Can share houses with TShock groups.
houseregions.nolimits Can define houses without a maximum limit or size restrictions.
houseregions.housingmaster Can display a list of all house owners. Can change settings of any house, either owned or not owned.
houseregions.cfg Can reload the configuration file.
````

#### Links


- https://tshock.co/xf/index.php?resources/house-regions.191/


## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, this project is maintained under [the Semantic Versioning guidelines](http://semver.org/). Sometimes we screw up, but we'll adhere to those rules whenever possible.

See [the Releases section of our GitHub project](https://github.com/kuetemeier/project-template/releases) for changelogs for each release version.

## Issues

Please report any bugs or requests that you have using the GitHub issue tracker!

## Contributing

**Contributions Welcome!**

Please read through our [contributing guidelines](./CONTRIBUTING.md). Included are directions for opening issues, coding standards, and notes on development.

Editor preferences are available in the editor config for easy use in common text editors. Read more and download plugins at http://editorconfig.org.

## Authors

**Jörg Kütemeier**

* <https://twitter.com/kuetemeier>
* <https://github.com/kuetemeier>

### Inspired by

This project would not be possible with the great work form the TShock Server team, docker and the inspirations from 
[amonetta](https://github.com/amonetta/tshock/) and [kalhartt](https://github.com/kalhartt/docker-tshock). Thank you, very much!

## Copyright and Licenses

### Apache License 2.0

Copyright 2016-2019 - Jörg Kütemeier - https://kuetemeier.de

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   <http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

### Documentations under CC-BY

Documentations in the `doc` folder released under Creative Commons - [CC-BY 4.0][]

### External libraries and software

All files located in the `lib` and `external` directories (if present)
are externally maintained libraries used by this software which have their own
licenses; we recommend you read them, as their terms may differ from the
terms above.

[Jörg Kütemeier]: https://kuetemeier.de/	"Jörg Kütemeier"
[CC-BY 4.0]: http://creativecommons.org/licenses/by/4.0/	"Creative Commons Attribution 4.0 International (CC BY 4.0)"
[Apache 2.0]: http://www.apache.org/licenses/LICENSE-2.0
