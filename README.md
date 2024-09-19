# Lauf

File-Manager inspired by [walk](https://github.com/antonmedv/walk) and [fff](https://github.com/dylanaraps/fff).

## cd on exit

Add following to shell rc-file:

```sh
lf() {
    lauf
    cd "$(cat ${XDG_CACHE_HOME:-$HOME/.cache}/.lauf_d)"
}
```
