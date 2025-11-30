## Description

Sequence

Progressive Stacking Runner Sequence (Left-to-Right)
	In this mode, a single runner LED moves sequentially from the leftmost LED to the rightmost LED, and each time the runner reaches the end, that LED becomes permanently latched ON, causing the illuminated LEDs to stack progressively from right to left until all LEDs remain ON.
  
Progressive Stacking Runner Sequence (Right-to-Left) 
	When the button is pressed, the runner LED travels from the rightmost LED to the leftmost LED, and whenever it reaches the end of the strip, that LED is locked ON, producing a progressive stacking effect from left to right until the entire LED array is illuminated.


## Software

### Project Usage

Universal instructions on building, flashing, and debugging this project can be found in the **[MSDK User Guide](https://analogdevicesinc.github.io/msdk/USERGUIDE/)**.

### Project-Specific Build Notes

* This project comes pre-configured for the MAX78000EVKIT.  See [Board Support Packages](https://analogdevicesinc.github.io/msdk/USERGUIDE/#board-support-packages) in the UG for instructions on changing the target board.

## Setup

If using the MAX78000EVKIT (EvKit_V1):
-   Connect a USB cable between the PC and the CN1 (USB/PWR) connector.
-   Connect pins 1 and 2 (P0_1) of the JH1 (UART 0 EN) header.
-   Open a terminal application on the PC and connect to the EV kit's console UART at 115200, 8-N-1.
-   Close jumper JP1 (LED1 EN).
-   Close jumper JP2 (LED2 EN).

If using the MAX78000FTHR (FTHR_RevA)
-   Connect a USB cable between the PC and the CN1 (USB/PWR) connector.
-	Open a terminal application on the PC and connect to the EV kit's console UART at 115200, 8-N-1.

## Expected Output

The Console UART of the device will output these messages:

```
Hello World!
count : 0
count : 1
count : 2
count : 3
```

You will also observe the LED (LED1 for EvKit_V1 or D1 for the Featherboard) blinking at a rate of 2Hz.
