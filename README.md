# telakone-robo-board

## Requirements


* Input power supply range 12..50V
* 5V regulator for external stuff (servos, LEDs, ...)
* CPU STM32F407
* RS-485 half-duplex serial interface
* PS2 (playstation) control (SPI)
* I2C for external acceleration sensors
* WS2812B control for LED lights
* USB device interface
  * Virtual serial port
* Digital outputs
  * 1 enable output for stepper drivers
  * 6 pulse outputs for stepper drivers
  * 6 direction outputs for stepper drivers
  * 2 servo signal outputs
  * 2 high side switch outputs
* Digital inputs
  * 14 inputs for limit/zero switches
  * 1 input for emergency stop
  
