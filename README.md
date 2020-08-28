# STM32F401RExx-TFT-Display
This example shows how to integrate with the TFT 240x320 Display with the almost all the STM32 MCUs via SPI.
To use this for different STM32MCU please update all the references from the source. Also, make sure to update the PIN layout if you are not using the SPI. Please look at the sample for the reference:

```c
                                //  TFT | STM32F401RExx Nucleo Board
#define T_CLK_Pin GPIO_PIN_5    // SCK	PA_5(D13)
#define T_CLK_GPIO_Port GPIOA

#define T_MISO_Pin GPIO_PIN_6   // MISO	PA_6(D12)
#define T_MISO_GPIO_Port GPIOA

#define T_MOSI_Pin GPIO_PIN_7   // MOSI	PA_7(D11)
#define T_MOSI_GPIO_Port GPIOA

#define T_CS_Pin GPIO_PIN_5     // CS	PB_5(D4)
#define T_CS_GPIO_Port GPIOB

#define DC_Pin GPIO_PIN_8       // D/C	PA_8(D7)
#define DC_GPIO_Port GPIOA

#define RST_Pin GPIO_PIN_10     // Reset	PA_10(D2) Pull Up(100k)
#define RST_GPIO_Port GPIOA
```

Find the file mxconstants.h for PIN layout.

![STM32-TFT Sketch](https://github.com/mhdazeem/STM32F401RExx-TFT-Display/blob/master/STM32-TFT%20Sketch/Pin%20Layout%20TFT%20Display.jpg)
