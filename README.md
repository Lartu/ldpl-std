# The LDPL Standard Library

![LDPLSTD Logo](https://raw.githubusercontent.com/Lartu/ldpl/master/images/tutorial-logo.png)

This repository contains the LDPL Standard Library, which contains many
useful SUB-PROCEDURES for the
[LDPL Programming Language](https://github.com/lartu/ldpl).

The library is organized in a series of `.ldpl` files (*briefcases*),
each containing
SUB-PROCEDURES designed with a certain context in mind. For example the
`std-lists.ldpl` briefcase includes general LIST releated SUB-PROCEDURES,
like reversing a list or sorting its elements.

New SUB-PROCEDURES and entire briefcases are welcome contributions,
corrections and feedback are most certainly welcome as well.

## How to use the LDPL Standard Library

Just download the briefcase you want and IMPORT it in your LDPL source file.
For example, if you want to include the file `std-lists.ldpl` you must add
the line

`IMPORT "/route/to/std-lists.ldpl"`

before the `DATA:` and `PROCEDURE:` sections.

**Note:** please bear in mind that at the moment the LDPL Standard Library only works with [this experimental LDPL branch](https://github.com/Lartu/ldpl/pull/124), so if by the time you read this that particular branch hasn't been merged into master, you'll have to
pull from it in order to use the library.

## License

LDPL is distributed under the GNU General Public License 3.0. All LDPL Dinosaur logos are released under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.
