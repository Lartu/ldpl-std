![The LDPL Standard Library](images/logo-readme.png)

# The LDPL Standard Library
This repository contains the LDPL Standard Library, a collection of
LDPL libraries that contain many useful pre-written statements for the
[LDPL Programming Language](https://github.com/lartu/ldpl)
that are not included in the base language.

The library is organized in a series of `.ldpl` files lovingly called *briefcases*
(this is a very serious language, you know, we have ties) each containing new statements
designed to extend the functionality of LDPL in many areas. In simpler terms, designed
to make your life as an LDPL programmer easier. For example the `brc_lists.ldpl` briefcase
includes many statements designed for working with LIST values, like `FLIP LIST` and `SORT LIST - ASCENDING`.

New statements and entire briefcases are very welcome contributions,
corrections and feedback are most certainly welcome as well.

## How to use the LDPL Standard Library

Most of the time you won't need the entire Standard Library for a single project,
so you can just get the briefcases you are going to use. You can do this **by hand**
or **using [LPM](https://github.com/lartu/lpm)** (the LDPL Package Manager).

### 📦 Installing a briefcase using LPM

Open a terminal and write `lpm install <briefcase-name>` to install the desired briefcase.
Available briefcases are `std-list` (list statements), `std-math` (math statements),
`std-text` (text statements), `std-os` (operating system functions) and `std-random` (random
number generation and statements).

For example: `lpm install std-random`.

To include the downloaded briefcase in your project add the line `USING PACKAGE <briefcase-name>`
before the `DATA:` and `PROCEDURE:` sections.

For example: `USING PACKAGE std-random`.

### ✋🏻 Installing a briefcase by hand

Just download the briefcase you want and include it in your LDPL source file.
For example, if you want to include the file `std-lists.ldpl` you should add
the line

`INCLUDE "/route/to/std-lists.ldpl"`

before the `DATA:` and `PROCEDURE:` sections.

## Statements included in each briefcase

Every statement is documented in more detail within its own briefcase file.

- **std-list.ldpl** (`LIST` statements):
   - `DISPLAY LIST $`
   - `SORT LIST $ ASCENDING`
   - `SORT LIST $ DESCENDING`
   - `APPEND LIST $ TO LIST $`
   - `SPLICE ELEMENT $ OF LIST $`
   - `FLIP LIST $`

- **std-math.ldpl** (mathematical statements):
   - `FIND SQUARE ROOT OF $ IN $`
   - `PI` constant

- **std-random.ldpl** (random statements):
   - `GET RANDOM BETWEEN $ AND $ IN $`
   - `GET RANDOM INTEGER BETWEEN $ AND $ IN $`
   - `GET RANDOM ELEMENT FROM LIST $ IN $`
   - `SHUFFLE LIST $`
   
 - **std-os.ldpl** (operating system statements):
   - `LIST CONTENTS OF DIRECTORY $ IN $`
   - `GET CURRENT DAY IN $`
   - `GET CURRENT MONTH IN $`
   - `GET CURRENT YEAR IN $`
   - `GET CURRENT TIME IN $ $ $`
   
 - **std-text.ldpl** (text statements):
   - `SHIFT $ TO LOWER CASE IN $`
   - `SHIFT $ TO UPPER CASE IN $`
   - `SHIFT $ TO PROPER IN $`

## License

The LDPL Standard Library is distributed under the MIT License. LDPL is distributed under the GNU General Public License 3.0. All LDPL Dinosaur logos where created by [Lartu](https://github.com/Lartu) and are released under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.
