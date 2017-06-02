This is the beginnings of a TTR implementation in Python 3.4.3.  Run
the examples in the files example-records.py and example-types.py

This implementation covers a core of TTR, including:
     Basic types
     Ptypes (types constructed with predicates and their arguments)
     Meet (intersection) types
     Join (union) types
     Function types
     List types
     Record types
     String types
     Judging (assigning objects to types)
     Querying (asking whether an object is of a type)
     Adding witness conditions to types
     Creating objects of types
     Subtyping
     Type merging (including asymmetric type merging)
     Possibilities (types may have different witnesses in different
     		   possibilities)
     
  
7th April 2017

The query method in ttrtypes will now add an object to the witness_cache that it
computes as a witness on the basis of the witness conditions.

Rudimentary support for projections from ttr variables in ttrtypes: lazy objects
like LazyObj(['r','.','x'])

Added in_poss method to functions in ttrtypes to restrict the domain type to a
given possibility

Judging an object to be of a meet type (ttrtypes) will now judge that object to
be of the two component types of the meet type. 

A preliminary implementation of neural TTR has been added (neurons, nu, example-neurons, example-nu) together with a Jupiter notebook which is partially developed corresponding to example-nu (nu.ipynb). 
     

2nd June 2017

Fixed bug with Possibility in ttrtypes.py
Improved show-method for possibilities

Changed subst and eval methods for LazyObj so that left recursive lazy
objects will be correctly evaluated.

A preliminary jupyter notebook (lspc.ipynb) has been added with
examples from the paper Interfacing Language, Spatial Perception and
Cognition in Type Theory with Records by Simon Dobnik and Robin Cooper
(to appear in Journal of Language Modelling).

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org:/repo/gu-clasp/pyttr)
