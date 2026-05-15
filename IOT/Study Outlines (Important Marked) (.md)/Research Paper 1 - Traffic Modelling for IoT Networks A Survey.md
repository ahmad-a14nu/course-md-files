Research Paper 1 - Traffic Modelling for IoT Networks A Survey

*   **Traffic Modelling for IoT Networks: A Survey**
    *   **1. Introduction**
        *   Introduces network traffic models as mathematical representations of application flows used to monitor, predict, and manage network services. It contrasts time-consuming experimental investigations with mathematical analysis.
    *   **2. Major Traffic Models Developed for Traditional Computer Networks [*]**
        *   Explains that traditional network traffic exhibits self-similarity, periodicity, chaos, and burstiness. Traditional models are divided into two main categories: SRD and LRD.
        *   **2.1 Short-range Dependence (SRD) Models [*]**
            *   Based mostly on the Poisson distribution process. They require low computational complexity but struggle to capture burstiness and self-similarity in large-scale networks.
            *   *Autoregressive (AR) / ARIMA*: Uses past values/white noise to predict future traffic, but cannot capture sudden data rate changes.
            *   *Markov Model / MMPP*: Relies on current system states for low-complex reasoning; good for voice/data but incapable of predicting long-range IoT traffic.
        *   **2.2 Long-range Dependence (LRD) Models [*]**
            *   Designed to better represent the self-similarity of network traffic (where a part of the data is similar to the whole).
            *   *ON-OFF Model*: Source is either continuously transmitting or off; fails to account for varying independent data sources.
            *   *Fractional Brownian Motion*: Captures autocorrelation but fails with non-Gaussian marginal distributions.
            *   *M/G/∞ Queuing Model*: Simulates packet transfers but assumes traffic is always busy, lacking burstiness representation.
            *   *FARIMA*: Measures self-similarity using the Hurst parameter but struggles to capture severe traffic burstiness.
        *   **2.3 Discussion**
            *   Concludes that traditional SRD and LRD models are fundamentally unsuitable for IoT networks because they cannot accurately model the massive variety, burstiness, and dynamic nature of modern device traffic.
    *   **3. Major IoT Applications and Their Traffic Characteristics**
        *   **3.1 Intelligent Living and Buildings**
            *   Covers home automation and building monitors. Characterized by small/medium networks, infrequent/irregular transmission rates, and varied power sources (batteries/fixed).
        *   **3.2 Smart Health [*]**
            *   Covers medical monitoring and identity/drug management. Characterized by highly critical, regular, and frequent data uploads with a strong need for low data loss, low latency, and high security.
        *   **3.3 Intelligent Environment**
            *   Covers ambient sensors (wildlife, pollution, forest fires). Characterized by medium/large networks, regular monitoring but irregular emergency traffic, heavily reliant on energy-efficient or renewable power.
        *   **3.4 Smart Grid**
            *   Covers utility (water/electricity) metering. Characterized by medium/large networks, regular periodic traffic loads, fixed power supplies, and relatively low data transmission rates.
        *   **3.5 Smart Transport and Mobility**
            *   Covers vehicle automation and traffic monitoring. Characterized by strict Quality of Service (QoS) and low-latency requirements for accident prevention, with highly variable data rates.
    *   **4. Challenges and Potential Research Directions in Modelling IoT Network Traffic [*]**
        *   **4.1 Massive Heterogeneous Traffic [*]**
            *   *Challenge*: Dealing with 48 billion devices generating a mix of tiny regular payloads and massive bursty payloads. 
            *   *Potential Solution*: Integrating Poisson-based models (for regular traffic) with Pareto-based models (for burst/heavy-tailed traffic).
        *   **4.2 Device and Application Heterogeneity**
            *   *Challenge*: Devices use completely different network types (wired/wireless) and have vastly different power constraints. 
            *   *Potential Solution*: Developing models that integrate mobility patterns with energy consumption policies across heterogeneous networks.
        *   **4.3 Dynamic Traffic Load [*]**
            *   *Challenge*: IoT devices are mobile and placed in harsh environments, making their data flows highly dynamic in both space and time.
            *   *Potential Solution*: Utilizing supervised and reinforcement machine learning algorithms to train models on dynamic conditions and predict future traffic.
        *   **4.4 Traffic Model Scalability [*]**
            *   *Challenge*: The sheer volume of devices and different communication protocols (ZigBee, LoRa, RFID) makes scaling models difficult.
            *   *Potential Solution*: Using scalable AI models, specifically Long Short-Term Memory (LSTM) neural networks, which can continuously learn and adapt to new network technologies in real-time.
    *   **5. Conclusion**
        *   Summarizes that the massive increase and heterogeneity of connected devices dictate the future of IoT traffic modeling. Extensive combination of existing mathematical models with advanced Machine Learning (ML) techniques is the primary path forward.