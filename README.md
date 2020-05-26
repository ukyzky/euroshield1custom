# 1010 music euroshield 1 custom

## hardware

- 1010 music euroshield 1 with teensy 3.2

- ili9341 SPI 2.8inch touch LCD.

at first, solder LCD's J1 jumper for using 3.3V

connect teensy3.2 and LCD pins.
(below teensy3audioboard is not used. it's only for information.)

|ili9341 LCD|euroshield 1|(teensy3audioboard)|teensy3.2|teensy3.2|(teensy3audioboard)|euroshield 1|ili9341 LCD|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|GND|ground|GND|GND|VIN||VIN 5V||
||midi in||0|A GND|GND|||
||midi out||1|3.3V|3.3V|3.3V|RESET, VCC, LED(with 100ohm registor)|
||button input||2|23|LRCLK|LRCLK||
||led1||3|22|DIN|TX||
||led2||4|21||pot input||
||led3||5|20||pot input||
||led4|MEMCS|6|19|SCL|SCL||
|SDI(MOSI), T_DIN||MOSI|7|18|SDA|SDA||
|T_CS(alt any)|||8|17||||
||BCLK|BCLK|9|16|||T_IRQ(optional. alt any *2)|
|D/C(alt 10,15,*20,21)||SDCS|10|15|Vol||CS(alt 9,15,20,*21)|
||MCLK|MCLK|11|14|SCK||SCK, T_CLK|
|SDO(MISO), T_DO||MISO|12|13|DOUT|RX||

## software

(now in development)

- hand writing waveform oscillator

- CV and touch controlling bezier curve slope generator

## refs

