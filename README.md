> живе доки: назавжди (вхід у репо продукту) · розкладка — Р-7, `lens-governance:kernel/Lens_REPO_LAYOUT.md` §4

# KPI Lens

PWA показників KPI мережі (сімейство Lens): HTML-звіт, який генерує Excel (Power Query → VBA-експорт). Один HTML-файл.
Правила роботи — у ядрі родини [`Konst-Andre/lens-governance`](https://github.com/Konst-Andre/lens-governance) (`CLAUDE.md` · `kernel/`; Excel/PQ/VBA — `kernel/Lens_excel_protocol.md`). Цей репо самодостатній.

## Де що

| тека | роль |
|---|---|
| корінь (`index.html` · `manifest.json` · `icons/`) | **сайт** — перехідний стан, як в EquipLens: переїзд у `docs/` лише разом із перемиканням публікації |
| `lens/` | канон: `KPI_Lens_INDEX.md` (що живе) · `KPI_Lens_CHERGA.md` (відкрите) |
| `sessions/` | живі самері (стеля 2) |
| `archive/` | витіснене: специфікація імплементації категорій у Excel (Batch 15) |

## Як почати сесію

Сесія Claude Code: **першим — адаптувати репо під каркас** за `lens-governance:tools/claude-code/ADOPT.md` (тут ще нема `CLAUDE.md`, `tools/env_check.sh`, журналу аудиту — `frame_check` покаже). Далі: `lens/KPI_Lens_CHERGA.md` цілком → самері в `sessions/`.
Гейт продукту: `python3 <lens-governance>/kernel/Lens_validate.py --product .`
