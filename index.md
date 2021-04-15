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

## Why should you build and program your own syringe pump?

If you are interested in tissue engineering, a syringe pump offers you a simplified version of an extrusion printer. This bioplotter allows you to robustly plot tissue constructs for innovative research in regenerative medicine and human physiology. Building and programming your own syringe pump (potentially with the resources on this website) allows you flexibility to design your bioprinter to your specific biofabrication needs!
