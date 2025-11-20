# MainE1 — N² Overmind

The hierarchical recursion engine I designed in December 2024.

This is the real thing.

`maine1_n2_overmind.py` is a drop-in module.
Add it to any CrewAI / LangGraph / Swarms project.
It will make your agent stop outputting garbage.

It forces:
- 6 sub-personalities with tone anchors + forced SIM
- ODAI validation with private alignment score
- Automatic repair loops if score <9
- Final clean markdown only when perfect

Just do:
```python
from n2_overmind import run_n2_overmind

answer = run_n2_overmind("your query here")
