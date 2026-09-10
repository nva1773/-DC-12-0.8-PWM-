# -DC-12-0.8-PWM-
Chinese DC 12V 0.8A PWM fan speed controller with temperature sensor.

![Foto](https://github.com/nva1773/-DC-12-0.8-PWM-/blob/main/Foto/Chinese%20DC%2012V%200.8A%20PWM%20fan%20speed%20controller%20with%20temperature%20sensor%20-%20foto.jpg)

Schematic diagram created from a printed circuit board:

![Chinese DC 12V 0.8A PWM fan speed controller - circuit diagram](https://github.com/nva1773/-DC-12-0.8-PWM-/blob/main/Foto/Chinese%20DC%2012V%200.8A%20PWM%20fan%20speed%20controller%20-%20circuit%20diagram.jpg)

Sometimes it is necessary to respond to overheating of the cooled component (such as a heatsink) where the NTC sensor for this fan speed controller is mounted. If installing an additional overheat sensor is not feasible, a simple detector can be built using an LM358 operational amplifier:

![Overheat detector - SCH](https://github.com/nva1773/-DC-12-0.8-PWM-/blob/main/Foto/Overheat%20detector.jpg)

The voltage divider at the non-inverting input of the operational amplifier sets the comparator's switching threshold (which is 70°C with the current resistor values). The 510 kΩ resistor provides positive feedback, introducing a switching hysteresis of ±5°C.

I assembled the circuit on a 40x50 mm prototyping board. Since I needed to cool two separate heatsinks, I utilized the second channel of the op-amp LM358.

![Overheat detector - PCB](https://github.com/nva1773/-DC-12-0.8-PWM-/blob/main/Foto/Overheat%20detector%20-%20pcb.jpg)
