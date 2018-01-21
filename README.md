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
    * SPI_CS_N PA9 OUTPUT
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
* Wired UART
  * USART3
    * USART3_TX PD8 AF7
    * USART3_RX PD9 AF7
* Digital outputs
  * 1 enable output for stepper drivers
    * PE14
  * 6 frequency outputs for stepper drivers
    * TIM4_CH1 PD12 AF2
    * TIM5_CH1 PA0 AF2
    * TIM8_CH1 PC6 AF3
    * TIM9_CH1 PE5 AF3
    * TIM10_CH1 PB8 AF3
    * TIM11_CH1 PB9 AF3
  * 6 direction outputs for stepper drivers
    * PE8
    * PE9
    * PE10
    * PE11
    * PE12
    * PE13
  * 2 servo signal outputs
    * TIM3_CH1 PA6 AF2
    * TIM3_CH2 PA7 AF2
  * 2 high side switch outputs
    * PC0
    * PC1
  * 1 debug led output
    * PC2
* Digital inputs
  * 16 inputs for limit/zero switches, emergency stop
    * PC8
    * PC9
    * PC10
    * PC11
    * PC12
    * PC13
    * PC14
    * PC15
    * PD0
    * PD1
    * PD2
    * PD3
    * PD4
    * PD5
    * PD6
    * PD7
  
  
