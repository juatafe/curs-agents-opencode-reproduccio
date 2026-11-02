---
name: exportacio-pdf
description: Genera una versió PDF llegible d’una graella curricular Markdown després de crear-la i abans de la revisió humana.
---

# Exportació de la graella a PDF

Usa aquesta skill quan `generador-graelles` haja creat o actualitzat una
graella curricular Markdown i el projecte demane una versió per a lectura o
impressió.

## Procediment

1. Conserva el fitxer Markdown com a font traçable.
2. Comprova que `pandoc` i `xelatex` estan disponibles abans d’exportar.
3. Genera el PDF en la mateixa carpeta d’eixides, amb el mateix identificador
   de la graella.
4. Comprova que el PDF existix i que es pot obrir.
5. Informa de la ruta del PDF i de qualsevol advertiment.

Des de l’arrel del projecte, adapta les rutes a la graella real:

```bash
pandoc "sortides/graella-curricular-3016.md" \
  --from=markdown \
  --pdf-engine=xelatex \
  --output="sortides/graella-curricular-3016.pdf"
```

En Windows PowerShell:

```powershell
pandoc "sortides/graella-curricular-3016.md" `
  --from=markdown `
  --pdf-engine=xelatex `
  --output="sortides/graella-curricular-3016.pdf"
```

Si falta alguna eina, no instal·les dependències ni presentes un PDF
inexistent. Marca l’exportació com a `PENDENT` i informa el supervisor.
