# golf-horse-sigbovik
These are "sanitized" versions of my submissions to the Sigbovik Golf Horse competition (http://golf.horse/sigbovik/). "Sanitized" means I have changed the string containing compressed data, as well as the multiplier of 9.1, so as to not reveal my best solution. auroch_sanitized.js still solves the problem, but the compressed data is much larger than my submissions. Please see my article https://www.luke-g.com/sigbovik-golf-horse/ for a detailed description how my programs work.

My submissions are as follows:
* auroch: 564 bytes
* auroch_v2: 561 bytes, using the same code as the original auroch, but encoder improvements that found a better multiplier and compressed data
* auroch_v3: 559 bytes. Replaced "^=" with "=" to save one byte, and further encoder improvements that saved another byte of compressed data
* auroch_v4: 556 bytes. Replaced the loop termination condition to save three bytes
