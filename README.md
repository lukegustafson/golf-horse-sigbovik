# golf-horse-sigbovik
These are "sanitized" versions of my submissions to the Sigbovik Golf Horse competition (http://golf.horse/sigbovik/). "Sanitized" means I have changed the string containing compressed data, as well as the multiplier of 9.1, so as to not reveal my best solution. auroch_sanitized.js, unlike the other JS files here, does solve the problem, but the compressed data is much larger than my submissions. Please see my article https://www.luke-g.com/sigbovik-golf-horse/ for a detailed description how my programs work.

My submissions are as follows:
* auroch: 564 bytes
* auroch_v2: 561 bytes, using the same code as the original auroch, but encoder improvements that found a better multiplier and compressed data
* auroch_v3: 559 bytes. Replaced "^=" with "=" to save one byte, and further encoder improvements that saved another byte of compressed data
* auroch_v4: 556 bytes. Replaced the loop termination condition to save two bytes in expectation, plus a byte saved in compressed data due to luck
* auroch_v5: 553 bytes. Modified the hash slightly so it could be combined with the loop termination condition, saving 2 bytes of code. Enhanced the encoder to consider 4-byte characters and invalid UTF-8, saving another byte.
* auroch_v6: 550 bytes. Saved 7 bytes of code: 1 byte for handling newlines, 2 bytes for getting hexes, and 4 bytes for the hashing. Lost 4 bytes of compressed data: 1 byte needed for padding, about 1 byte from fewer degrees of freedom (especially, there's no longer a multiplier to search over), and about 2 bytes probably due to the lower-quality hash.
