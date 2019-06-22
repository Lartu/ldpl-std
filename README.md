# The LDPL Standard Library

![LDPLSTD Logo](https://raw.githubusercontent.com/Lartu/ldpl/master/images/tutorial-logo.png)

This repository contains the LDPL Standard Library, which contains many
useful statements for the
[LDPL Programming Language](https://github.com/lartu/ldpl) not included in the base language.

The library is organized in a series of `.ldpl` files called *briefcases*,
each containing new statements designed with to extend the functionality of LDPL in
particular areas. For example the
`brc_lists.ldpl` briefcase includes general LIST releated statements,
like `FLIP LIST` and `SORT LIST - ASCENDING`.

New statements and entire briefcases are welcome contributions,
corrections and feedback are most certainly welcome as well.

## How to use the LDPL Standard Library

Just download the briefcase you want and IMPORT it in your LDPL source file.
For example, if you want to include the file `std-lists.ldpl` you must add
the line

`IMPORT "/route/to/std-lists.ldpl"`

before the `DATA:` and `PROCEDURE:` sections.

**Note:** please bear in mind that at the moment the LDPL Standard Library only works with [this experimental LDPL branch](https://github.com/Lartu/ldpl/pull/124), so if by the time you read this that particular branch hasn't been merged into master, you'll have to
pull from it in order to use the library.

## Statements included in every briefcase

Every statement is documented in more detail in their own briefcase file.

- **brc_lists.ldpl** (`LIST` statements):
   - `DISPLAY LIST $`
   - `SORT LIST $ ASCENDING`
   - `SORT LIST $ DESCENDING`
   - `APPEND LIST $ TO LIST $`
   - `SPLICE ELEMENT $ OF LIST $`
   - `FLIP LIST $`

- **brc_math.ldpl** (mathematical statements):
   - `FIND SQUARE ROOT OF $ IN $`
   - `STORE PI IN $`

## License

LDPL is distributed under the GNU General Public License 3.0. All LDPL Dinosaur logos where created by [Lartu](https://github.com/Lartu) and are released under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.
