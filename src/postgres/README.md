# ApplyMyPatch

NOTE: this is going to potentially be in its own repository,
as it was thought for any set of patches, not exclusively the
one in this repository.



## Build

```earthly
earthly --interactive --no-satellite +build-all
earthly --no-satellite --interactive ./src/postgres+build-w-patch
```


## Applying patches

Inside the `patches` folder, name your patch and pass its name through the `PATCH` 
argument.

