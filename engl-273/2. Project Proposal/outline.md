# Project Proposal Outline

## Summary

Write this last

## Introduction

## Target Market

While most hard-core enthusiasts own an emergency transponder like a Garmin InReach, many casual recreators do not. This product targets established outdoor tourism/recreation organizations who see a large volume of casual visitors and who want to add a layer of redundancy to their safety communication systems apart from cellular coverage. The AVAlink and Petal radio system is the backbone of what FLoRa Communications offers, but as the people who know it best we will offer contracting services to these organizations to evaluate their communication needs, design a network, and deploy our AVAlink product in their region to protect their patrons.
We are already in talks with the Kludahk Outdoors Club to do a trial of our product on the Kludahk Trail.

## Technical

*Problem*: When emergencies in the outdoors happen it is difficult to contact rescue and medical services because there is usually no cell coverage. 
*Current Solutions*: Satellite comms - expensive, exclusive, coverage dependent, unpredictable latency
*Proposed Solution*: LoRa mesh network - cheaper, accessible, predictable latency
*Problems*:

### Theory

- A LoRa based network provides low-cost and robust text-based communication. 
- Low power means the devices can operate on solar and battery power - perfect for the outdoors
- Having a gateway node allows access out to emergency services
- Chaining nodes together into a mesh network allows coverage to be tuned to location (IDK what this means write better)

### Scope

- A digital radio network with fixed access points that can be chained together to provide coverage for popular wilderness areas
- Browser-based user interface that can be accessed by anyone with a smart phone. No special hardware required on the user's end.
- Gateway node customization for direct contact with emergency services (location specific, requires consulting)
- Recommendations for solar and battery sizing and for network coverage.

***Not Covered***
- Location specific applications: Power, coverage, latency (number of nodes), emergency service connections.

### Methods/Procedures

#### Software/Firmware
- An open-source web-based LoRa mesh network is already available on GitHub (LoRaLink) which we are using for prototyping and may use for some demonstratable outcomes at this stage.
- We aim to develop everything in-house (AVAlink v0.0) and have to allow for customizations and reduced complexity.
  - Firmware will be written in the Rust programming language to guarantee memory safety while ensuring maximal code performance.
  - The web app will be written using .NET Blazor or Svelte which can be served as a static Web Assembly (.wasm) file, offloading most of the compute from the microcontroller to the user's smartphone. This will optimize user experience and app performance.
    - All modern mobile browsers support wasm since 2017 (caniuse.com)
  - Beta software release is planned for October 28th 2024 followed by two weeks of testing. Software testing will be developed as part of the second beta release and throughout the project.

  #### Hardware
  - We will deliver a prototype PCB (Petal v0.0) using pre-built modules by October 1st to be sent to JLCPCB
  - We will develop additional hardware testing protocols by that time as well

### Parts/Materials
- Version 0 of the Petal Board will use pre-fabbed modules for the LoRa transciever, processor, and Wi-Fi to expedite the prototyping process and avoid the complexities of desinging a radio frequency (RF) PCB. 
- For the LoRa transciever, we will use the WAVE Core1262 module which uses a Semtech 1262 transciever. It comes with the receiver balun, transmitter harmonic filters, RF switch, impendance matching circuits, and a temperature compensated crystal oscillator pre-installed. 
- For the processor and Wi-Fi, we will use the ESP32-S3-MINI-1 system on chip (SoC), which contains an ESP32-S3 dual-core microprocessor, peripherals with breakout pins, and a Wi-Fi module with in-built antenna. 
- These RF circuits would be very difficult to design on our PCB without the luxury of time to do multiple PCB revisions, so version 0 will use modules. Version 1, our future production release, will replace these with circuits designed in-house to reduce the cost of and reliance on specialty modules.

### Assumptions

1. Modules will be available throughout the prototyping stage
2. The 915MHz ISM band will remain free for use by license-exempt radio equipement.
3. Our system will not interfere with existing 915MHz systems when installed.

## Management

### Team
*Knowledge*
*Training*
*Experience*
*Skills*

### Logistics
*Suppliers*
*Parts*
*Transportation*
*Storage*

### Facilities
We will develop our product both at home and using equipment at Camosun College.

## Financial
The cost of developing the prototype.

### Cost Breakdown
***MAJOR***
- Labour: ~1680 hrs

***MINOR***
- Shipping
- 

### Total Cost

### Sources of Money?
The college has agreed to fund our project provided we have justification for our design choices.

## Conclusion
CALL TO ACTION: 