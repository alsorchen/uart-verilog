### Simple verilog UART.

Requires a 50MHz input clock that gets divided into 
clock enables for a 16x oversampling receiver
clock enable and 115200 baud transmission clock enable.

Icarus verilog testbench verifies that each byte can be sent correctly, but
does not do anything with spacing between bytes.

### use with DE-10 Lite

* GPIO[24] : uartTX - fpgaRX wire
* GPIO[25] : uartRX - fpgaTX wire
* 3.3V & GND

![image](https://user-images.githubusercontent.com/6558862/32832009-7a0940a0-ca3d-11e7-9485-fc3430176367.png)
