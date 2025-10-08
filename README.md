RDB to Knowledge graph pipeline.

This project converts relational database schemas into graph-based, LLM-readable formats.
It includes a sequence of scripts that extract, transform, and prepare data for both visualisation and LLM reasoming.

Contributions:
The schema extraction (extract.ipynb) was completed by Felix. Evanna completed the mapping_specs.py
and llm_prompts.py, I refined both the scripts and I implemented and tested the remaining scripts to
check that the full pipeline wrked successfully from extract to visualisation.

Files:
extract.ipynb
schema_to_graph.py
mapping_specs.py
llm_prompts.py
mapping_to_yFiles.py

How to run:
Run the scripts in the following order from the root directory.
- extract.ipynb
- schema_to_graph.py
- mapping_specs.py
- llm_prompts.py
- mapping_to_yFiles.py

Folder outputs:
- artifacts/runs/spider/        : Stores schema.json files generated from extract.ipynb.
- artifacts/runs/graph_schemas/ : Contains generated graph JSON files.
- mapping_specs/                : Contains mapping specification JSON files.
- llm_prompts/                  : Stores text-based LLM prompts.
- yfiles_graphs/                : Stores yFiles compatible JSON files for visualisation.
