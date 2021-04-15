# How to Build a Syringe Pump

- **[Home](/CHBE-5890-Syringe-Pump-Build/index)**
- [Mechanical](/CHBE-5890-Syringe-Pump-Build/mechanical)
- [Electrical](/CHBE-5890-Syringe-Pump-Build/electrical)
- [Code](/CHBE-5890-Syringe-Pump-Build/code)

## Specifications

The assembly that I describe on the pages above can accomodate a syringe with the dimensions in the image below, and the program that I provide in "Code" specifies 200 steps/revolution of the stepper motor. A bill of materials for the syringe pump provides further material specifications and is available on the "Mechanical" page.

![Specifications for syringe housed by our assembly](/CHBE-5890-Syringe-Pump-Build/Images/Syringe-Specs.png)

Assuming that this assembly uses a single start screw, it can take 564 steps/mL fluid released from syringe when its stepper motor is operating at 200 steps/revolution. Our assembly is also capable of microstepping, with the stepper motor accomodating 3,200 steps/revolution. In this case, 9,029 steps/mL are possible.

At 200 steps/revolution, the assembly achieves microliter resolution (1.8e-3 mL released from syringe/step). At 3,200 steps/revolution, 10e-7 L resolution is possible (1.1e-4 mL released from syringe/step). Therefore, the max resolution from our assembly is 10e-7 L.

The calculations I performed to obtain these values are below (image captured from my notes):

![Calculations for syringe pump resolution](/CHBE-5890-Syringe-Pump-Build/Images/Resolution-Calculation.heic)

Factors that restrict the maximum flow rate from the syringe at each pump incude limitations in the Arduino's processing speed and maximum current output. Indeed, the bottleneck in a stepper motor's operation is the time between pulses that it receives from the Arduino and other drivers; this time is not changable. The result is a limit on the amount of outflow from the syringe, as less time between pulses could result in more continuous efflux. The maximum current output of the Arduino Uno is 40 mA, and stepper motors are spec'd. by their current capacities. These factors further limit signal strength for stepping (and the associated pumping), limiting flow from the syringe.

## Why should you build and program your own syringe pump?

If you are interested in tissue engineering, a syringe pump offers you a simplified version of a bioplotter. This extrusion system allows you to robustly plot tissue constructs for innovative research in regenerative medicine and characterization of human physiology. Building and programming your own syringe pump (potentially with the resources on this website) gives you flexibility to design a printer to your specific biofabrication needs!
