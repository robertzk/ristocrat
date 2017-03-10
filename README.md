# Ristocrat - better, richer REPL for R

Ristocrat (pronounced "*arr*istocrat") will be a better, richer REPL for R, that 

  * Easier editing of R commands and history using [ed-like](https://github.com/robertzk/productivus/blob/master/R/ed.r) history
    traversal and an editor of your choice (like vim).

  * Color-coded console input and output, which should allow for clearer and faster
    inspection of code.

  * Smart pasting capabilities, preventing R expressions such as

    ```r
    if (blah) 1
    else 2
    ```
    
    from causing errors due to sequential line interpretation.

  * Integration with a background Docker service that is much smarter about 
    maintaining an in-memory cache of your data than [RData files](https://stat.ethz.ch/R-manual/R-devel/library/base/html/load.html),
    and will allow for (probably immutable read-only) shared memory between Ristrocrat
    sessions.

