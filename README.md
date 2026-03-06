Multi-Agent Systems for Sustainable Product Design Specifications

Overview
This repository contains the complete dataset and supplementary materials for the research paper: "Multi-Agent Systems Improve Structural Quality of AI-Generated Sustainable Product Design Specifications"
Paper Status: Submitted for review
DOI: [To be added upon publication]

Abstract
This study investigates whether adversarial multi-agent system (MAS) architectures can enforce structural-functional balance in AI-generated product design specifications by simulating professional engineering team deliberation. We compared three generative workflows (zero-shot, iterative single-agent, adversarial MAS) across eleven consumer products. Results demonstrate that MAS achieved substantially higher Axiomatic Realisability Index (ARI) across all products (mean 0.46 vs. 0.18, p<0.001, Cohen's d=1.75, 100% directional consistency), while single-agent iteration provided minimal benefit over baseline (p=0.48).

Repository Structure
├── README.md                          # This file
├── data/
│   ├── raw/                          # Raw generated specifications
│   │   ├── vacuum_cleaner/
│   │   │   ├── ZeroShot_PDS.csv
│   │   │   ├── PDS_2.csv             # Single-agent Iteration 1
│   │   │   ├── PDS_3.csv             # Single-agent Iteration 2 (final)
│   │   │   ├── MAS_Iteration_1_Output.csv
│   │   │   ├── MAS_Iteration_2_Output.csv
│   │   │   ├── MAS_Iteration_1_AllCritiques.csv
│   │   │   ├── MAS_Iteration_1_MasterCritique.csv
│   │   │   ├── MAS_Iteration_1_TradeOffs.csv
│   │   │   ├── MAS_Iteration_2_AllCritiques.csv
│   │   │   ├── MAS_Iteration_2_MasterCritique.csv
│   │   │   └── MAS_Iteration_2_TradeOffs.csv
│   │   ├── electric_kettle/
│   │   ├── cordless_drill/
│   │   ├── coffee_machine/
│   │   ├── hair_dryer/
│   │   ├── portable_blender/
│   │   ├── bladeless_fan/
│   │   ├── electric_toothbrush/
│   │   ├── electric_wheelchair/
│   │   ├── folding_bicycle/
│   │   └── lawn_mower/
│   ├── processed/                    # Processed analysis results
│   │   ├── quantitative_metrics_all_products.csv
│   │   └── expert_evaluation_results.csv
│   └── expert_evaluation/           # Expert evaluation materials
│       ├── Expert_Reader_Packet.html
│       ├── Expert_Scoring_Sheet.xlsx
│       └── expert_ratings_raw.csv
│   ├── prompts/
│   │   ├── baseline_prompt.txt       # Zero-shot generation prompt
│   │   ├── single_agent_critique.txt # Single-agent critique prompt
│   │   ├── single_agent_revision.txt # Single-agent revision prompt
│   │   ├── mas_agent_1_material.txt  # Material & Design Expert prompt
│   │   ├── mas_agent_2_production.txt # Production Engineer prompt
│   │   ├── mas_agent_3_inservice.txt  # In-Service Expert prompt
│   │   ├── mas_agent_4_circularity.txt # Circularity Expert prompt
│   │   ├── mas_agent_5_chief.txt      # Chief Engineer prompt
│   │   └── mas_revision.txt           # MAS revision prompt
├── supplementary/
│   ├── engineering_lexicon.csv        # Complete 847-term lexicon
└── LICENSE                            # MIT License
