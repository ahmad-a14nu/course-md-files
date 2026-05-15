# LoRa® and LoRaWAN®

## 1. What are LoRa® and LoRaWAN®? [*]
This section introduces LoRa as a physical wireless radio frequency (RF) modulation technology for Low-Power Wide-Area Networks (LPWANs), offering long-range and ultra-low power capabilities. LoRaWAN is the open networking protocol (MAC layer) built on top of LoRa, designed to connect battery-operated devices in a star topology. 

## 2. Radio Modulation and LoRa [*]
Explains how LoRa uses a proprietary Spread Spectrum technique based on Chirp Spread Spectrum (CSS). It trades data rate for sensitivity, allowing signals to be transmitted over long distances using very little power.
* **2.1. Key LoRa Modulation Properties [*]:** Introduces Spreading Factors (SF7 to SF12). A higher Spreading Factor increases the range and reliability of a signal but decreases the data rate and increases the "Time on Air" (TOA).
* **2.2. LoRa Modulation Characteristics:** Covers regional parameters and channel plans, such as the North American use of 125 kHz and 500 kHz uplink/downlink channels, and how the modulation resists interference and Doppler shifts.
* **2.3. Data Collisions and Spreading Factor Orthogonality [*]:** Explains that signals using different Spreading Factors on the same channel do not collide (they are orthogonal/invisible to each other). It also introduces Adaptive Data Rate (ADR) to optimize device battery life and network capacity.

## 3. LoRaWAN Network Fundamentals [*]
Breaks down the entire end-to-end architecture (the technology stack) of a LoRaWAN network.
* **3.1. LoRaWAN Network Elements: An Introduction:** An overview of the physical and software components that make up the network.
    * **3.1.1. LoRa-based End Devices:** Autonomous sensors or actuators that collect data and transmit it wirelessly.
    * **3.1.2. LoRaWAN Gateways [*]:** Devices that receive RF signals from end devices and simply forward them over an IP network (Wi-Fi, Ethernet, Cellular) to the Network Server. They do not read the data payload.
    * **3.1.3. Network Server [*]:** The "brain" of the network. It manages data routing, deduplication of messages received by multiple gateways, frame authentication, and the Adaptive Data Rate (ADR).
    * **3.1.4. Application Servers:** Securely handle, decode, and manage the actual sensor data (the application payload).
    * **3.1.5. Join Server:** Manages the over-the-air activation (OTAA) process and securely derives encryption keys.
* **3.2. LoRaWAN Network Elements: Device Commissioning [*]:** Details how devices are added to the network. It contrasts **Over-the-Air Activation (OTAA)** (secure, dynamic, preferred) with **Activation by Personalization (ABP)** (hardcoded, static).
* **3.3. LoRaWAN Network Elements: Security [*]:** Explains the network's 128-bit AES end-to-end encryption and mutual authentication.
    * **3.3.1. The Join Procedure [*]:** Describes how the device and network exchange requests and accepts to generate unique Network Session Keys (NwkSKey) and Application Session Keys (AppSKey) so the network server and application server are kept separate and secure.
* **3.4. Device Classes: A, B and C [*]:** The three communication profiles dictating how devices receive data.
    * **3.4.1. Class A Devices [*]:** Highly battery-optimized. The device sleeps most of the time, transmits an uplink, and briefly opens two receive windows (Rx1, Rx2). The network cannot wake it up.
    * **3.4.2. Class B Devices [*]:** Offers scheduled receive windows (ping slots). Good for actuators that need to be reached at predictable times.
        * **Class B Beacons:** The network gateways send periodic GPS-synchronized beacons so the end device can align its internal clock to know exactly when to listen.
    * **3.4.3. Class C Devices [*]:** Always listening (receive windows are always open unless transmitting). Offers the lowest latency but consumes the most power (usually mains-powered, like streetlights).

## 4. The LoRa Alliance
Briefly mentions the organization of over 500 member companies responsible for standardizing the LoRaWAN protocol and ensuring device interoperability and certification.

## Disclaimer
Standard legal text stating Semtech's limitations of liability regarding the use of their products and the information in the document.