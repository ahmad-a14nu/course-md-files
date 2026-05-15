# 3 Wireless Protocols and Technologies for the Internet of Things

## 3.1 WPAN TECHNOLOGIES FOR IOT [*]

### 3.1.1 IEEE 802.15.4 [*]
- Layered Architecture (Physical and MAC layer data flow)
- FCC-Allocated Frequencies for Industrial, Scientific, and Medical (ISM) Applications
- **Key MAC functions defined in the standard:** [*]
  - 1. Beacon Management
  - 2. Channel Access
  - 3. Frame Formatting
  - 4. Acknowledgments
  - 5. Network Topology (Star and Peer-to-Peer)
- **Limitations of IEEE 802.15.4 standard:** [*]
  - 1. Limited Range
  - 2. Limited Throughput
  - 3. Limited Scalability
  - 4. Limited Interoperability
  - 5. Limited Security
- **Common uses of IEEE 802.15.4 in IoT:**
  - 1. Smart Homes
  - 2. Industrial Automation
  - 3. Smart Cities
  - 4. Healthcare
  - 5. Agriculture

### 3.1.2 Zigbee [*]

- **Zigbee Architecture (Figure 3.3)** [*]
  - Physical Layer
  - Media Access Control (MAC)
  - Network Layer
  - Application Support Sublayer (APS)
  - Security Services
  - Application Framework
    - App Objects
  - Zigbee Device Object (ZDO)
    - ZDO Public Interface
    - ZDO Management

- **Zigbee NWK Frame Format (Table 3.2)**
  - Frame control
  - Destination address
  - Source address
  - Radius
  - Sequence numbers
  - Routing Fields
  - Frame payload

- **Field Size of Zigbee NWK Format (Table 3.3)**
  - Frame control
  - Destination endpoint
  - Cluster identifier
  - Application profile identifier
  - Source endpoint
  - Counter
  - Payload

- **Zigbee Node Types (Figure 3.4)** [*]
  - 1) Zigbee End Device (ZED)
  - 2) Zigbee Route (ZR)
  - 3) Zigbee Coordinatiors (ZC)
  - 4) Zigbee Network Layer (NWK)
  - 5) Zigbee APS Layer

### 3.1.3 HART
- **Key aspects of HART well-suited for IoT:**
  - 1. Compatibility with Legacy Systems
  - 2. Bidirectional Communication
  - 3. Low Bandwidth Requirements
  - 4. Security
  - 5. Standardization

### Z-Wave Network (Covered in Text/Diagrams before 3.1.6)
- Primary Controller (Master Mode)
- Secondary Controller
- Network Registration Process (Inclusion and Exclusion)

### 3.1.6 Bluetooth/BLE (Bluetooth Low Energy) [*]
- **Key aspects of BLE well-suited for IoT:** [*]
  - 1. Low Power Consumption
  - 2. Short-Range Communication
  - 3. Interoperability
  - 4. Security
  - 5. Compatibility
- Disadvantages of BLE (Low bandwidth, limited range, gateway requirement, interference)
- **Software levels in BLE architecture:** [*]
  - Application
  - Host
  - Controller