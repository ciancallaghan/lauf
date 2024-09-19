# Lauf

File-Manager inspired by [walk](https://github.com/antonmedv/walk) and [fff](https://github.com/dylanaraps/fff).

# Keybindings

| Keybinding | Description |
| ---------- | ----------- |
| j | Move down |
| k | Move up |
| g | Go to top of list |
| G | Go to bottom of list |
| C-d | Move down 5 items |
| C-u | Move up 5 items |
| h | Go up a directory |
| l | Enter a directory or open the file in `$EDITOR` |
| ~ | Go to `$HOME` |
| . | Toggle hidden directories |
| q | Quit |

## cd on exit

Add following to shell rc-file:

```sh
lf() {
    lauf
    cd "$(cat ${XDG_CACHE_HOME:-$HOME/.cache}/.lauf_d)"
}
```
