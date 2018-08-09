# The Mersenne Twister Pseudo Random Number Generator

This is a mirror of my library hosted at https://create.stephan-brumme.com/mersenne-twister/

The [Mersenne Twister](http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt.html) is often regarded as the fastest pseudo-random number generator which passes almost all statistical tests.

The [original C code](https://create.stephan-brumme.com/mersenne-twister/original.c) isn't exactly beautiful, therefore I decided to write my own C++ class.
`.h` plus `.cpp` file are under 100 lines even though there are tons of comments.

Basic usage:
``` cpp
#include "mersenne.h"
...
// create new Mersenne Twister
MersenneTwister prng(123456);
// generate two random 32-bit numbers
int x = prng();
int y = prng(); 
```

And for the fun of it, I converted the C++ code to Javascript and added two [live demos](https://create.stephan-brumme.com/mersenne-twister/), too.
