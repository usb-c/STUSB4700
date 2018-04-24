# STUSB4700
Autonomous USB-PD controller for Power Sources

# Presentation

Product type: USB PD controller <br/>
Manufacturer: STMicroelectronics <br/>
Role: Provider only <br/>
Architecture: Full hardware solution <br/>
Supported Version: USB-C r1.2 & USB-PD r2.0 <br/>

The STUSB4700 is a USB Type-C & Power Delivery controller, that has to be used on the Source side (USB-PD Provider / DFP / Source). <br/>
No software needed, but it can be optionally controlled with a Microcontroller (like STM32) to configure it through I2C interface.

The STUSB4700 is certified by the USB-IF consortium. <br/>
Official USB Certification test ID = 1030023

There are 2 versions of STUSB47:
   - one part number with Vconn power output (needed for active cables): STUSB4700
   - one part number without Vconn (in a smaller package) : STUSB4710

It can be added easily to different kind of applications:
  - Application without USB data (e.g. Power supplies doesn't need Data interface)
  - Application with USB 1.1 Data interface (Low speed)
  - Application with USB 2.0 Data interface (Full speed 12Mbps - or - High speed 480Mbps)
  
  
# Main features

* Support any USB PD profiles:
  * the official profiles : 5V, 9V, 15V, 20V
  * the older profiles : 5V, 12V, 20V
  * or custom profiles (for instance: 5V, 10V, 19V)
  * It embeds a internal memory which can contain up to 5 PDOs (Power Data Object)

* Flexible power supply input: 
  - Directly from Vbus voltage level [4.1 V; 22 V]
  - or with a fixed supply in the system [3.0 V; 5.5 V]

* Embed high voltage protection on VBUS pin & CC pin
  - No need of external ESD protection on these pins
  - Protect from potentially damaged USB-C cables with VBUS-to-CC short protection


* Can be used to buid a standard USB-PD power supply at : 7.5W, 15W, 27W, 36W, 45W, 60W. <br/>
Any voltage can be used, but not more than 3A because it would required extra communication with an active cable.
  
 Note: <br/>
 A Standard USB-C cable on the market is rated 3A. <br/>
 The USB-C cables supported 5A are more expensive. <br/>
 
  
