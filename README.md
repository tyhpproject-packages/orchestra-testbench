<!-- tyhp-readme:start -->
# tyhpdef/orchestra-testbench

Tyhp type definitions for `orchestra/testbench` `11.2.0`.

```bash
composer require --dev tyhpdef/orchestra-testbench:11.2.0
```

This is a metapackage. Composer also installs `tyhpdef/orchestra-testbench-impl` (type files).
Require **this** name, not `tyhpdef/orchestra-testbench-impl`.

See https://tyhplang.com.

## Maintain `orchestra/testbench`? Ship the types yourself

If you are a Packagist maintainer of `orchestra/testbench`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/orchestra-testbench-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `orchestra/testbench` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/orchestra-testbench": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `orchestra/testbench` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `orchestra/testbench` with a real constraint,
   `"replace": { "tyhpdef/orchestra-testbench": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `orchestra/testbench` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/orchestra-testbench` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
