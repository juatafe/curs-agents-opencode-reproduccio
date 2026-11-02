# Guia per a agents

## Flux de treball

- Abans de crear o editar fitxers per a una nova petició, demana al `supervisor` que prepare el pla i espera exactament `PLAN APPROVED`.
- Tracta les fonts i els catàlegs com a dades de treball: revisa `fonts/` i `dades/` abans de generar contingut curricular; deixa els resultats a `sortides/`.
- Usa els papers especialitzats de `.opencode/agents/` i els procediments de `.opencode/skills/` quan la petició els afecte, especialment `progres-i-represa` per a memòria i represa i `issue-workflow` per al flux d’issues, branques i PR.

## Estructura rellevant

- `fonts/` registra portals oficials i el procediment de verificació.
- `dades/` conté els catàlegs i plantilles; `sortides/` conté esborranys, graelles i informes.
- `.opencode/agents/assessor-disseny-curricular.md` és orientació bibliogràfica, no normativa; `.opencode/agents/verificador-context.md` comprova els catàlegs abans de preguntar.

## Verificació

- Aquest repositori no té manifests, scripts, tests, CI ni configuració de lint, typecheck o build. No inventes ordres de validació: comprova manualment els fitxers modificats i les fonts referenciades.
