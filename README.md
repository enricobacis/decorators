# decorators
DECORATORS DECORATORS DECORATORS !!!

* **memo**:
  - `memo`: The classical *memoize* decorator. It keeps a cache arg -> result so you don't continue to perform the same computations.
  - `keymemo`: It allows to specify a `key` function that takes the `args` and `kwargs` of the decorated function and computes a `key` value to use as key in the cache dictionary. This way you can for example use a single value of a dictionary as key of the cache, or apply a function before passing something to the cache.
  - `classmemo`: The classical *memoize* decorator that can be applied to class functions. It keeps a cache arg -> result so you don't continue to perform the same computations. The cache is kept in the class namespace.
  - `classkeymemo`: Works like a combination of `classmemo` and `keymemo`, so it allows to specify a function that generate the cache key based on the function arguments and can be applied to class functions.
