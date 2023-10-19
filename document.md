
# Lumberscript Commands

Lumberscript is a scripting language for controlling various aspects of pen, text display, file loading, conditional statements, loops, and Discord integration.

## Pen Commands

### Pen Settings
- `pen.col #`: Change the pen color on a scale from -100 to 100. Example: `pen.col 50 ;`
- `pen.sat #`: Change pen saturation. Preferably set to 0 for grayscale. Example: `pen.sat 0 ;`
- `pen.bri #`: Change pen brightness. Typically used as 0 or 100. Example: `pen.bri 100 ;`
- `pen.siz #`: Change pen size. Example: `pen.siz 5 ;`
- `pen.erease`: Erase the screen. Example: `pen.erease ;`
- `pen.hex ffffff`: Change pen color based on a hex value. Example: `pen.hex ffffff ;`

## Trace Commands

### Trace a Pen Shape
- `trc.lin x1 y1 x2 y2`: Draw a line. Example: `trc.lin 0 0 100 100 ;`
- `trc.dot x y`: Draw a dot. Example: `trc.dot 50 50 ;`

## Wait Command
- `wait #`: Wait for a specified time in seconds. Example: `wait 2 ;`

## Variable Commands

### Variable Manipulation
- `var.set:example:! expression !`: Set a variable. Example: 
  ```
  var.set:example:! 15 + 10 !;
  var.set:example:! §example§ + 20 !;
  ```
- `var.cng example number`: Change the value of a variable. Example: `var.cng example 42 ;`
- `var.del example`: Delete a variable to reduce lag. Example: `var.del example ;`

### Variable Expressions
- `! 

## Text Commands

### Text Display
- `txt.prt x y size text`: Print text on-screen. Example: `txt.prt -100 100 100 "Hello, World!" ;`

## File Loading Commands

### Load External Files
- `load.ign file_name x y z`: Load an image with scaling. Example: `load.ign example_image 0 50 100 ;`

## Conditional Statements

### If Statement
- `txt.prt x y size text /;`: Execute a line conditionally using a forward slash before the semicolon. Example: `txt.prt 0 0 100 "Example Text" /;`
- `if.key key_code line_number`: Check if a key is pressed and run a specific line. Example: `if.key w 1 ;`
- `if.eq value variable_name line_number`: Check if a value is equal to a variable and run a specific line. Example: `if.eq 10 §points§ 1 ;`

## Looping
- `loop line_number`: Create a loop that goes to a specified line. Example: `loop 1 ;`

## Discord API Integration
- `dcapi.load. userID skinName`: Load an avatar of a user. Example: `dcapi.load. 12345 my_skin ;`
- `dcapi.action. skinName`: Switch to a skin already loaded by the script. Example: `dcapi. action.skin1 ;`
