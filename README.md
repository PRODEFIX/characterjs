# CharacterJS
## Installation
```console
$ npm install characterjs
```

## Usage
```js
const character = require("characterjs");

character.normalize("๐ฝ๐๐กโ๐ผโโ๐ฉE ๐ ๐"); // "NORMALIZE COOL ๐"
character.normalize("๐ฝ๐๐กโ๐ผโโ๐ฉE ๐ ๐", true); // "NORMALIZE COOL"

character.emojify("Emojify'"); // "๐ช๐ฒ๐ด๐ฏ๐ฎ๐ซ๐พ'"
character.emojify("Emojify'", true); // "๐ช๐ฒ๐ด๐ฏ๐ฎ๐ซ๐พ"

character.tinyText("Tiny text'"); // "แตแถฆโฟสธ แตแตหฃแต'"
character.tinyText("Tiny text'", true); // "แตแถฆโฟสธ แตแตหฃแต"

character.reverse("Reverse'"); // "ษนวสวษนsว'"
character.reverse("Reverse'", true); // "'วsษนวสวษน"
character.reverse("Reverse'", false, true); // "ษนวสวษนsว"

character.ascii("Ascii", "NoText"); // "Ascii" or "NoText" in ascii

/*   _             _ _
    / \   ___  ___(_|_)
   / _ \ / __|/ __| | |
  / ___ \\__ \ (__| | |
 /_/   \_\___/\___|_|_|
*/

character.startUpper("A text of test"); // A Text Of Test
character.toggleCase("A TEXT of test"); // a text OF TEST
character.wordCount("A text of test"); // 4
character.sentenceCount("A text of test. A text of test"); // 2
character.emojiCount("A text of test ๐"); // 1
```