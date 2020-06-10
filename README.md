# Generate C++ Module.

***gen_cc_mod*** is shell tool for generating C++ modules.

Developed in bash code: ***100%***.

The README is used to introduce the modules and provide instructions on
how to install the modules, any machine dependencies it may have and any
other information that should be provided before the modules are installed.

[![GitHub issues open](https://img.shields.io/github/issues/vroncevic/gen_cc_mod.svg)](https://github.com/vroncevic/gen_cc_mod/issues)
 [![GitHub contributors](https://img.shields.io/github/contributors/vroncevic/gen_cc_mod.svg)](https://github.com/vroncevic/gen_cc_mod/graphs/contributors)

<!-- START doctoc -->
**Table of Contents**

- [Installation](https://github.com/vroncevic/gen_cc_mod#installation)
- [Usage](https://github.com/vroncevic/gen_cc_mod#usage)
- [Dependencies](https://github.com/vroncevic/gen_cc_mod#dependencies)
- [Shell tool structure](https://github.com/vroncevic/gen_cc_mod#shell-tool-structure)
- [Docs](https://github.com/vroncevic/gen_cc_mod#docs)
- [Copyright and Licence](https://github.com/vroncevic/gen_cc_mod#copyright-and-licence)
<!-- END doctoc -->

### INSTALLATION

Navigate to release [page](https://github.com/vroncevic/gen_cc_mod/releases) download and extract release archive.

To install modules type the following:

```
tar xvzf gen_cc_mod-x.y.z.tar.gz
cd gen_cc_mod-x.y.z
cp -R ~/sh_tool/bin/   /root/scripts/gen_cc_mod/ver.1.0/
cp -R ~/sh_tool/conf/  /root/scripts/gen_cc_mod/ver.1.0/
cp -R ~/sh_tool/log/   /root/scripts/gen_cc_mod/ver.1.0/
```

![alt tag](https://raw.githubusercontent.com/vroncevic/gen_cc_mod/dev/docs/setup_tree.png)

Or You can use docker to create image/container.

### USAGE

```
# Create symlink for shell tool
ln -s /root/scripts/gen_cc_mod/ver.1.0/bin/gen_cc_mod.sh /root/bin/gen_cc_mod

# Setting PATH
export PATH=${PATH}:/root/bin/

# Generating module-pair (source+header file)
gen_cc_mod GTKMyOption
```

### DEPENDENCIES

This module requires these other modules and libraries:

* sh_util https://github.com/vroncevic/sh_util

### SHELL TOOL STRUCTURE

gen_cc_mod is based on MOP.

Shell tool structure:
```
.
├── bin
│   └── gen_cc_mod.sh
├── conf
│   ├── gen_cc_mod.cfg
│   ├── gen_cc_mod_util.cfg
│   └── template
│       ├── cc_editorconfig.template
│       ├── cc_source.template
│       └── h_header.template
└── log
    └── gen_cc_mod.log
```

### DOCS

[![Documentation Status](https://readthedocs.org/projects/gen_cc_mod/badge/?version=latest)](https://gen_cc_mod.readthedocs.io/projects/gen_cc_mod/en/latest/?badge=latest)

More documentation and info at:

* https://gen_cc_mod.readthedocs.io/en/latest/

### COPYRIGHT AND LICENCE

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Copyright (C) 2018 by https://vroncevic.github.io/gen_cc_mod

This tool is free software; you can redistribute it and/or modify
it under the same terms as Bash itself, either Bash version 4.2.47 or,
at your option, any later version of Bash 4 you may have available.

