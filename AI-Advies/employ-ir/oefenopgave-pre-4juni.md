# Oefenopgave — Voorbereiding op 4 juni

Doel: voor 4 juni een mini-tool bouwen die je op dag 1 bij Employ IR al kan laten zien. Niet perfect — werkend.

---

## De opdracht: CV Quickscan Tool

Bouw een simpele tool waarbij je een CV (als tekst) erin gooit en er automatisch uitkomt:

1. **Top 5 skills** van de kandidaat
2. **Samenvatting** in 3 zinnen (geschikt om aan een werkgever te sturen)
3. **Match-score** (0-10) tegen een vooraf ingevulde vacature
4. **Aanbeveling**: geschikt / twijfel / niet geschikt

---

## Drie fases

### Fase 1 — Prompting (dag 1-2)
Geen code. Gewoon in Claude.ai of Claude Code terminal.

Schrijf een prompt die:
- Een CV-tekst als input neemt
- De 4 outputs hierboven geeft in een vast format
- Consistent werkt op 3 verschillende nep-CV's die je zelf verzint

**Je slaagt als:** je de prompt 3x runt en elke keer een bruikbaar resultaat krijgt zonder dat je handmatig iets hoeft bij te sturen.

---

### Fase 2 — Claude Code (dag 3-5)
Bouw een simpel Python-scriptje dat:
- Een CV-tekst als input accepteert (gewoon copy-paste in terminal is prima)
- Jouw prompt uit Fase 1 automatisch uitvoert via de Claude API
- De output netjes print in de terminal

Gebruik de Anthropic SDK. Vraag Claude Code om je te helpen als je vastloopt — maar probeer eerst zelf.

**Je slaagt als:** je `python cv_scan.py` typt, een CV-tekst plakt, en de output eruit rolt.

---

### Fase 3 — Design (dag 6-7)
Maak de output presentabel. Twee opties:

**Makkelijk:** laat Claude Code een simpele HTML-pagina genereren die de output mooi weergeeft — naam kandidaat, skills als badges, score als getal, aanbeveling in kleur (groen/oranje/rood).

**Uitdaging:** maak er een mini-webformulier van waarbij je de CV-tekst in een tekstvak plakt en op "Scan" klikt.

**Je slaagt als:** je het aan Rinus kan laten zien zonder dat het eruit ziet als een terminal-output.

---

## Waarom deze opgave

- **Fase 1** traint je prompting — leren hoe je Claude betrouwbaar dezelfde output laat geven
- **Fase 2** traint Claude Code — API calls, input/output, scripts bouwen
- **Fase 3** traint design met AI — iets bruikbaars en mooi maken zonder designer te zijn

En het resultaat is iets wat je op 4 juni letterlijk kan openen bij Employ IR en zeggen: *"Kijk, dit heb ik alvast gebouwd — dit kan ik voor jullie inrichten op P-net data."*

---

## Hulpbronnen

- Anthropic SDK docs: via Claude Code (`/help` of gewoon vragen)
- Nep-CV's verzinnen: vraag Claude om 3 fictieve CV's van ZA-technici te genereren
- Vasthaken? Zeg het gewoon hier, dan helpen we verder

---
*Aangemaakt: 2026-05-26*
