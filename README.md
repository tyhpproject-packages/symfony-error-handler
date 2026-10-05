<!-- tyhp-readme:start -->
# tyhpdef/symfony-error-handler

Tyhp type definitions for `symfony/error-handler` `7.4.17`.

```bash
composer require --dev tyhpdef/symfony-error-handler:7.4.17
```

This is a metapackage. Composer also installs `tyhpdef/symfony-error-handler-impl` (type files).
Require **this** name, not `tyhpdef/symfony-error-handler-impl`.

See https://tyhplang.com.

## Maintain `symfony/error-handler`? Ship the types yourself

If you are a Packagist maintainer of `symfony/error-handler`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-error-handler-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/error-handler` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-error-handler": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/error-handler` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/error-handler` with a real constraint,
   `"replace": { "tyhpdef/symfony-error-handler": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/error-handler` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-error-handler` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
