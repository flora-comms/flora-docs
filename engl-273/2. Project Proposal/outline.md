# Project Proposal Outline

## Summary

Write this last

## Introduction

## Technical

*Problem*: When emergencies in the backcountry happen it is difficult to contact rescue and medical services because there is usually no cell coverage. 
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
  - Beta software release is planned for October 28th 2024 followed by two weeks of testing. Software testing will be developed

  #### Hardware
  - We will deliver a prototype PCB (Petal v0.0) using pre-built modules by October 1st to be sent to JLCPCB
  - We will develop hardware testing protocols by that time as well

### Parts/Materials


### Assumptions


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
Things we need to arrange and use.

## Financial

### Cost Breakdown

### Total Cost

### Sources of Money?

## Conclusion
CALL TO ACTION: 