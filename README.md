# Terraria on your own tShock Server in Docker (with some usefull PlugIns)

Let's play [Terraria](http://terraria.org/) with [docker](https://www.docker.com/) on your own [tShock](https://tshock.co) Server with some usefull PlugIns. ;-)

**Feel free to use it directly or fork it for you own server configuration**

The project itself is licensed under the [Apache 2.0][] and the [CC-BY 4.0][] licenses (see [Copyright and Licenses](#copyright-and-licenses) for more informations).

Contributions [welcome](#contributing).

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


## Plugins

### Permabuffs

- https://tshock.co/xf/index.php?resources/permabuffs.5/

### GHOST PLUGIN (VANISH) 1.1

- https://tshock.co/xf/index.php?resources/ghost-plugin-vanish.217/
- https://github.com/DannyDan77/Ghost



### House Regions Plugin

- https://tshock.co/xf/index.php?resources/house-regions.191/

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
