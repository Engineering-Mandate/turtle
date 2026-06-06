# TURTLE.EXE

A Logo-style turtle graphics interpreter dressed up as a Windows 95 application.

**[▶ Live demo](https://engineering-mandate.github.io/turtle/)**

![screenshot placeholder](https://via.placeholder.com/600x400?text=TURTLE.EXE)

## Usage

Type commands in the editor and press **Run** (or `Ctrl+Enter`).

| Command | Effect |
|---|---|
| `fd n` | Forward *n* steps |
| `bk n` | Back *n* steps |
| `rt d` | Turn right *d* degrees |
| `lt d` | Turn left *d* degrees |
| `pu` / `pd` | Pen up / pen down |
| `home` | Return to centre |
| `cs` | Clear screen |
| `setpc colour` | Set pen colour (e.g. `red`, `#ff0000`) |
| `setpw n` | Set pen width |
| `repeat n [ ... ]` | Loop a block *n* times |

Comments start with `;`. Blocks nest freely.

```logo
; Rotating squares
repeat 36 [
  repeat 4 [fd 50 rt 90]
  rt 10
]
```

Six presets are included (Square, Triangle, Star, Flower, Petals, Sunburst). Use the **Speed** slider to slow the animation down or crank it up.

## Keyboard shortcuts

| Key | Action |
|---|---|
| `Ctrl+Enter` | Run |
| `Alt+R` | Run |
| `Alt+S` | Stop |
| `Alt+C` | Clear |
| `Tab` / `Shift+Tab` | Indent / outdent |

## Implementation

Single self-contained `index.html` — no build step, no dependencies.
