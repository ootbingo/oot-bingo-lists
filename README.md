# OoT Bingo Lists

![image](https://img.shields.io/npm/v/oot-bingo-lists)

Provides the bingo goal lists of various Ocarina of Time Bingo versions.

## Install

```
npm install --save oot-bingo-lists
```

## Supported bingo versions

* `v9.1`
* `v9.2`
* `v9.3`
* `v9.4`
* `v9.5`
* `v9.5.1`
* `v10.0`
* `v10.1`

## Usage

Use the `getBingoList()` function to retrieve the bingo list of a specific bingo version:

```ts
import { getBingoList } from "oot-bingo-lists";

const bingoList = getBingoList("v10.1");
```

### Generator

With the [OoT Bingo Generator](https://github.com/xwmtp/oot-bingo-generator) (`npm install --save oot-bingo-generator`),
these bingo lists can be used to generate boards:

```ts
import { getBingoList } from "oot-bingo-lists";
import { generateBingoBoard } from "oot-bingo-generator";

const bingoList = getBingoList("v10.1");
const board = generateBingoBoard(bingoList, "blackout", 654321);
```

### Latest version

Get the latest bingo list:

```ts
import { getBingoList, latestBingoVersion } from "oot-bingo-lists";

const bingoList = getBingoList(latestBingoVersion);
```