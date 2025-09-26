````markdown
```mermaid
flowchart TB
    %% Define Main Components
    subgraph BoardManagement[USSF Board Management Process]
        direction TB
        subgraph Phase1[Phase 1: Pre-Board Planning]
            A1[Determine Board Type and Policy]
            A2[Identify Board President and Panel Members]
            A3[Define Organizations Involved]
            A4[Build Plan of Action and Milestones (PoAM)]
            A5[Schedule Stakeholder Meetings]
        end

        subgraph Phase2[Phase 2: Preparation]
            B1[Release Initial PSDM]
            B2[Schedule Townhalls]
            B3[Determine Candidate Pool]
            B4[Send Target Messages]
            B5[Conduct Initial Leveling Brief]
        end

        subgraph Phase3[Phase 3: Execution]
            C1[Conduct Pre-Run Day]
            C2[Execute Board Activities]
            C3[Capture Board Comments and Notes]
            C4[Document Final Results]
            C5[Conduct End-of-Day Tag-Ups]
        end

        subgraph Phase4[Phase 4: Post-Board Actions]
            D1[Release Final Results]
            D2[Coordinate Final Service Transfers]
            D3[Conduct Final Townhalls]
            D4[Capture Lessons Learned]
        end
    end

    %% Define Datasets
    subgraph Datasets[Datasets]
        DS1[Board Population Dataset]
        DS2[Board Messages Dataset]
        DS3[Board Matching Dataset]
        DS4[Board Results Dataset]
        DS5[Statement of Intent Dataset]
        DS6[Board Scoring Dataset]
    end

    %% Define Systems
    subgraph Systems[Systems]
        SYS1[Envision]
        SYS2[STARS]
        SYS3[MyVector]
        SYS4[Salesforce]
    end

    %% Connect Phases to Datasets
    A1 --> DS1
    A2 --> DS1
    A3 --> DS1
    A4 --> DS1
    A5 --> DS1
    B1 --> DS2
    B2 --> DS2
    B3 --> DS1
    B4 --> DS2
    B5 --> DS1
    C1 --> DS6
    C2 --> DS6
    C3 --> DS6
    C4 --> DS4
    C5 --> DS4
    D1 --> DS4
    D2 --> DS4
    D3 --> DS2
    D4 --> DS5

    %% Connect Datasets to Systems
    DS1 --> SYS1
    DS2 --> SYS1
    DS3 --> SYS1
    DS4 --> SYS1
    DS5 --> SYS1
    DS6 --> SYS2
    DS6 --> SYS3
    DS2 --> SYS4
```
````