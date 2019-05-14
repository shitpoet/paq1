# PAQ1

Original source code of lossless data compressor PAQ1 by Matthew V. Mahoney.

PAQ1 is context mixing compressor, competitive with PPM. Main model of PAQ1 combines 8 nonstationary context models. Nonstationary models are fast adapting to changes in data source. PAQ1 also includes other models for long matches, texts and fixed records. 

The algorithm and its implementation are described in paper http://www.mattmahoney.net/dc/paq1.pdf.

See also Matt's page on his compression programs - https://cs.fit.edu/~mmahoney/compression/.

See also this <a href="https://www.youtube.com/watch?v=J5WX-wN_RKY">video</a> by Nathan Egge on usage of PAQ1(2/3?) in extreme x86 compression (and for short description of PAQ1-like algorithm).

See also comments in cpp file.

## Note on compilation on 64-bit Linux 

To get correct results on 64-bit OS it can be needed to change `typedef` on line 304:

```c++
//typedef unsigned long U32;
typedef unsigned int U32;
```

Because `U32` meant to be 32-bit integer, but `long` is usually 64-bit on 64-bit Linux.
    

## Licence 

Licence: GPL.
