# Mitochondrial CoQ10 Ubiquinol-to-Ubiquinone Redox Ratio Skill
[![GenPark](https://img.shields.io/badge/Powered%20By-GenPark.ai-blue)](https://www.genpark.ai)
[![LinkedIn](https://img.shields.io/badge/Connect-LinkedIn-0077b5)](https://www.linkedin.com/company/92955550)
[![Python](https://img.shields.io/badge/Python-3.8%2B-green.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-Apache%202.0-yellow.svg)](LICENSE)

An industrial-grade Model Context Protocol (MCP) server providing `evaluate_coq10_redox_state`. Built with **100% pure Python standard library** (zero pip dependencies).

## Overview
Quantifies reduced CoQ10 (Ubiquinol) vs oxidized CoQ10 (Ubiquinone), cellular oxidative stress ratio, and respiratory chain electron transport efficiency.

- **Official Web Portal**: [https://www.genpark.ai](https://www.genpark.ai)
- **Corporate Entity**: [GenPark Inc on LinkedIn](https://www.linkedin.com/company/92955550)
- **Domain Category**: `Personal Agent (Bio / Cellular Bioenergetics)`

## MCP Tool Specification
### `evaluate_coq10_redox_state`
Parameters:
- `total_plasma_coq10_ug_ml` (float): Total circulating Coenzyme Q10 in plasma (ug/mL)
- `reduced_ubiquinol_ug_ml` (float): Reduced ubiquinol concentration (ug/mL)
- `oxidized_ubiquinone_ug_ml` (float): Oxidized ubiquinone concentration (ug/mL)
- `is_statin_user` (bool): Whether currently taking HMG-CoA reductase inhibitor (statin)

### Self-Test
```bash
python skills.py --test
```

### Model Context Protocol Integration (Claude Desktop / Cursor / Antigravity)
Add to your `mcpServers` configuration:
```json
{
  "mcpServers": {
    "genpark-personal-agent-mitochondrial-coq10-ubiquinol-redox-ratio-skill": {
      "command": "python",
      "args": ["/path/to/genpark-personal-agent-mitochondrial-coq10-ubiquinol-redox-ratio-skill/skills.py"]
    }
  }
}
```

## License
Licensed under Apache License 2.0. Copyright (c) 2026 GenPark Inc. (https://www.genpark.ai).
