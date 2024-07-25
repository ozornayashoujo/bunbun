## TODO 

### Add screens with no dialogue/text etc. For example, when in room
    clicking should advance NOTHING, no text, only user ACTIONS should be able to progress the game

### Time system
    turn-based, each action progresses time by X amount. mod 24
        add calendar, roll over days and weekdays

        [23:00 Wed]
        - do action
        [23:30 Wed]

    display time and weekday as overlay in HUD

### Create system of "rooms", going between which will not advance time
    it can be "house" - "door" - "street" - "store" or any kind of basic "map"

### Add room customization
    add function to add/remove object decorations
        add interactable objects
    add function to change character sprite (costume)

### Basic inventory management
    Display overlay with icons OR list with item display and description on side
        OR mouse-over description
        ANDOR selection description

### Basic stat counters
    add items that will display a stat to be higher than it actually is, make status effects system (flag system)

### Sleep event
    when action is sleep display specific event sequence
        choose sequence to display based on stats and flags (maybe add flags that update dynamically with stat updates) 
            action -> stat update ++/-- -> raise/lower flag
                when action is sleep choose dream scene based on flags
                    (update only before sleep?)

### Add item acquisition
    create a new scene for the store
        add overlay with clickable buttons to add items to inventory
            check if the player has enough money to buy items
                add special bunmom interaction if you use her credit card
    add computer first computer interaction - buying items from bunzon
        display list of items to buy
            add basic item search?

### Usable items
    basic item functionality/usage. Click "use item" -> increase one stat by +1.

### Limit player saving to select stages/screens/phases (no saving during dream scenes)

### windowframe.png always has highest zorder
    hide windowframe for dream scenes

### Add achievement system
    add achievement menu
        display completion % ???

### Add artwork gallery
    add dream replay gallery?

__________________________________________________________________________________________________

## IDEAS


### Make actions adjust stats with RNG based on function. See link for possible reference
      https://easings.net/

### add door opening/closing mini-game
    show window with a keyhole -> click to put in a key -> drag the side of the key to rotate it -> finish, close the window

### Computer interactions
     TODO. WIP. add a website scrolling animation. text and placeholder being displayed, going up and disappearing
        add drawing mini-game. show empty window -> click to draw with a basic pencil -> possibly make it save-able?????
        basic desktop "game". when opened the desktop has random files -> drag and drop them into the recycle bin -> remove entity
            add system32 to desktop, make it deleteable, make it disable clicking (using) the computer
        sudoku minigame. steal sudoku generator code, remove some numbers, add input box with input limitations (or dropdown select)
     add "buncord" (discord) - you input messages, they display in a window, scrolling up, and with a random interval the "friend" replies
        (all they say is scripted messages like "LOL" "that's crazy" "based" "cringe" etc.)

### If under status effect (extra low or high stat), unlock special item interactions
    (fun and fatigue < 0 + knife, fun > 10 + something...) - you get the idea


### FINAL TASK:
    Implement minigame window to run custom scripts in python
        Run snake in a separate screen/window
        https://github.com/RuolinZheng08/renpy-minigames101