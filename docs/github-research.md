# GitHub packaging research

| Example | Pattern | Roger uses |
| --- | --- | --- |
| [aprocom/chatgpt-pets](https://github.com/aprocom/chatgpt-pets/blob/main/README.md) | Per-pet v2 manifest and atlas, animation examples, and manual copy instructions | Two files in a standalone `roger/` folder and previews beside the install instructions |
| [awesome-codex-pets](https://github.com/HuaqingAI/awesome-codex-pets/blob/main/docs/PET_FORMAT.md) | Install assets alongside a deeper format reference and short preview gallery | A short main README plus separate frame map and motion previews |
| [offchan42/codex-pets](https://github.com/offchan42/codex-pets) | Dedicated contact sheets and validation artifacts | A labeled contact sheet and checked-in validation results |
| [astandrik/codex-pets](https://github.com/astandrik/codex-pets/blob/main/README.md) | v1 and v2 compatibility notes and optional installer | Clear v1 and v2 downloads with simple manual install steps |
| [OpenAI’s hatch-pet reference](https://github.com/openai/skills/blob/main/skills/.curated/hatch-pet/references/codex-pet-contract.md) | Local pet directory and a relative sprite sheet path | The standard `pets/roger/` package layout |

The [current ChatGPT Pets docs](https://learn.chatgpt.com/docs/pets) specify a 1536 × 1872 transparent PNG or WebP for the web uploader. Community v2 desktop packages document 1536 × 2288 with the extra look rows. Roger ships an actual file for each route.
