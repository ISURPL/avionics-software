# Add filename.o to include in compilation
OBJECTS=misc.o stm32f4xx_gpio.o stm32f4xx_rcc.o stm32f4xx_usart.o stm32f4xx_dma.o stm32f4xx_i2c.o stm32f4xx_spi.o


%.o: %.c
	$(CC) -c $(CFLAGS) $(CPPFLAGS) $< -o $@

%.o: %.s
	$(AS) -c $(ASFLAGS) $< -o $@

all: $(OBJECTS)

clean:
	rm -f *.o
