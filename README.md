# 👋 Hi, I'm Noah

## 🧠 Autonomous Cognitive Architecture

Below is the current high-level system architecture for **DeltaCore**, an evolving autonomous AI runtime.

```mermaid
graph TD
    %% Interface Layer
    subgraph "Interface Layer"
        UI["Web Dashboard (React / JS)"]
        API["REST API (FastAPI / LocalDeltaAPIServer)"]
        UI <--> API
    end

    %% Cognitive Layer
    subgraph "Cognitive Layer (Metacognition & Evolution)"
        MC["Metacognition Engine (Pattern Detection)"]
        EV["Evolution Engine (Adaptive Heuristics)"]
        STRAT["Strategy Orchestrator"]
        MC --> STRAT
        EV --> STRAT
    end

    %% Logic & Continuity Layer
    subgraph "Logic & Continuity Layer"
        CONT["Continuity Engine (Narrative / Identity)"]
        ECO["Ecosystem Manager (Diversity / Exchange)"]
        COH["Coherence Enforcement"]
    end

    %% Distributed Core Engine
    subgraph "Distributed Core Engine"
        CORE["DeltaCore (Phases 0–25)"]
        MEM["MemoryRouter (Chronicle / Dewey / Bus)"]
        SWARM["Swarm Orchestrator"]
        CORE <--> MEM
        CORE <--> SWARM
        CORE <--> MC
        CORE <--> CONT
        CORE <--> ECO
    end

    %% Resource & Runtime Layer
    subgraph "Resource & Runtime Layer"
        ZMQ["ZMQ Bridge (IPC)"]
        SIL["SiliconRuntime (NPU / ONNX Runtime)"]
        GOV["NodeHealthGovernor (Auto-Scaling)"]
        SYSTEM["OS Metrics (CPU / RAM / Win32)"]
        CORE <--> ZMQ
        ZMQ <--> SIL
        CORE <--> GOV
        GOV <--> SYSTEM
    end

    %% Cluster Layer
    subgraph "Cluster Layer"
        PEER1["Peer Node 1"]
        PEER2["Peer Node 2"]
        PEERN["Peer Node N"]
        SWARM <--> PEER1
        SWARM <--> PEER2
        SWARM <--> PEERN
    end

    %% Cross-Layer Links
    API <--> CORE
