*Block TEA (xxtea) Tiny Encryption Algorithm implementation in JavaScript as a Node module*

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

## Install

To install run `npm install git://github.com/devotis/node-tea#master`

Or add this to package.json

    "dependencies": {
        "tea": "git://github.com/devotis/node-tea#master"
    }
...and run `npm install`

## Attribution

The code of index.js is a complete copy paste of what you can find here by the original author http://www.movable-type.co.uk/scripts/tea-block.html

I have changed nothing except adding `module.exports = Tea;`


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
