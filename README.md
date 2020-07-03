# org.electrum.electrum

Flatpak build of [electrum](https://electrum.org/#home).

## Building

The `python3-requirements*` files are built
using
[these](https://github.com/spesmilo/electrum/tree/master/contrib/requirements)
requirements files,
and `flatpak-pip-generator` from
[flatpak-builder-tools](https://github.com/flatpak/flatpak-builder-tools/), with
a few modifications.


## User data

Wallets are located at `~/.var/app/org.electrum.electrum/.electrum`, to use
`~/.electrum` instead, give the app filesystem permissions

``` sh
flatpak override --filesystem=home org.electrum.electrum 
```
