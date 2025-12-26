# invisible-languages

[![License](https://img.shields.io/github/license/theinvisiblelab/invisible-languages)](LICENSE)
[![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/theinvisiblelab/invisible-languages)

**Community-led tools and resources for making underrepresented languages usable online.**

Supporting communities to make their languages typable, findable, and sustainable in digital spaces - from keyboards and fonts to preservation and learning pathways.

[Learn more](https://theinvisiblelab.org/languages)

```mermaid
---
config:
  layout: elk
title: Visibility Pipeline for Invisible Languages
---
flowchart LR
 subgraph collabs["Collaborators"]
        C1("SILICON, Stanford")
        C2("CredOx, Oxford")
        C3("Wikimedia")
        C4("Respond")
        C5("Public Knowledge Project")
        C6("Common Crawl")
  end
 subgraph pipeline[" "]
        B["Phase 2: Encode langauge as text<br>"]
        C["Phase 3: Retrieve encoded texts<br>"]
        D["Phase 4: Amplification<br><br><i>Fairmodels<br>Librelingo</i>"]
  end
    A["Phase 1: Assess Need"] L_A_B_0@==> B
    B L_B_C_0@-- Ample text encoded --> C
    C L_C_D_0@-- Text is retrievable --> D
    D L_D_A_0@-- Feedback --> A
    D L_D_Policy_0@==> Policy["Policy Implications"]
    C1 -..- B
    C4 -..- B
    C3 -..- C
    C6 -..- C
    C5 -..- C
    C2 -..- D

    B@{ shape: db}
    C@{ shape: tag-doc}
    D@{ shape: docs}
    A@{ shape: paper-tape}
    Policy@{ shape: paper-tape}
     C1:::Rose
     C2:::Aqua
     C3:::Peach
     C4:::Rose
     C5:::Peach
     C6:::Peach
     B:::Rose
     C:::Peach
     D:::Aqua
     A:::Pine
     Policy:::Pine
    classDef Sky stroke-width:1px, stroke-dasharray:none, stroke:#374D7C, fill:#E2EBFF, color:#374D7C
    classDef Aqua stroke-width:1px, stroke-dasharray:none, stroke:#46EDC8, fill:#DEFFF8, color:#378E7A
    classDef Rose stroke-width:1px, stroke-dasharray:none, stroke:#FF5978, fill:#FFDFE5, color:#8E2236
    classDef Peach stroke-width:1px, stroke-dasharray:none, stroke:#FBB35A, fill:#FFEFDB, color:#8F632D
    classDef Pine stroke-width:1px, stroke-dasharray:none, stroke:#254336, fill:#27654A, color:#FFFFFF
    style collabs stroke:none
    style pipeline stroke:none
    linkStyle 5 stroke:#D50000,fill:none
    linkStyle 6 stroke:#D50000,fill:none
    linkStyle 7 stroke:#FFD600,fill:none
    linkStyle 8 stroke:#FFD600,fill:none
    linkStyle 9 stroke:#FFD600,fill:none
    linkStyle 10 stroke:#00C853,fill:none

    L_A_B_0@{ animation: slow } 
    L_B_C_0@{ animation: slow } 
    L_C_D_0@{ animation: slow } 
    L_D_A_0@{ animation: slow } 
    L_D_Policy_0@{ animation: slow }
```
