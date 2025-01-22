# Simon Says Game on STM32 F4F407VG Discovery Board

Hello! This is my first STM32 project! In this project, I have created a **Simon Says** game on the **STM32 F4F407VG Discovery Board** using the **HAL** library and external buttons.

## Features
- Implements the classic **Simon Says** game.
- User can interact with the game through external buttons.
- You can change the difficulty by adjusting the `numOfSequences` value (e.g., setting it to 10 instead of 8 for a harder game).
- Uses the **GPIO** pins for buttons and **RNG** (Random Number Generator Peripheral) for generating sequences.

## Requirements
- **STM32 F4F407VG Discovery Board**
- **HAL (Hardware Abstraction Layer) library**
- External buttons connected to the GPIO pins
- Set HCLCK to 168MHz to ensure smooth inputs
- Utilize 1K Ohm reistors if GPIO pins are not in PULLUP mode

## Setup

1. **Configure the Hardware**:
   - Connect external buttons to the appropriate GPIO pins for input detection.
   - Set up the LEDs on the board to display the sequence (or any other GPIO pins you prefer for output).

2. **Enable Peripherals**:
   - In your STM32CubeMX or initialization code, ensure you enable the following peripherals:
     - GPIO Clocks
     - RCC Clock
     - RNG Peripheral

## Usage

- After the setup, the game will run, and the system will generate a sequence of light patterns.
- The player must repeat the sequence by pressing the corresponding buttons.
- The game continues until the sequence is correctly repeated or the player makes an error.
  
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to STM32CubeMX for peripheral initialization.
- Thanks to the STM32 community for their invaluable resources and examples!

---

Thanks for checking this out! I hope you enjoy it as much as I did making it.

