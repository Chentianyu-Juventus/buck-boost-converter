# buck-boost-converter


1.Buck-Boost DC/DC Converter:
The Buck-Boost converter, also known as a step-up/step-down converter, is a type of switching regulator. It is a single-inductor, non-isolated DC-DC converter capable of generating an output voltage that is either lower or higher than the input voltage. The Buck-Boost circuit overcomes the limitations of traditional linear regulators, such as low efficiency, and provides advantages like small size, lightweight, and better adaptability to varying output voltage requirements.


2.Buck-Boost Operating Principle:
The Buck-Boost converter combines the working principles of Buck and Boost converters into one circuit with a single switch. This type of converter can adjust the input voltage VS to a desired output voltage Vo , allowing it to step up or step down the input voltage. It is widely used in small and medium-sized DC/DC power conversion applications due to its efficient energy utilization, voltage regulation, and noise suppression capabilities.


![image](https://github.com/user-attachments/assets/2fc16abf-201f-4104-99cf-c8f2227b3c10)


As shown in the diagram, the Buck-Boost circuit consists of an IGBT (Sw, the switch), a diode (D), an energy storage inductor (L), and a filter capacitor (C). The IGBT operates at a switching frequency of tens to hundreds of kilohertz. Its operation is divided into two states: conduction (𝑇on) and cutoff (𝑇off)

(1)During 𝑇on, the IGBT is conducting, the inductor 𝐿stores energy, and the inductor current 𝑖𝐿 increases.

(2)During 𝑇off, the IGBT stops conducting, and the energy stored in the inductor is released to the load through the diode 𝐷.This allows the output voltage 𝑉𝑜to remain continuous, and the circuit completes energy transfer to the load.


3.Relationship between input and output volatges in the circuits

  (1) Vi*Ton = Vo*Toff
  (2) then Vo =  Ton/Toff * Vi = Ton/Ts-Ton * Vi = D/1-D * E
note: D = Ton/Toff is the duty cycle ,by adjusting the duty cycle D:
The output voltage can be lower than the input voltage (0<D<0.5), functioning as a Buck converter.
The output voltage can be higher than the input voltage (0.5<D<1), functioning as a Boost converter.
  


