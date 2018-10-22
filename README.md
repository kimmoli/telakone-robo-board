# telakone-robo-board

## Requirements


* Input power supply range 12..50V
* 5V regulator for external stuff (servos, LEDs, ...)
* CPU STM32F407
* RS-485 half-duplex serial interface
* PS2 (playstation) control (SPI)
  * SPI1
    * SPI1_SCK PB3 AF5
    * SPI1_MISO PB4 AF5
    * SPI1_MOSI PB5 AF5
    * SPI_CS_N PA8 OUTPUT
* I2C for external acceleration sensors
  * I2C1
    * I2C1_SCL PB6 AF4
    * I2C1_SDA PB7 AF4
* WS2812B control for LED lights
  * USART2
    * USART2_TX PA2
* USB device interface
  * Virtual serial port
    * OTG_FS_DM PA11 AF10
    * OTG_FS_DP PA12 AF10
	* USB_RENUM PB15 OUTPUT
* Wired UART
  * USART3
    * USART3_TX PD8 AF7
    * USART3_RX PD9 AF7
* RS485 UART
  * USART1
    * USART1_TX PA9 AF7
	* USART1_RX PA10 AF7
	* USART1_TXE PD15 OUTPUT
* Digital outputs
  * 1 enable output for stepper drivers
    * PE14 OUTPUT
  * 6 frequency outputs for stepper drivers
    * TIM4_CH1 PD12 AF2
    * TIM5_CH1 PA0 AF2
    * TIM8_CH1 PC6 AF3
    * TIM9_CH1 PE5 AF3
    * TIM10_CH1 PB8 AF3
    * TIM11_CH1 PB9 AF3
  * 6 direction outputs for stepper drivers
    * PE8 OUTPUT
    * PE9 OUTPUT
    * PE10 OUTPUT
    * PE11 OUTPUT
    * PE12 OUTPUT
    * PE13 OUTPUT
  * 2 servo signal outputs
    * TIM3_CH1 PA6 AF2
    * TIM3_CH2 PA7 AF2
  * 2 high side switch outputs
    * PC0 OUTPUT
    * PC1 OUTPUT
  * 3 debug led outputs
    * PC2 OUTPUT DEBUG (Green)
	* PC3 OUTPUT RUN (Green)
	* PC4 OUTPUT ERROR (Red)
* Digital inputs
  * 16 inputs for limit/zero switches, emergency stop
    * PC8 INPUT
    * PC9 INPUT
    * PC10 INPUT
    * PC11 INPUT
    * PC12 INPUT
    * PC13 INPUT
    * PC14 INPUT
    * PC15 INPUT
    * PD0 INPUT
    * PD1 INPUT
    * PD2 INPUT
    * PD3 INPUT
    * PD4 INPUT
    * PD5 INPUT
    * PD6 INPUT
    * PD7 INPUT
