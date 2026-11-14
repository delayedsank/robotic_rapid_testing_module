# robotic_rapid_testing_module

> Portfolio overview of embedded firmware work on a rapid gene-testing instrument. This repository presents selected, sanitized software concepts and architecture notes—not a complete device firmware release.

## Project overview
This project was basically for scientists who discovered rapid algorithm for a potent disease which would be stationed at airports to check possible contaminated passengers in a quick test.  

The instrument combines embedded control with electromechanical and thermal subsystems. The host computer communicates with the embedded controller over UART using command-based control. The broader device work included cartridge movement, a UV illumination chamber, and custom heater hardware intended to maintain a controlled temperature range which involves High Power AC Control using Zero detection of Sinusoidal waves.

Power control was required for a specialized component that needed to be at certain temperature constantly for the diagnostic process .

I headed the project as Project Manger working on device system and headed various miscellaneous teams from 3D designers to Purchase Teams. 

As this system had many components like high power heating equipment,  NEMA stepper motors ,sensors , a start up check as boot loader was required to check all components and test against various referenced voltages and current . which was very important .  

## Firmware concepts represented in the available source excerpts

- UART communication with a host computer (configured at 115200 baud in the provided examples)
- GPIO initialization and command-driven output control
- Command parsing and state flags
- ESP-IDF / FreeRTOS application structure
- MCPWM-based servo or motion-control interface
- Timer-based state/time-out handling
- AHT20 I²C sensor interface setup 
-
-
-
-
-







The device is based on PCB designed by me thru hit and trial of various electronic component procured by purchase department.


This Device used ESP32 S3 at prototype level and was converted to STM32 later during production level . 
