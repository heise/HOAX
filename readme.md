HX3 Hammond Clone
=================

<b>LATEST NEWS:</b> New update program for Windows available - makes fiddling with AVRdude and TeraTerm obsolete! See directory LATEST.

HX3/HOAX steht kurz f�r Hammond On A Xilinx FPGA und ist ein v�llig neuer Ansatz einer Tonewheel-Emulation als 
eigenst�ndiges Soundmodul auf einer Platine, erh�ltlich bei KeyboardPartner (http://shop.keyboardpartner.de). Hier 
finden Sie alle Schaltpl�ne, Zeichnungen und Firmware-Updates.

HX3 is a full-featured Hammond clone module with physical modelled tone generation from KeyboardPartner 
(http://shop.keyboardpartner.de). Please find here all documentation, schematics, drawings and firmware/configuration updates.

(Scroll to bottom for english description) 

HX3-Firmware-Installation
=========================

Bitte beachten Sie die ausf�hrliche Anleitung auf http://wiki.keyboardpartner.de! Ge�nderte File-Struktur im Repository: Alle zusemmengeh�rigen Dateien sind jetzt f�r einfacheren Download in entsprechende ZIP-Dateien verpackt.

### Enthaltene Flash-Dateien

* <b>HOAX_main.hex</b>             HX3 Standard, ggf. mit Preset24 oder 1 bis 2 Preset16-Panel<br>
* <b>HOAX_main_latching.hex</b>	   Latching Presets (einrastende Tasten) mit alter Preset12 MPX Platine<br>
* <b>HOAX_main_tabvib.hex</b>      wie Standard, jedoch drei Schalter (V1,V2,CH - V3=V1+V2) statt Drehschalter an PL5<br>
* <b>HOAX_main_buttonvib.hex</b>   wie Standard, jedoch Vibrato-Einstellung �ber die vier Common-Preset-Taster von Panel16 statt Drehschalter<br>
* <b>HOAX_main_xb2.hex</b>         Spezialversion f�r XB2-Einbausatz, nutzt vorhandene Bedienelemente und Display<br>
* <b>HOAX_main_xb2_panel16.hex</b> Spezialversion f�r alten XB2-Einbausatz mit Panel16<br>
* <b>Preset24.hex</b>              Firmware f�r ATmega8 auf Preset25-Platine<br>

### im Verzeichnis FPGACORES

* <b>fpga_*.bit</b>                FPGA-Konfiguration zum Upload mit HX3 Remote<br>
* <b>*.dat</b>                     Keyscan-Routinen, zum Upload mit HX3 Remote<br>
* <b>*.bin</b>                     SPIN-1 externe I2C Rerverb Programme, zum Upload mit HX3 Remote<br>

### Verzeichnisse

* <b>LATEST</b>                      enth�lt allerletzte Firmware und FPGA-Konfiguration<br>
* <b>DOCS_PDF</b>                  Syntax-Tabelle zur Kommunikation und weitere Unterlagen<br>
* <b>FPGACORES</b>                 FPGA-Konfiguration, Hallprogramme und Scan-Cores<br>
* <b>PLATINEN</b>                  Schaltpl�ne, Best�ckungspl�ne und weitere Unterlagen<br>
* <b>FOR_OEM</b>                   enth�lt alle dateien f�r AVR-Erstprogrammierung, wie oben, jedoch mit eingebautem Bootloader 
(Arduino/AVRdude-kompatibel) f�r Programmierung eines fabrikneuen AVR-
Controllers. Au�erdem: <b>ATmegaBOOT_xx8.c</b> und <b>Makefile</b>, nur f�r Neukompilierung des Bootloaders mit WinAVR n�tig<br>


HX3 Firmware Installation (english)
===================================

<b>LATEST NEWS:</b> New update program for Windows available - makes fiddling with AVRdude and TeraTerm obsolete! See directory LATEST.

FPGA configuration and scan cores may be uploaded by provided HX3 Remote application. 

### AVR flash files

Flash files for serial upload via HX3 Remote 

* <b>HOAX_main.hex</b>             standard version with rotary vibrato switch, optional Preset24 or Preset16-Panel<br>
* <b>HOAX_main_latching.hex</b>	  version for latching preset keys with old Preset12 MPX board<br>
* <b>HOAX_main_tabvib.hex</b>      as standard, but 3 switches (V1,V2,CH - V3=V1+V2) instead of rotary vibrato switch at PL5<br>
* <b>HOAX_main_buttonvib.hex</b>   as standard, but vibrato setting (V1..V3, CH) by four Common Preset buttons on Panel16<br>
* <b>HOAX_main_xb2.hex</b>         special version for XB2 retrofit kit, uses XB2's buttons and display<br>
* <b>HOAX_main_xb2_panel16.hex</b> special version for XB2 retrofit kit, uses installed Panel16<br>

### directories

* <b>LATEST</b>                    last firmware revisions and FPGA configurations, testing only<br>
* <b>DOCS_PDF</b>                  Syntax table for HX3 COM port, MIDI tables etc. <br>
* <b>FPGACORES</b>                 FPGA configuration, reverb firmware and keyboard scan cores for upload with TeraTerm macro<br>
* <b>PLATINEN</b>                  schematics, mechanical drawings, board and componentlayouts<br>
* <b>TERATERM_MACRO</b>            FPGA and scan core pdate macros for terminal emulator TeraTerm 4.7x (Windows)<br>
* <b>FOR_OEM</b>                   contains all flash files as above, but with built-in bootloader (Arduino/AVRdude compatible). Contains also:
<b>ATmegaBOOT_xx8.c</b> and <b>Makefile</b>, only needed for re-compilation of bootloaders with WinAVR<br>

AdaBoot by Adafruit, modified for ATmega644P(A)06/2012 by Carsten Meyer, cm@ct.de

