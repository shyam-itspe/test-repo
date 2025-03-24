```mermaid
sequenceDiagram
    OTU-->>CPU: Serial Force Bits
    OTU-->>TIS: UG405 Reply Bits
    CPU->>OTU: Serial Reply Bits
    TIS->>OTU: UG405 Force Bits
    TIS->>OTU: Custom Message
    Detector->>OTU: Traffic Data
   Local-I/O->>OTU: Local Inputs
   RSU->>OTU: SRM
   OTU-->>TIS: Custom Message
   OTU-->>Local-I/O: Local Output
   OTU-->>RSU: SSM
   OTU-->>CDT: Timer Message
