# Programming of Embedded System and Microcontrollers main project

Group task by me (Nina), Leo and Aleksi. I explain a little bit in English, as the course was in Finnish, and so was the report.

Our plan was to get max points, 5, from this project which meant:
-	Use at least 4 blocks of the microcontroller
-	Use 3 of those blocks with registers
-	Have a working bidirectional UI
-	Special detail
-	2 interrupts.

We used EEPROM, T/C1 sand ADconv with registers and TWI. Interrupts were with basic button interrupt and timer overflow interrupt. There is more detailed information about used parts in the report. Four row LCD-screen is attached to Arduino with I2C adapter.

My task was to create Spede-game, interrupts and register controls for T/c1 and ADC. Leo created part of the UI, register controls for switches, connect switches to Arduino and Minute-game. Aleksi’s task was to create the sweater, Sakari-game and connect the light sensor.

### Menu: 
Move up with yellow button (D9) and move down with white button (D11) and select with red one (D3). 

### Spede-game: 
React to X position on the LCD screen. If X in middle, click middle button, if right, click right etc. After pressing wrong button or timer runs out the game ends. Timer goes faster every successful click. After the end, check if the score is enough for top three and add it accordingly to EEPROM if it is.

### Sakari-game: 
Put the sweater on Sakari before 10 seconds timer runs out. Light sensor reads the sweater light blocking. Cannot be used in dark room.

### Minute-game: 
Press the button one minute. Closer the time is to one minute, bigger points you get.  






