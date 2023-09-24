# LumberImage Commands

LumberImage is a tool for creating and manipulating images using various commands.

## General Commands

- `/#clear`: Close the menu when you're done reading.

## Setting Commands

Setting commands start with "s" as the first command indicator, followed by the specific setting.

- `s§z§[number]§`: Set the size. Example: `s§z§5§;`
- `s§b§[number]§;`: Change brightness. Example: `s§b§50§;`
- `s§col§[number]§;`: Change color.
- `s§sat§[number]§;`: Change saturation.
- `s§h§[hex_color]§`: Set the color using hex values. Example: `s§h§ff0000§;`

## Drawing Commands

Drawing commands are used to create shapes and lines.

- `d§l§x1§y1§x2§y2§`: Draw a line. Example: `d§l§0§0§100§100§;`
- `d§d§x§y§`: Draw a dot. Example: `d§d§50§50§;`
- `d§c§x§y§z§`: Draw a circle. Example: `d§c§100§100§50§;`
- `l§q§x§y§`: Continue a line from the previous position. Example: `l§q§50§50§;`

## File Loading Commands

- `load.ign example x y z`: Load other IGN files from your files. Example: `load.ign example 100 0 0;`

These commands can be used in LumberImage to create and manipulate images. Remember to use the specified separators and indicators to ensure proper execution of commands.
