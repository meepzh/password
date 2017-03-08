A memorable password generator for Node.js
==========================================

`password` is a simple server-side memorable password generator for Node.js

It is based on a list of 1,296 English words, thereby providing about 10 bits of randomness per word. A useful password will therefore require at least 3 words.

The module returns a function which can be called with the desired number of words.

    var password = require('password');
    console.log(password(4));

You can also access the list of words:

    var words = require('password').wordlist;
    console.log(words[352]);

Wordlist from [Short Wordlist for Passphrases #1](https://www.eff.org/document/eff-short-wordlist-passphrases-1) by the [EFF](https://www.eff.org/), used under [CC BY 3.0 US](https://creativecommons.org/licenses/by/3.0/us/). The words have been extracted into a JSON file.

[![Build Status](https://travis-ci.org/meepzh/password.svg?branch=eff-short)](https://travis-ci.org/meepzh/password)
