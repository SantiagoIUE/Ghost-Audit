# 👻 Ghost Audit — Exorcista de Legacy

## 💡 La Idea Core
Un Power de Kiro que lee un proyecto viejo, explica en español simple qué hace el
negocio y dibuja un mapa de riesgo (rojo = frágil, verde = migrado). Después lo
moderniza por etapas, con un humano que valida el alcance y aprueba el plan antes
de tocar código.

Problema que resuelve: las empresas tienen sistemas viejos que nadie entiende,
cuestan caro de mantener y dan miedo de modificar.

## 🛠️ Stack Tecnológico
- IDE / agente: Kiro (Power con plugin.json, mcp.json, skills/, dev.kiro/)
- Frontend: React + Vite + React Flow (mapa de módulos)
- Backend: Node.js (lee el repo y genera el análisis en JSON)
- Datos: archivos JSON (sin base de datos, para ir rápido)
- Proyecto viejo de ejemplo: [JavaScript / PHP]
- Control de versiones: GitHub

## 📋 Alcance Mínimo Viable (MVP)
Debe estar sí o sí:
1. Análisis de un repo de ejemplo -> JSON con módulos, dependencias y riesgo
2. Mapa visual con colores de riesgo
3. Explicación en español simple de al menos 1 módulo
4. Pantalla de aprobación humana (alcance y plan)
5. Migración real de al menos 1 módulo
6. Reporte final antes/después

Fuera del MVP (se descarta si no alcanza):
- Varios lenguajes
- Ataque de seguridad en entorno de prueba (extra)
- Métricas avanzadas de rendimiento
- Login de usuarios

## ⏳ Cronograma por Horas
- Bloque 1 (primeras ~5h): repo, estructura, cuentas de Kiro, proyecto viejo de ejemplo, mockup.
- Bloque 2 (siguientes ~12h): backend de análisis, mapa, aprobación, Power de Kiro, migrar 2-3 módulos.
- Bloque 3 (últimas ~5h): pruebas, reporte antes/después, ensayo de demo x3, video/pitch, plan B.

## 🤝 División de Roles
- [Ingeniero]: análisis del repo, grafo de dependencias, migración, Power de Kiro.
- [Santiago]: proyecto de ejemplo, interfaz del mapa, aprobación humana, reporte, guion de demo y pitch.
- Ambos: pruebas y ensayo final.
- Una rama por funcionalidad; merge a main solo con la funcionalidad probada.

## 🔄 Flujo (humano valida alcance y plan)
1. Work item: "Modernizar este proyecto"
2. Contexto: el agente lee el repo y las reglas de negocio
3. Alcance: mapa de impacto -> humano valida
4. Plan: etapas ordenadas por riesgo -> humano aprueba
5. Código: migra un módulo por etapa
6. Learning: actualiza reporte y mapa

El grafo sugiere impacto, no confirma alcance ni reemplaza la revisión del equipo.

## 🎬 Demo (3-4 min)
1. Proyecto viejo + mapa en rojo
2. Explicar un módulo en español simple
3. Mostrar el plan y aprobarlo en vivo
4. Migrar un módulo: pasa de rojo a verde
5. Reporte final

## ⚠️ Riesgos
- Cubrir muchos lenguajes -> usar solo uno
- Hallazgos sin evidencia -> cada uno con archivo y línea
- Dejar la demo para el final
- Probar solo contra el repo de ejemplo, nunca contra sistemas ajenos

## 📌 Pendientes por definir
- [ ] Duración y reglas del hackathon
- [ ] Lenguaje del proyecto de ejemplo
- [ ] Cuentas y acceso a Kiro listos
- [ ] Horario de ensayo de la demo
