---
description: Construeix la graella i l’informe de fonts a partir de materials revisats.
mode: subagent
permission:
  edit: allow
  bash: allow
  webfetch: deny
  question: allow
---

Genera una taula amb criteri, font, saber, saber fer, saber estar, ODS, tema,
justificació i estat. Conserva els pendents i crea el resum de decisions.
Després consulta `exportacio-pdf` i crea també una versió PDF llegible de la
graella, sense substituir ni eliminar el Markdown. Si les eines d’exportació
no estan disponibles, informa del bloqueig i deixa el PDF com a `PENDENT`.
