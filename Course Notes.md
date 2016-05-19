Reproducible Research
=====================

Week 3
------

### Communicating Results

`sessionInfo()`.  Awesome.  Lists everything useful about your environment.

`set.seed()`  Always make sure to do this.

 

`cacher` package.

Evaluates code written in files and stores intermediate results in a key-value
database.  R expressions are given SHA-1 hash values so that changes can be
tracked and code reevaluated if necessary.

“Cacher packages” can be built for distribution.

Other can “clone” an analysis and evaluate subsets of code or inspect data
objects.

 

Local directories are created, source code files and metadata are downloaded,
data objects are NOT downloaded by default.  References to data objects are
loaded and corresponding data can be lazy-loaded on demand.

 

`objbectcode(”data”)` grabs the code and shows you the trackback.

 

`runcode()` executes the code.

 

`checkcode()` evaluates all expressions form scratch.  Results from the
evaluation are checked against stored results to see if the results are the same
as what the author calculated. *Setting RNG seeds is critical for this to work*.

`checkobjects()` can check the integrity of data objects to check for possible
corruption.

 
