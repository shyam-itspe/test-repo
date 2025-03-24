```mermaid
sequenceDiagram
OTU->>CPU: Serial Force Bits
CPU->>OTU: UG405 Reply Bits
CPU->>TIS: Serial Reply Bits
TIS->>CPU: UG405 Force Bits
TIS->>CPU: Custom Message
Detector->>CPU: Traffic Data
Local-I/O->>CPU: Local Inputs
RSU->>CPU: SRM
CPU->>RSU: Custom Message
CPU->>Local-I/O: Local Output
CDT->>RSU: SSM
RSU->>CDT: Timer Message
