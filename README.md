<!-- tyhp-readme:start -->
# tyhpdef/guzzlehttp-guzzle

Tyhp type definitions for `guzzlehttp/guzzle` `8.2.0`.

```bash
composer require --dev tyhpdef/guzzlehttp-guzzle:8.2.0
```

This is a metapackage. Composer also installs `tyhpdef/guzzlehttp-guzzle-impl` (type files).
Require **this** name, not `tyhpdef/guzzlehttp-guzzle-impl`.

See https://tyhplang.com.

## Maintain `guzzlehttp/guzzle`? Ship the types yourself

If you are a Packagist maintainer of `guzzlehttp/guzzle`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/guzzlehttp-guzzle-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `guzzlehttp/guzzle` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/guzzlehttp-guzzle": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `guzzlehttp/guzzle` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `guzzlehttp/guzzle` with a real constraint,
   `"replace": { "tyhpdef/guzzlehttp-guzzle": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `guzzlehttp/guzzle` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/guzzlehttp-guzzle` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
