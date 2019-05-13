# PAQ1

Original source code of lossless data compressor PAQ1 by Matthew V. Mahoney.

PAQ1 is context mixing compressor, competitive with PPM. Main model of PAQ1 combines 8 nonstationary context models. Nonstationary models are fast adapting to changes in data source. PAQ1 also includes other models for long matches, texts and fixed records. 

The algorithm and its implementation are described in paper http://www.mattmahoney.net/dc/paq1.pdf.

See also Matt's page on his compression programs - https://cs.fit.edu/~mmahoney/compression/.

See also this <a href="https://www.youtube.com/watch?v=J5WX-wN_RKY">video</a> by Nathan Egge on usage of PAQ1(2/3?) in extreme x86 compression (and for short description of PAQ1-like algorithm).

See also comments in cpp file.

License: GPL.
