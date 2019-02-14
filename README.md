# Sniper-cache-controller-class-C++
Defines classes and methods to control access to multiple levels of cache memory in a multi-core computing system.

Header file:-
Defines class CacheController and prototypes for various methods that will control cache operations.

Main file:-
Implements all the methods defined in header file. Following is a high level overview of these methods-
1] Core-interfacing stuff- 
    accessCache()--> function to access private/level 1 caches  
    operationPermissibleinCache() --> function to check cache hit/miss
    copyDataFromNextLevel() --> fucntion to fetch data from next (lower level) cache in case of miss in current level
2] Cache meta-data operations-
    getCacheBlockInfo() --> returns pointer to a particular cache block, NULL if the block is absent 
3] Cache data operations-
    retrieveCacheBlock() --> read data from a cache block
    insertCacheBlock() --> insert cache block in 'this' cache 
    updateCacheBlock() --> update data in 'this' cache block
    
