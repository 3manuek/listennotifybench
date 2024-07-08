# ApplyMyPatch

NOTE: this is going to potentially be in its own repository,
as it was thought for any set of patches, not exclusively the
one in this repository.



## Build

```earthly
earthly --interactive --no-satellite +build-all
earthly --no-satellite --disable-remote-registry-proxy --interactive ./src/postgres+build-w-patch
```

About `--disable-remote-registry-proxy`, see [Earthly issue 3736](https://github.com/earthly/earthly/issues/3736#issuecomment-1906786044).

## Applying patches

Inside the `patches` folder, name your patch and pass its name through the `PATCH` 
argument.

