This is library to use the nrf24l01 on the raspberry pi.

It's based on the arduino lib from J. Coliz <maniacbug@ymail.com>.
The library was berryfied by Purinda Gunasekara <purinda@gmail.com>.
Ported to shared library by Arco van Geest <arco@appeltaart.mine.nu>
rpi-hub examples by Stanley Seow <stanleyseow@gmail.com>

Instruction for installing the shared libraries :-

cd librf24
make
sudo make install
cd ../examples
make

To execute the examples, type :-
sudo ./pingtest or
sudo ./scanner

Pin used for RPi & nRF as below

RPi-3v3 	= nRF-vcc ( Can ONLY accept 3.3V only )
RPi-gnd 	= nRF-gnd
RPi-MOSI/GPIO10 = nRF-MOSI
RPi-MISO/GPIO9	= nRF-MISO
RPi-SCLK/GPIO11	= nRF-SCK
RPi-CE0/GPIO8	= nRF-CE
RPi-CSN/GPIO25	= nRF-CSN

/dev/spidev0.0 = CE0/GPIO8
/dev/spidev0.1 = CE1/GPIO7


