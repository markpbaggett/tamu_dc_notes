DPMT Workflows
##############

This document is meant to serve as a flowchart to understand complex DPMT processes. It is derived from notes in the
`DPMT Workflow in the Google Drive <https://docs.google.com/document/d/10B31IKpucxNgtp-DlcKcI4ylbrmm4IfawUMZwAJxLjs/edit>`_
and current issues in completing DPMT projects.  It is highly experimental and may change when thinking becomes more
clear.

Flowchart
---------

.. mermaid::

    ---
    title: DPMT Workflow
    ---
    graph TD
        START --> PREPROCESS
        subgraph PREPROCESS
            S[Stakeholder] -- Submits IDEA Document --> D[Mark]
            S -- Submits Inventory --> D
            S -- Submits Access Rights Review --> D
            S -- Confirms Content Review --> D
            D -- Reviews Submission --> S
            D -- Notifies Docs are Ready for Review --> DPMT[DPMT Members]
            DPMT -- Completes Feasibility Report --> D
            D -- Schedules --> KICKOFF
        end
        subgraph KICKOFF
            J[Jeanette] --  Define Metadata --> ST[Stakeholder]
            M[Micah] -- Determine Repository --> ST
            JO[John] -- Define Access Restrictions --> ST
            SE[Sean] -- Determine Digitization --> ST
            M[Mark] -- Adds Project --> CHK[[Checklist]]
            MEM[DPMT Members] -- If Platform --> HT{HathiTrust}
            HT -- Yes --> HATHITRUST
            HT -- No --> NORMAL
        end
        subgraph HATHITRUST
            MHT[Mark] -- Writes --> HTDASI[[DASI]]
            MHT -- Writes --> HTCS[[Cover Sheet]]
            MHT -- Pursues --> HTCC[[Creative Commons Declaration]]
            MHT -- Contacts --> HTR[HathiTrust]
        end
        subgraph NORMAL
            NST[Stakeholder] -- Sends Items --> DISC[DISC]
            DISC -- Digitizes --> Assets
            Assets -- Added to --> CIFS[[CIFS]]
        end



.. mermaid::

    ---
    title: DPMT Workflow
    ---
    graph TD
        Start --> PRE((Preprocess))
        PRE --> S[Stakeholder]
        S[Stakeholder] -- Submits IDEA Document --> D[Director, Digital Collections]
        S -- Submits Inventory --> D
        S -- Submits Access Rights Review --> D
        S -- Confirms Content Review --> D
        D -- Reviews Submission --> S
        D -- Notifies Docs are Ready for Review --> DPMT[DPMT Members]
        DPMT -- Completes Feasibility Report --> D
        D -- Schedules Kickoff --> REV((Review))
        REV --> KICK[[Kickoff Meeting]]
        subgraph KICK
            J[Jeanette] --> S
        end




Test
----

.. mermaid::

  graph TB
    sq[Square shape] --> ci((Circle shape))

    subgraph A
        od>Odd shape]-- Two line<br/>edge comment --> ro
        di{Diamond with <br/> line break} -.-> ro(Rounded<br>square<br>shape)
        di==>ro2(Rounded square shape)
    end

    %% Notice that no text in shape are added here instead that is appended further down
    e --> od3>Really long text with linebreak<br>in an Odd shape]

    %% Comments after double percent signs
    e((Inner / circle<br>and some odd <br>special characters)) --> f(,.?!+-*ز)

    cyr[Cyrillic]-->cyr2((Circle shape Начало));

     classDef green fill:#9f6,stroke:#333,stroke-width:2px;
     classDef orange fill:#f96,stroke:#333,stroke-width:4px;
     class sq,e green
     class di orange


