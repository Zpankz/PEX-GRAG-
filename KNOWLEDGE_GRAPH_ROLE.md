# KNOWLEDGE_GRAPH_ROLE.md

> This file documents this repository's role in the unified
> CICM/ANZCA medical knowledge graph. The canonical skill lives at:
> `MAK95-Vault/.claude/skills/medical-knowledge-graph/`.
> The skill ingests this repository as part of its build pipeline.

## Role

Graph-RAG library providing the entity-extraction / community-detection / local-vs-global retrieval substrate. The unified graph could be loaded via NetworkXStorage or Neo4jStorage backends. Entity-extraction prompts and chunk de-duplication via mdhash inform the construction of Concept-level nodes and their CO_OCCURS_WITH edges.

## Source of truth

- Skill manifest: `MAK95-Vault/.claude/skills/medical-knowledge-graph/SKILL.md`
- Build pipeline: `scripts/build_graph.py`
- Ontology (homoiconic): `ontology/{nodes,edges,properties}.yaml`
- Self-improvement loop: `gepa/README.md`

## Branch

Development branch for this initiative: `claude/medical-knowledge-graph-UjThY`
