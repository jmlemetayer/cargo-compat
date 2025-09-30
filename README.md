# `cargo-compat`

Quick and dirty solution to update dependencies compatible with a specified
toolchain.

```bash
$ cargo update
    Updating crates.io index
     Locking 20 packages to latest compatible versions
    Updating addr2line v0.24.2 -> v0.25.1
    Updating anstyle v1.0.11 -> v1.0.13
    Updating backtrace v0.3.75 -> v0.3.76
    Updating gimli v0.31.1 -> v0.32.3
      Adding hashbrown v0.16.0
    Updating memchr v2.7.5 -> v2.7.6
    Updating object v0.36.7 -> v0.37.3
    Updating pest v2.8.0 -> v2.8.2
    Updating pest_derive v2.8.0 -> v2.8.2
    Updating pest_generator v2.8.0 -> v2.8.2
    Updating pest_meta v2.8.0 -> v2.8.2
    Updating serde_spanned v1.0.1 -> v1.0.2
    Updating thiserror v2.0.16 -> v2.0.17
    Updating thiserror-impl v2.0.16 -> v2.0.17
    Updating toml v0.9.6 -> v0.9.7
    Updating toml_datetime v0.7.1 -> v0.7.2
    Updating toml_edit v0.23.5 -> v0.23.6
    Updating toml_parser v1.0.2 -> v1.0.3
    Removing windows-link v0.1.3
    Updating windows-sys v0.61.0 -> v0.61.1
    Updating windows-targets v0.53.3 -> v0.53.4
note: pass `--verbose` to see 1 unchanged dependencies behind latest
$ cargo compat 1.75.0
INFO: Checking build...
INFO: Updating crate pest_generator@2.8.2 to 2.8.0
INFO: Updating crate pest_derive@2.8.2 to 2.8.0
INFO: Checking build...
INFO: Updating crate toml_edit@0.23.6 to 0.23.5
INFO: Checking build...
INFO: Updating crate toml_parser@1.0.3 to 1.0.2
INFO: Updating crate toml@0.9.7 to 0.9.6
INFO: Checking build...
INFO: Updating crate toml_parser@1.0.3 to 1.0.2
INFO: Checking build...
INFO: Updating crate pest_generator@2.8.2 to 2.8.0
INFO: Checking build...
INFO: Updating crate toml_datetime@0.7.2 to 0.7.1
INFO: Checking build...
INFO: Updating crate pest@2.8.2 to 2.8.0
INFO: Updating crate pest_meta@2.8.2 to 2.8.0
INFO: Checking build...
INFO: Updating crate pest@2.8.2 to 2.8.0
INFO: Checking build...
INFO: Updating crate serde_spanned@1.0.2 to 1.0.1
INFO: Checking build...
INFO: Done
```

> [!NOTE]
> One day I'll do it in rust, I promise!

## License

The `cargo-compat` script is released under the [MIT License](LICENSE.md).
