# Projecte de graelles curriculars verificables

Sistema multiagent per preparar graelles curriculars a partir de fonts oficials,
relacionant criteris, sabers, ODS i temes transversals.

## Què fa

1. Rep una petició sobre un mòdul o una assignatura.
2. Prepara un pla i espera l’aprovació.
3. Extrau informació de fonts registrades.
4. Relaciona criteris, sabers, ODS i temes transversals.
5. Genera una graella i un informe de fonts.
6. La verifica amb un agent independent.
7. La deixa preparada per a revisió humana.

## Estructura

- `AGENTS.md`: regles generals del projecte.
- `fonts/`: registre, portals oficials i procediment de verificació.
- `.opencode/agents/gestor-fonts.md`: localitza i registra fonts abans de l’extracció.
- `.opencode/agents/assessor-disseny-curricular.md`: aplica el llibre de disseny curricular com a orientació bibliogràfica, sense confondre’l amb normativa.
- `.opencode/agents/verificador-context.md`: comprova els catàlegs abans de fer preguntes.
- `.opencode/skills/progres-i-represa/SKILL.md`: controla memòria, represa i convergència.
- `.opencode/skills/issue-workflow/SKILL.md`: defineix issues, branques, PR i merge.
- `dades/`: catàlegs, estat de les fonts i plantilles de treball, inclosos `estat-catalogs.md`, `cicles-fp.md`,
  `referencies-cicles.md`, `moduls-fp.md` i `cursos-especialitzacio.md`.
- `sortides/`: esborranys, graelles i informes.
- `.opencode/agents/`: papers especialitzats.
- `.opencode/skills/`: procediments reutilitzables.

## Primera petició

Obri OpenCode en aquesta carpeta i demana al `supervisor` que prepare un pla
per al mòdul o assignatura que vulgues treballar. El supervisor ha d’esperar
`PLAN APPROVED` abans de crear o editar fitxers. Les preguntes amb opcions es mostren amb el selector interactiu d’OpenCode.

## Descarregar i provar el projecte

Si vols provar el projecte sense escriure els fitxers a mà, descarrega’l amb
Git. Obri una terminal en la carpeta on vulgues guardar-lo i executa:

```bash
git clone https://github.com/juatafe/curs-agents-opencode-reproduccio.git
cd curs-agents-opencode-reproduccio
```

En Windows PowerShell, les mateixes ordres són:

```powershell
git clone https://github.com/juatafe/curs-agents-opencode-reproduccio.git
Set-Location .\curs-agents-opencode-reproduccio
```

Després, obri OpenCode en aquesta carpeta i segueix la secció «Primera
petició». El projecte inclou les configuracions, les dades de treball i unes
eixides d’exemple perquè pugues inspeccionar el resultat abans de generar-ne
un de nou. No inclou credencials ni dependències instal·lades.

### Abans de començar

Necessites:

- Git.
- OpenCode instal·lat i un proveïdor amb un model disponible.
- Node.js només si vols activar les extensions o la configuració MCP que ho
  necessite; no cal per a llegir els fitxers ni revisar les eixides incloses.

Les fonts remotes poden canviar i els annexos sobre GitHub, MCP i workflows
descriuen ampliacions opcionals. No s’activen automàticament en clonar aquest
projecte.

### Primera prova segura

Després de clonar-lo, obri OpenCode exactament en la carpeta del projecte i
demana una operació de lectura, per exemple:

```text
Llig el README.md i enumera les carpetes del projecte. No edites cap fitxer.
```

Després, demana al `supervisor` que prepare un pla per a una graella
curricular. No autoritzes cap canvi fins que el supervisor mostre literalment
`PLAN APPROVED`. Una comprovació mínima és que la petició de lectura no haja
modificat cap fitxer i que el pla identifique les fonts i els criteris que
caldria revisar.

## Estat del projecte

La configuració inicial és una base didàctica. Les fonts, els criteris i les
relacions curriculars s’han d’omplir i revisar per a cada ensenyament.
