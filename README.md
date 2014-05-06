*Block TEA (xxtea) Tiny Encryption Algorithm implementation in JavaScript as a Node module*

A complete copy paste of code from http://www.movable-type.co.uk/scripts/tea-block.html

## Install

To install run `npm install git://github.com/devotis/node-tea#master`

Or add this to package.json

    "dependencies": {
        "tea": "git://github.com/devotis/node-tea#master"
    }
...and run `npm install`

## Usage

```javascript
var tea = require('tea');

var clear     = 'string to be encrypted';
var password  = 'BH&^!   ljknca>":{L{}uuj~``BF';
var encrypted = tea.encrypt(clear,     password);
var decrypted = tea.decrypt(encrypted, password);

console.log(clear, encrypted, decrypted);
//--> 'string to be encrypted', 'xR4q8OXWSShGk/LYrCQNLWET1GtXooG3', 'string to be encrypted'
```

## Attribution
```javascript
/* - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  */
/*  Block TEA (xxtea) Tiny Encryption Algorithm implementation in JavaScript                      */
/*     (c) Chris Veness 2002-2012: www.movable-type.co.uk/tea-block.html                          */
/* - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  */

/* - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  */
/*  Algorithm: David Wheeler & Roger Needham, Cambridge University Computer Lab                   */
/*             http://www.cl.cam.ac.uk/ftp/papers/djw-rmn/djw-rmn-tea.html (1994)                 */
/*             http://www.cl.cam.ac.uk/ftp/users/djw3/xtea.ps (1997)                              */
/*             http://www.cl.cam.ac.uk/ftp/users/djw3/xxtea.ps (1998)                             */
/* - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  */
```
