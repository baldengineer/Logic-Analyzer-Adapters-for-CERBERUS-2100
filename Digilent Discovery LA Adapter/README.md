## Digilent Discovery LA Adapter
![Digital Discovery Adapter Connected](images/CERBERUS_2100_Digital_Discovery_Adapter.jpg)

This adapter is inteded to be used with a [Digilent Digital Discovery](https://digilent.com/shop/digital-discovery-portable-usb-logic-analyzer-and-digital-pattern-generator/). (Not the Analog Discovery!) These are USB-based logic analyzers that sample up to 100 MHz and 32 signals.

The center connector plugs into the socket. The right connector is for an expansion card. The left connector is for the Digital Discovery. 

Three connection options:
1. Use a short ribbon cable.
2. Mount the header upside-down.
3. Mount the header top-side-up.

### Waveforms Project File
Use the latest [beta version of Waveforms](https://forum.digilent.com/topic/8908-waveforms-beta-download/).

There is a bug with the pattern trigger. Addresses are reversed. So, to trigger on `0x0205` (`0000 0010 0000 0101`) you need to set the pattern to `0xA040` (`1010 0000 0100 0000`).

The clocks and control signals connect to the 24-32 inputs.

[CERBERUS 2100 Digital Discovery Template.dwf3work](CERBERUS 2100 Digital Discovery Template.dwf3work) is a starting project. It has all of the signals mapped for you! 


### Build Notes
Easily connect a Digilent Digital Discovery to a CERBERUS 2100. At a minimum, you'll need a 40-pin socket and a right-angle 32-pin socket. To act as an interposer between the CERBERUS and expansion card, you need a 40-pin header. There's also a spot for a 0805 resistor and 1206 LED for bling.

### OSH Park Link
The KiCad design files and PCB gerbers are available. Or you can order these boards directly from [OSH Park using this link](https://oshpark.com/shared_projects/0LsKYepP).