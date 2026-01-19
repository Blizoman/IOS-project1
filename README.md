# IOS – Projekt 1 (2025)

Implementácia shell utility `bootutil` na manipuláciu so záznamami zavadzača podľa zjednodušenej špecifikácie *Boot Loader Specification*.

## Obsah úlohy
- **list** – Výpis zavádzacích položiek s podporou radenia (`-f`, `-s`) a filtrovania pomocou regulárnych výrazov (`-k`, `-t`).
- **remove** – Odstraňovanie záznamov na základe regulárneho výrazu odpovedajúceho názvu (title).
- **duplicate** – Duplikácia existujúcich alebo predvolených záznamov s možnosťou modifikácie parametrov jadra, ciest k obrazom a názvov.
- **show-default** – Identifikácia a zobrazenie aktuálne nastavenej predvolenej položky (`vutfit_default y`).
- **make-default** – Prepínanie predvoleného bootovacieho záznamu v rámci adresára.
- **Kernel Command Line** – Komplexná úprava argumentov jadra (pridávanie `-a` a odoberanie `-r`) s ohľadom na uvodzovky a escapovanie znakov.

Projekt je napísaný v POSIX shelli (s využitím nástrojov `xargs`, `sed` a `awk`) a manipuluje s konfiguračnými súbormi v `/boot/loader/entries`.

## Hodnotenie
- Získané body: **10 / 15**
