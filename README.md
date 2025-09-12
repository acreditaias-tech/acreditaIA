# AcreditaIA — Evidencias de IA verificables (AIBOM + VC + ai.txt)

Cumplimiento verificable de IA (AI Act &amp; NIS2). Generamos automáticamente AIBOM, Model Cards y credenciales verificables (VC 2.0) con archivo público ai.txt para demostrar transparencia y confianza en sistemas de inteligencia artificial.

Verifiable AI compliance (AI Act & NIS2). Automatically generates AIBOM, Model Cards and Verifiable Credentials (VC 2.0) with a public ai.txt file to provide transparency and trust in AI systems.




**Transparencia y verificación para sistemas de IA.**  
Este repositorio muestra cómo publicamos y verificamos evidencias de IA: `/.well-known/ai.txt`, `aibom.json`, `ai-credential.json` (VC con hash del AIBOM), `MODEL_CARD.md`, `risk_register.csv` y `ai-policy.html`.

---

## 🚀 Quick demo
- `ai.txt` → https://acreditaias-tech.github.io/acreditaIA/.well-known/ai.txt  
- `AIBOM` → https://acreditaias-tech.github.io/acreditaIA/aibom.json  
- `Credencial (VC)` → https://acreditaias-tech.github.io/acreditaIA/ai-credential.json  
- `Política IA` → https://acreditaias-tech.github.io/acreditaIA/ai-policy.html  
- `Model Card` → https://acreditaias-tech.github.io/acreditaIA/MODEL_CARD.md  
- `Risk Register` → https://acreditaias-tech.github.io/acreditaIA/risk_register.csv

> **Nota:** Estos artefactos son **demo**. Para cada cliente, publicamos en su propio dominio/Pages (p.ej., `https://cliente.github.io/evidencias`).

---

## ✅ ¿Qué entregamos?
1. `/.well-known/ai.txt`: tarjeta pública con enlaces y contacto.  
2. `aibom.json`: inventario técnico (AI Bill of Materials).  
3. `ai-credential.json`: credencial verificable con **SHA-256** del AIBOM.  
4. `MODEL_CARD.md`: uso, datos, riesgos, métricas por sistema.  
5. `risk_register.csv`: riesgos/controles con evidencia.  
6. `ai-policy.html`: política pública de IA.

🛠️ Cómo generamos estas evidencias para un cliente (resumen)

Ejecutamos el motor privado (AcreditaIA Engine) con su repo (solo lectura) → genera aibom.json, ai-credential.json, /.well-known/ai.txt, MODEL_CARD.md, risk_register.csv, ai-policy.html.

Revisamos/Enriquecemos (riesgos, controles, métricas).

Publicamos en el dominio del cliente (GitHub Pages u otro hosting).

Validamos: URLs 200 OK + hash coincide + fechas/contacto correctos.

---

## 🔒 Verificar integridad del AIBOM (Windows)
Comprueba que el `bomHash` de la VC coincide con el hash real de `aibom.json`:

```cmd
certutil -hashfile aibom.json SHA256


## Licencia
© 2025 AcreditaIA. Todos los derechos reservados.  
Uso permitido solo para evaluación. Prohibido uso comercial o redistribución sin autorización escrita.  
Contacto: [acreditaias@gmail.com](mailto:acreditaias@gmail.com)
