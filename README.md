
**Ecosistema SaaS de Salud Digital Pediátrica**

*Detección temprana · Rehabilitación adaptativa · Impacto real*

[![TRL](https://img.shields.io/badge/TRL-5%20→%209-teal?style=flat-square)](https://github.com/earlify-health/wiki/Arquitectura-Tecnica)
[![MDR](https://img.shields.io/badge/MDR-Clase%20IIa%20%7C%20Clase%20I-blue?style=flat-square)](https://github.com/earlify-health/wiki/Estrategia-Regulatoria)
[![AI Act](https://img.shields.io/badge/AI%20Act-Alto%20Riesgo%20(Anexo%20III)-orange?style=flat-square)](https://github.com/earlify-health/wiki/Estrategia-Regulatoria)
[![License](https://img.shields.io/badge/License-Earlify%20SAL%201.0-red?style=flat-square)](LICENSE)
[![Lang](https://img.shields.io/badge/Lang-ES%20%7C%20EN-lightgrey?style=flat-square)]()

</div>

---

> **⚠️ AVISO REGULATORIO**  
> Este software está en desarrollo como Dispositivo Médico Software (SaMD) bajo EU MDR 2017/745. Actualmente en **TRL 5**, sin Marcado CE. **No debe utilizarse en entornos clínicos reales** hasta obtener la certificación aplicable. Ver [Estrategia Regulatoria](https://github.com/earlify-health/wiki/Estrategia-Regulatoria).

---

## ¿Qué es Earlify Health?

Earlify Health es el primer ecosistema 360° de salud digital pediátrica que **cierra el ciclo completo** de atención temprana en niños de 2 a 6 años con alteraciones del neurodesarrollo, el lenguaje y la audición — desde la detección funcional en el hospital hasta la terapia inmersiva en el colegio.

```
🏥 Hospital          🏠 Hogar              🏫 Colegio
┌──────────┐         ┌──────────┐          ┌──────────┐
│  VIA+    │ ──────▶ │ VALERIA+ │ ───────▶ │  MAGIC   │
│          │  perfil │          │  scoring │          │
│  Cribado │ funcio- │  Rehab.  │   TPR    │  Terapia │
│ funcional│  nal    │adaptativa│          │ inmersiva│
│ (CDSS)   │         │ (padres) │          │   (AR)   │
└──────────┘         └──────────┘          └──────────┘
 MDR Clase IIa        MDR Clase I           MDR Clase I
```

---

## Los tres módulos

### 🔵 VIA+ — Clinical Decision Support System
Sistema de cribado funcional avanzado basado en análisis acústico de la voz infantil.

- Discrimina alteraciones en tres dominios: **audición · lenguaje verbal · funciones ejecutivas**
- Genera perfiles de riesgo (bajo/medio/alto) por dominio — **nunca etiquetas diagnósticas**
- Clasificador ML (Random Forest/XGBoost) con **SHAP values** para explicabilidad
- Integración nativa con HCE vía **HL7-FHIR R4**
- Clasificación MDR: **Clase IIa** · AI Act: **Sistema de alto riesgo (Anexo III)**

### 🟢 VALERIA+ — Rehabilitación Adaptativa
Módulo de intervención que genera cápsulas terapéuticas TPR personalizadas para el hogar.

- Reconocimiento de voz infantil con **OpenAI Whisper** fine-tuned (español 2-6 años)
- Cápsulas **Total Physical Response (TPR)** adaptadas al perfil de VIA+
- Involucra a los padres como agentes terapéuticos activos
- Clasificación MDR: **Clase I**

### 🟣 MAGIC — Terapia Inmersiva Escolar
Entorno de realidad aumentada que lleva la rehabilitación clínica directamente al aula.

- Tres escenarios AR: **Zoo Fonético · Aventura Narrativa · Música del Habla**
- **ARKit / ARCore + Unity** — sin hardware especializado (tablet/móvil)
- Diseñado para ser supervisado por educadores, no requiere logopeda presente
- Clasificación MDR: **Clase I**

---

## Estado actual

| Indicador | Detalle |
|-----------|---------|
| 🎯 **Madurez tecnológica** | TRL 5 — Prototipos validados en entorno clínico real |
| 👶 **Niños pilotados** | +100 en España y República Dominicana |
| 🏥 **Centros de validación** | Hospital Ribera Polusa · UFHEC Santo Domingo |
| 🏆 **Reconocimiento** | Premio Innovación en Salud · SERGAS 2023 |
| 📅 **Marcado CE VIA+ (objetivo)** | Q4 2027 – Q1 2028 |
| 💰 **Primer ingreso comercial** | 2028 (post-Marcado CE) |

---

## Stack tecnológico principal

| Área | Tecnología |
|------|-----------|
| Análisis acústico | `Parselmouth` · `openSMILE` · `librosa` |
| Machine Learning | `scikit-learn` · `XGBoost` · `SHAP` · `MLflow` |
| ASR (voz infantil) | `OpenAI Whisper` (fine-tuned) |
| Realidad Aumentada | `ARKit` · `ARCore` · `Unity` |
| Frontend | `React Native` · `Angular` · `TypeScript` |
| Backend | `Node.js` · `PostgreSQL` · `Redis` |
| Interoperabilidad | `HL7 FHIR R4` |
| Seguridad | `TLS 1.3` · `AES-256` · `OAuth 2.0 + PKCE` |

---

## Documentación (Wiki)

| Página | Descripción |
|--------|-------------|
| 📐 [Arquitectura Técnica](../../wiki/Arquitectura-Tecnica) | VIA+, VALERIA+, MAGIC — componentes, flujos y dependencias |
| ⚙️ [Stack Tecnológico](../../wiki/Stack-Tecnologico) | Dependencias completas, versiones y snippets |
| ⚖️ [Estrategia Regulatoria](../../wiki/Estrategia-Regulatoria) | MDR, AI Act, plan de certificación, PEC |
| 🤝 [Guía de Contribución](../../wiki/Guia-de-Contribucion) | Onboarding, flujo Git, estándares, política de datos |

---

## Contribuir

Las contribuciones son bienvenidas, especialmente de:

- **Investigadores** en procesamiento de voz infantil, ML clínico o neurodesarrollo
- **Desarrolladores** con experiencia en healthtech, SaMD o AR
- **Clínicos** (logopedas, pediatras, neuropediatras, ORL) para validación de features y protocolos

Antes de empezar, lee la [Guía de Contribución](../../wiki/Guia-de-Contribucion). El principio más importante:

> **Ningún output del sistema puede generar etiquetas diagnósticas.** Los outputs son siempre niveles de riesgo funcional por dominio. Cualquier violación de este principio debe reportarse inmediatamente como issue `clinical-safety`.

```bash
# Quick start
git clone https://github.com/earlify-health/earlify-health.git
cd earlify-health
cp .env.example .env.local   # solicitar valores reales al CTO
```

Ver instrucciones completas de configuración en la [Guía de Contribución](../../wiki/Guia-de-Contribucion).

---

## Partners

<table>
  <tr>
    <td align="center"><b>GooApps</b><br/><sub>Frontend / UX</sub></td>
    <td align="center"><b>GooApps</b><br/><sub>AR / VR</sub></td>
    <td align="center"><b>GooApps</b><br/><sub>Cloud / Seguridad</sub></td>
  </tr>
  <tr>
    <td align="center"><b>USC · UFHEC</b><br/><sub>Validación clínica</sub></td>
    <td align="center"><b>ACOPROS · FIAPAS</b><br/><sub>Asociaciones pacientes</sub></td>
    <td align="center"><b>Genesis Biomed</b><br/><sub>Modelado financiero</sub></td>
  </tr>
</table>

*Proyecto apoyado por FONDOCYT (República Dominicana) · Consellería de Política Social de Galicia*

---

## Licencia

Este proyecto está publicado bajo la **Earlify Health Source Available License v1.0**.

✅ Permitido: visualizar, estudiar, modificar para investigación no comercial, contribuir.  
❌ No permitido: uso comercial sin permiso escrito · despliegue clínico sin Marcado CE · redistribución como producto competidor.

Ver [LICENSE](LICENSE) y [NOTICE](NOTICE) para términos completos y atribuciones de terceros.

Para licencias comerciales o colaboraciones: **fbetances@futureforkids.eu**

---

## Contacto

**Dr. Frank Alberto Betances Reinoso**  
Founder & Chief Scientific Officer — Earlify Health  
Hospital Ribera Polusa, Lugo, España  

📧 fbetances@futureforkids.eu 
🌐 https://futureforkids.eu 
🔗 [LinkedIn](https://linkedin.com/in/frank-betances)

---

<div align="center">

*"In Pediatric Care, Early is Everything"*

**Earlify Health · Lugo, España · 2026**

</div>
