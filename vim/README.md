# Vim

## Cursor
| Comando | Descripción |
| :-----------: | ----------- |
| `0` | Mover el cursor al principio de la línea. |
| `^` | Mover el cursor al primer carácter que no esté en blanco de la línea. |
| `$` | Mover el cursor al final de la línea. |
| `g_` | Mover el cursor al último carácter que no esté en blanco de la línea. |
| `gg` | Mover el cursor a la primera línea del documento. |
| `G` | Mover el cursor a la última línea del documento. |
| `{` | Mover el cursor al párrafo (función/bloque) anterior.  |
| `}` | Mover el cursor al párrafo (función/bloque) siguiente. |

## Modo inserción
| Comando | Descripción |
| :-----------: | ----------- |
| `i` | Insertar antes del cursor. |
| `a` | Insertar después del cursor. |
| `I` | Insertar al principio de la línea. |
| `A` | Insertar al final de la línea. |
| `o` | Insertar una nueva línea debajo de la línea actual. |
| `O` | Insertar una nueva línea encima de la línea actual. |
| `Esc` | Salir del modo inserción. |

## Copiar
| Comando | Descripción |
| :-----------: | ----------- |
| `yy` | Copiar la línea actual. |
| `[n]yy` | Copiar `n` líneas. |
| `yw` | Copiar la palabra actual desde el carácter en el que se encuentra el cursor, hasta el final de la palabra. |
| `yb` | Copiar la palabra actual desde el carácter en el que se encuentra el cursor, hasta el principio de la palabra. |
| `yiw` | Copiar la palabra en la que se encuentra el cursor. |
| `y$` | Copiar desde la posición actual del cursor, hasta el final de la línea. |

## Cortar
| Comando | Descripción |
| :-----------: | ----------- |
| `dd` | Cortar la línea actual. |
| `[n]dd` | Cortar `n` líneas. |
| `dw` | Cortar la palabra actual desde el carácter en el que se encuentra el cursor, hasta el final de la palabra. |
| `db` | Cortar la palabra actual desde el carácter en el que se encuentra el cursor, hasta el principio de la palabra. |
| `diw` | Cortar la palabra en la que se encuentra el cursor. |
| `d$` | Cortar desde la posición actual del cursor, hasta el final de la línea. |
| `x` | Cortar el carácter actual. |
| `X` | Cortar el carácter anterior. |

## Pegar
| Comando | Descripción |
| :-----------: | ----------- |
| `p` | Pegar el texto copiado después del cursor. |
| `P` | Pegar el texto copiado antes del cursor. |

## Edición
| Comando | Descripción |
| :-----------: | ----------- |
| `r` | Reemplazar un carácter. |
| `u` | Deshacer la última acción. |
| `Ctrl + r` | Rehacer la última acción. |

## Guardar y salir
| Comando | Descripción |
| :-----------: | ----------- |
| `:w` | Guardar el documento sin salir. |
| `:q` | Salir del documento. |
| `:wq` | Guardar el documento y salir. |
| `:q!` | Salir sin guardar los cambios en el documento. |

## Referencias
- [Vim Cheat Sheet ](https://vim.rtorr.com/)
- [Wrapping Text In Vim](https://vim.works/2019/03/16/wrapping-text-in-vim/)
- [Tab settings in Vim](https://arisweedler.medium.com/tab-settings-in-vim-1ea0863c5990)
- [Understanding ‘listchars’](https://medium.com/usevim/understanding-listchars-acb9e5a90854)
- [vimcolorschemes](https://vimcolorschemes.com/)