# Inventario de Skills para Desarrollo de Modelos de Negocio y Marketing

112 SKILL.md | 485 archivos .md | 6 colecciones

## 01-business-consulting (abinauv/business-consulting)
Plugin de consultoría de gestión completo. 16 skills, 24 comandos, 5 overlays de industria.

**Skills incluidas:**
- market-research: /market-scan, TAM/SAM/SOM, landscape competitivo
- competitive-analysis: /competitor-profile, /swot, benchmarking
- financial-analysis: /financial-model, valoración, proyecciones
- pricing-strategy: /pricing-analysis, pricing tiers, WTP
- digital-transformation: /digital-assessment, madurez digital
- innovation-strategy: /innovation-assessment, portafolio I+D
- org-design: /org-design, estructura organizacional
- risk-assessment: /risk-assessment, riesgos operacionales
- talent-strategy: /talent-assessment, retención
- change-management: /change-plan, gestión del cambio
- customer-insights: /customer-analysis, churn
- cost-optimization: /cost-optimization, reducción de costos
- scenario-planning: /scenario-plan, escenarios
- strategy-deck: /strategy-deck, presentaciones estratégicas
- due-diligence: /due-diligence, debida diligencia
- market-entry: /market-entry, entrada a mercados

**Playbooks multi-paso:**
- /growth-strategy: landscape + posición + opciones + caso financiero
- /turnaround-playbook: diagnóstico + estabilización 90d + reestructuración 12m
- /ma-assessment: rationale + DD comercial + valoración + sinergias

**Instalación Claude Code:**
```
/plugin marketplace add abinauv/business-consulting
/plugin install business-consulting@abinauv-business-consulting
```

---

## 02-bmc-trusted (darren295/aifc-bmc-skill)
Business Model Canvas con etiquetado de confianza (evidenciado vs supuesto).

**Diferenciador:** cada ítem se etiqueta como evidenciado (solid) o supuesto (outline), resalta brechas entre bloques y cierra con acción siguiente.

**Instalación Claude Code:**
```
/plugin marketplace add darren295/aifc-bmc-skill
/plugin install aifc-bmc@aifc-bmc-skill
```

---

## 03-bmc-visual (RogCP/claude-skill-business-model-canvas)
BMC como visualización HTML interactiva. 9 bloques, modales, colores de marca, 20+ idiomas (incluido español).

**Tres modos:** Research (empresa existente), Ideation (idea nueva), Manual (datos propios).

**Instalación manual:**
```
Copiar carpeta a ~/.claude/skills/business-model-canvas/
```

---

## 04-mckinsey-strategy-team (limelights-amsterdam/mckinsey-strategy-team)
Equipo de agentes con 21 frameworks McKinsey. Orquestación: intake, diagnóstico, opciones competitivas, síntesis, panel verificador, decision memo.

**Requiere:** Claude Code >= 2.1.32 + agent teams habilitados.

**21 frameworks en references/:**
- Diagnóstico, mapeo de mercado, generación de opciones
- Pressure-test con panel de verificadores
- Output: decision memo listo para junta directiva

**Instalación:**
```
ln -s "$(pwd)/mckinsey-strategy-team" ~/.claude/skills/mckinsey-strategy-team
```

---

## 05-marketing-skill (arturseo-geo/marketing-skill)
Marketing operativo: campañas, funnels, ad copy, personas, positioning, go-to-market.

**Frameworks:** StoryBrand, $100M Offers, AIDA, PAS, BAB, PPPP, 4Ps, JTBD, AARRR, ICE

**Incluye references/:**
- frameworks.md: los 10 frameworks
- ad-copy.md: Google/Meta/LinkedIn Ads
- email.md: secuencias, cold outreach, subject lines
- analytics.md: UTM, atribución, KPIs, A/B testing

**Instalación:**
```
git clone https://github.com/arturseo-geo/marketing-skill.git ~/.claude/skills/marketing
```

---

## 06-alirezarezvani-business (alirezarezvani/claude-skills, parcial)
Del mega-repo de 24k estrellas, solo los dominios de negocio:

### commercial/ (8 skills)
- pricing-strategist: modelo de pricing, Van Westendorp, packaging
- deal-desk: aprobación de descuentos, redlines
- partnerships-architect: tiers de partner, revshare, GTM conjunto
- channel-economics: rentabilidad de canales, cost-to-serve
- commercial-policy: matriz de descuentos, excepciones
- rfp-responder: método Shipley, predictor de winrate
- commercial-forecaster: forecast trimestral, cohortes, confianza

### business-growth/ (5 skills)
- customer-success-manager
- sales-engineer
- revenue-operations
- contract-and-proposal-writer
- business-growth-skills (orquestador)

### c-level-advisor/ (68+ skills)
- CEO, CTO, CFO, CMO, CRO, CPO, COO, CHRO, CISO advisors
- Chief AI Officer, Chief Data Officer, Chief Customer Officer
- Executive mentor, founder-coach, board-meeting, scenario-war-room
- Competitive intel, M&A playbook, international expansion

### finance/ (4 skills)
- financial-analyst: DCF, presupuestos, forecasting
- saas-metrics-coach
- business-investment-advisor
- finance-skills (orquestador)

### business-operations/ (7 skills)
- process-mapper, vendor-management, capacity-planner
- internal-comms, knowledge-ops, procurement-optimizer

**Instalación selectiva Claude Code:**
```
/plugin marketplace add alirezarezvani/claude-skills
/plugin install commercial-skills@claude-code-skills
/plugin install business-growth-skills@claude-code-skills
/plugin install c-level-skills@claude-code-skills
/plugin install finance-skills@claude-code-skills
```

---

## Resumen de cobertura

| Fase del modelo de negocio | Skills que la cubren |
|---|---|
| Descubrimiento / ideación | 02-bmc-trusted, 03-bmc-visual, 04-mckinsey |
| Análisis de mercado | 01-business-consulting, 06-competitive-intel |
| Segmentos y propuesta de valor | 02-bmc-trusted, 01-customer-insights |
| Canales y relaciones | 05-marketing-skill, 06-channel-economics |
| Modelo de ingresos / pricing | 06-pricing-strategist, 01-pricing-strategy |
| Estructura de costos | 01-financial-analysis, 01-cost-optimization |
| Recursos y actividades clave | 06-process-mapper, 06-capacity-planner |
| Alianzas clave | 06-partnerships-architect, 06-vendor-management |
| Validación / stress-test | 04-mckinsey (panel verificador), 06-scenario-war-room |
| Go-to-market | 05-marketing-skill, 01-market-entry |
| Presentación ejecutiva | 01-strategy-deck, 06-board-deck-builder |

