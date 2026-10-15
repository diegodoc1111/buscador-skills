# Revisa una skill antes de instalarla

La guía del reel "Tu problema tiene una skill": cómo instalar **find-skills**, el buscador que te encuentra la skill que
necesitas, y cómo revisar cualquier skill antes de dejarla entrar a tu computador con un semáforo verde, amarillo o rojo.

Hecho por [Diego Osorio](https://instagram.com/soydiegoosorio).

**[👉 Abrir la guía paso a paso](https://diegodoc1111.github.io/buscador-skills/)**

## Qué trae

- Cómo instalar find-skills solo en tu proyecto (no en todo el computador).
- 3 ejemplos para pedirle una skill a Claude Code.
- El semáforo: qué revisar antes de instalar (quién la publica, cuánta gente la usa, el panel de seguridad, qué corre en
  tu computador).
- Un prompt que pone a Claude Code a revisar una skill sin instalar ni ejecutar nada: [`docs/prompt-auditar-skill.txt`](docs/prompt-auditar-skill.txt).
- Cómo ver y quitar las skills que ya no usas.

## Deja de hacerlo todo a mano

Haz en 3 días el trabajo de todo un mes. Ten un equipo de marketing de 4 personas trabajando para ti por unos $25 al mes:
**los agentes Imperio**. Te hacen el contenido, los carruseles, los anuncios, las páginas web, los VSL, las campañas en Meta
y hasta responden tus mensajes. Sin saber de tecnología, solo copias, pegas y facturas.

Son los mismos agentes que hoy les suman entre $5.000 y $10.000 dólares extra al mes a los negocios con los que trabajo.
**[Escríbeme "IMPERIO" por Instagram](https://ig.me/m/soydiegoosorio).**

## Fuentes verificadas

Revisado el 15 de octubre de 2026.

| Dato en la página | Fuente |
|---|---|
| find-skills es de `vercel-labs/skills`, 3,9 M de instalaciones, 35 mil estrellas, en skills.sh desde el 26 ene 2026; panel: Gen Agent Trust Hub Pass, Socket Pass, Snyk Warn | https://skills.sh/vercel-labs/skills/find-skills |
| find-skills es la n.º 1 del ranking de todos los tiempos | https://skills.sh/ |
| Motivo del Warn de Snyk en find-skills: lee contenido publicado por la comunidad (Snyk lo resume como riesgo medio; el hallazgo en sí lo puntúa bajo, 0.10) | https://skills.sh/vercel-labs/skills/find-skills/security/snyk |
| Comando `npx skills add https://github.com/vercel-labs/skills --skill find-skills` (+ `-a claude-code`), probado de verdad: instala en `.claude/skills/` del proyecto | https://skills.sh/vercel-labs/skills/find-skills · https://github.com/vercel-labs/skills#readme |
| Sin `-g` instala en el proyecto; `-g` = todo el computador; `-y` = sin preguntas; `npx skills list`, `npx skills ls -g`, `npx skills remove <skill>`, `npx skills remove --global <skill>` (list y remove probados) | https://github.com/vercel-labs/skills#readme |
| find-skills prefiere 1.000+ instalaciones, desconfía de menos de 100 y de repos con menos de 100 estrellas; al instalar usa `-g -y` | https://github.com/vercel-labs/skills/blob/main/skills/find-skills/SKILL.md |
| El instalador pide Node.js 22.20 o más nuevo; licencia MIT | https://github.com/vercel-labs/skills/blob/main/package.json · https://github.com/vercel-labs/skills/blob/main/LICENSE |
| Funciona con Claude Code, Cursor, Codex, OpenCode y 75 agentes más | https://github.com/vercel-labs/skills#readme |
| Mensaje del instalador: "Review skills before use; they run with full agent permissions." | Salida real de `npx skills add` (skills 1.7.2) |
| Node.js LTS actual: v24.22.0 | https://nodejs.org/en/download |
| PowerPoint de Anthropic (`anthropics/skills` › `pptx`): 236,6 mil instalaciones; panel: Gen Pass, Socket Warn, Snyk Pass | https://skills.sh/anthropics/skills/pptx |
| Motivo del Warn de Socket en pptx: advertencia leve en `scripts/office/soffice.py` (el que abre LibreOffice) | https://skills.sh/anthropics/skills/pptx/security/socket · https://github.com/anthropics/skills/blob/main/skills/pptx/SKILL.md |
| pptx trae 15 archivos `.py` y usa paquetes de npm (`pptxgenjs`) y pip (`markitdown`, `Pillow`, `defusedxml`, `lxml`) | https://github.com/anthropics/skills/tree/main/skills/pptx · https://github.com/anthropics/skills/blob/main/skills/pptx/SKILL.md |
| Los 3 revisores (Gen Agent Trust Hub, Socket, Snyk) y las etiquetas Safe / Low / Med / High Risk del resumen de auditorías | https://skills.sh/audits |
| En la ficha de cada skill el panel dice Pass / Warn / Fail; ejemplo: `design-mobile-apps` sale "High Risk" (Snyk) en auditorías y "Fail" en su ficha | https://skills.sh/audits · https://skills.sh/designed-by-ai/skills/design-mobile-apps |
| La fecha del último cambio está en la fila "Latest commit", arriba de la lista de archivos de GitHub (find-skills: último cambio el 10 jul 2026) | https://github.com/vercel-labs/skills/tree/main/skills/find-skills |
| skills.sh no garantiza la calidad ni la seguridad de cada skill; el ranking sale de instalaciones anónimas y las skills aparecen solas | https://skills.sh/docs · https://skills.sh/docs/faq |
| Skills = instrucciones + scripts; usar solo de fuentes de confianza y auditar todos los archivos | https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview |
| `/skills` en Claude Code; skills de proyecto en `.claude/skills/` y personales en `~/.claude/skills/`; `allowed-tools` y comandos `` !`...` `` | https://code.claude.com/docs/en/skills |
| Claude Code no viene en el plan gratis; Pro: 20 USD/mes o 17 USD/mes pagando el año (200 USD); "Prices shown don't include applicable tax" | https://claude.com/pricing |
| App de escritorio de Claude | https://claude.com/download |
