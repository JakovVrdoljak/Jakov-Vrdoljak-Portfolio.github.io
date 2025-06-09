# Jakov Vrdoljak - Portfolio
Electronics engineer specializing in microelectronics and embedded hardware. Experienced in IC design, PCB routing, and NB-IoT development.

## Work Experience
- **Junior Embedded Engineer, Holosys**  
  *July 2024 - Present*  
  - Developing NB-IoT devices, routing PCBs, and performing impedance matching for antennas 
  - Testing device performance and writing documentation 
  - *Tools*: Altium Designer, measurement equipment

- **Junior Layout Engineer, Inovacijski centar Nikola Tesla**  
  *March 2023 - November 2023*  
  - Designed layouts for test cells, ensuring LVS and DRC compliance
  - *Tools*: Cadence Virtuoso

- **Embedded Hardware EMC Engineer Intern, Rimac Technology**  
  *July 2022 - September 2022*  
  - Designed PCB traces for differential pairs and single-ended signals  
  - Reviewed PCBs for EMC compliance and wrote a Python script to calculate PCB dielectric constant using S-parameters  
  - *Tools*: Altium, Python

- **Technical Support, Končar INEM**  
  *July 2021 - August 2021*  
  - Added components to Altium Vault and routed PCBs  
  - *Tools*: Altium Designer

## Student Projects
- **Master Thesis: Bootstrap Switch and Op-Amp for Pipeline ADC with Switched Capacitance**  
  *October 2023 - July 2024*  
  - Designed a switched-capacitance amplifier with a bootstrap switch for an 8-bit pipeline ADC in 180nm CMOS technology using Cadence Virtuoso  
  - Developed and compared a bootstrap switch (on-resistance <400Ω) against a standard CMOS switch, analyzing THD, SNR, and SFDR via transient simulations  
  - Created the switch layout, extracted parasitic components (e.g., capacitance, resistance), and compared performance degradation against the ideal bootstrap design  

  - *Bootstrap schematics and layout*:  
    <table>  
      <tr>  
        <td><img src="/Images/Bootstrap_switch.png" alt="Bootstrap Switch Schematic" width="600"></td>  
        <td><img src="/Images/Layout_Bts.png" alt="Bootstrap Layout" width="600"></td>  
      </tr>  
      <tr>  
        <td>Bootstrap Switch Schematic</td>  
        <td>Bootstrap Switch Layout</td>  
      </tr>  
    </table>  

  - Built a folded-cascode op-amp (65 dB gain, 8.81 MHz bandwidth) with a power supply, constant-current generator, and startup circuit; performed AC and DC analysis for stability  
  - Implemented a feedback loop with CMOS switches, optimizing phase margin (>60°) and confirming stability under switched-capacitance operation  
  - Designed the amplifier layout and feedback loop, extracted parasitics, and compared post-layout performance with pre-layout analysis  

  - *Schematics*:  
    <table>  
      <tr>  
        <td><img src="/Images/Preklopljena_kaskoda.png" alt="Folded-cascode" width="600"></td>  
        <td><img src="/Images/Napajanje.png" alt="Power supply" width="600"></td>  
        <td><img src="/Images/iref.png" alt="Constant-current generator and startup circuit" width="600"></td>  
        <td><img src="/Images/PK_FB.png" alt="Feedback loop" width="600"></td>  
      </tr>  
      <tr>  
        <td>Folded-cascode</td>  
        <td>Power supply</td>  
        <td>Constant-current generator and startup circuit</td>  
        <td>Feedback loop</td>  
      </tr>  
    </table>  

  - *Layout*:  
    <table>  
      <tr>  
        <td><img src="/Images/pojačalo_napajanje.png" alt="Folded-cascode, power supply, Constant-current generator and startup circuit" width="600"></td>  
        <td><img src="/Images/Povratna_veza_lt.png" alt="Feedback loop" width="600"></td>  
      </tr>  
      <tr>  
        <td>Folded-cascode, power supply, Constant-current generator and startup circuit</td>  
        <td>Feedback loop</td>  
      </tr>  
    </table>  

  - Analyzed the switched-capacitance amplifier’s THD, SNR, and SFDR, comparing configurations with full CMOS, input-only bootstrap, and full bootstrap switches  
  - Conducted corner analysis across temperature (-40°C to 125°C) and voltage (1.62V to 1.98V), ensuring robust performance under process variations  

  - *Switched-capacitor amplifier schematics and layout*:  
    <table>  
      <tr>  
        <td><img src="/Images/switch_amp.png" alt="Switched-capacitor amplifier Schematic" width="600"></td>  
        <td><img src="/Images/switch_amp_lt.png" alt="Switched-capacitor amplifier Layout" width="600"></td>  
      </tr>  
      <tr>  
        <td>Switched-capacitor amplifier Schematic</td>  
        <td>Switched-capacitor amplifier Layout</td>  
      </tr>  
    </table>
  
- **RF Circuits: High-Pass Filter Design**  
  *October 2022 - February 2023*  
  - Designed a high-pass filter with a cutoff frequency of 1.8 GHz using AWR Microwave Office for an RF circuits course  
  - Simulated filter performance in AWR, optimizing layout to meet given frequency and attenuation specifications  
  - Translated design into a PCB layout using Altium Designer for fabrication  
  - Sent design to production and tested prototype with a network analyzer, confirming expected cutoff frequency and performance  

- **Seminar: 8-Bit Analog-to-Digital Converter Design**  
  *October 2021 - June 2022*  
  - Designed an 8-bit ADC in 180nm CMOS technology using Cadence Virtuoso to convert analog signals to digital  
  - Developed an 8-bit digital controller, simulated with ideal components to verify basic functionality  

  - *Digital controller schematic*:  
    <table>  
      <tr>  
        <td><img src="/Images/adc_controller.png" alt="Digital Controller Schematic" width="400"></td>  
      </tr>  
      <tr>  
        <td>Digital Controller Schematic</td>  
      </tr>  
    </table>  

  - Incorporated an ideal 8-bit DAC to provide reference signals for conversion  
  - Implemented a Sample-and-Hold circuit using an ideal component due to incomplete transistor-level design  
  - Designed a comparator with real transistor-level components based on “A 500-MSample/s, 6-Bit Nyquist-Rate for Disk-Drive Read Channel Applications,” validating performance in simulation alongside ideal elements  
  - *Comparator schematic*:  
    <table>  
      <tr>  
        <td><img src="/Images/adc_comparator.png" alt="Comparator Schematic" width="400"></td>  
      </tr>  
      <tr>  
        <td>Comparator Schematic</td>  
      </tr>  
    </table>  

      - *Complete ADC schematic*:  
    <table>  
      <tr>  
        <td><img src="/Images/adc_complete.png" alt="Complete ADC Schematic" width="400"></td>  
      </tr>  
      <tr>  
        <td>Complete ADC Schematic</td>  
      </tr>  
    </table>

- **Final Bachelor Project: Frequency Divider for Phase-Locked Loop**  
  *February 2022 - July 2022*  
  - Designed a frequency divider in 180nm CMOS technology using Cadence Virtuoso as part of a team project to build a PLL generating a stable 10 MHz output  
  - Developed a two-stage frequency divider, reducing a 10 MHz PLL output to 1 MHz for feedback, with a divide-by-2 stage followed by a divide-by-5 stage  
  - Created and simulated the electrical schematic, verifying functionality at nominal temperature and supply voltage (1.8V)  
  - Conducted corner analysis across temperature (-40°C to 125°C), voltage (1.62V to 1.98V), and process variations, confirming robust operation  
  - Designed the topological layout, detailing component placement and routing  
  - Extracted parasitic components from the layout and validated performance through post-layout simulations  
  - Added test circuits to facilitate verification of the fabricated chip’s operation  

  - *Frequency divider schematic and layout*:  
    <table>  
      <tr>  
        <td><img src="/Images/freq_div_schematic.png" alt="Frequency Divider Schematic" width="400"></td>  
        <td><img src="/Images/freq_div_layout.png" alt="Frequency Divider Layout" width="400"></td>  
      </tr>  
      <tr>  
        <td>Frequency Divider Schematic</td>  
        <td>Frequency Divider Layout</td>  
      </tr>  
    </table>

## Education
- **Master’s Degree in Electrical Engineering and Information Technology**  
  *Faculty of Electrical Engineering and Computing*  
  *October 2021 - July 2024*  
- **ERASMUS+ Exchange, Wrocław University of Science and Technology**  
  *October 2022 - February 2023*  
- **Bachelor’s Degree in Electrical Engineering and Information Technology**  
  *Faculty of Electrical Engineering and Computing*  
  *October 2018 - September 2021*

## Skills
- *Software*: Cadence Virtuoso, Altium Designer, MATLAB, LTspice  
- *Programming*: C, VHDL, Python  
- *Hardware*: PCB design, impedance matching, EMC testing  
- *Languages*: English (fluent)

## Development Roadmap & Projects
- This roadmap documents my learning progress and hands-on work in PCB, analog, FPGA, and ASIC design. Each project links to a dedicated folder with schematics, code, simulations, and documentation.

| Level | Category         | Project                                    | Status        | Link                        |
|-------|------------------|--------------------------------------------|---------------|-----------------------------|
| 0     | Analog           | USB-Powerd Cup Heater                      |  In Progress  |  [📁](./Projects/00_USB_Cup_Heater) |



## Interests & Volunteering
- *Interests*: Chess, gym, climbing, hiking, cycling, running, snowboarding  
- *Volunteering*:  
  - Garbage collection, Medvednica Nature Park (14.10.2023)  
  - Primary school wall painting (15.10.2021)  
  - Garden arranging, Udruga za promicanje inkluzije (16.10.2021)

## Contact
- *Phone*: +385 99 7938 007  
- *Email*: jakovvrdoljak017@gmail.com  
- *LinkedIn*: [linkedin.com/in/jakov-vrdoljak-633177138](https://linkedin.com/in/jakov-vrdoljak-633177138)
