# CI/CD: Ejemplo Práctico con GitHub Actions

Este proyecto explica de forma detallada el ciclo **CI/CD** usando GitHub Actions, incluyendo pruebas unitarias y la construcción automática de un **package**.  
El objetivo es que cualquier persona pueda reproducir el flujo desde cero.

---

## 📌 ¿Qué es CI/CD?

**CI (Integración Continua)** es la práctica donde cada cambio que se sube al repositorio se integra automáticamente, ejecutando pruebas para evitar errores.

**CD (Entrega Continua / Despliegue Continuo)** es cuando el sistema genera artefactos listos para entregar o incluso los despliega automáticamente en producción.

---

## 🔁 Ciclo completo CI/CD usado en este proyecto

1. **Desarrollador hace push al repositorio**  
2. GitHub Actions detecta el cambio y ejecuta el workflow:
   - 🧪 Instala dependencias  
   - 🧪 Ejecuta pruebas unitarias  
   - 🧪 Verifica calidad del código  
   - 📦 Construye un package (.zip)  
   - 📤 Guarda el artefacto en el pipeline  
3. El artefacto queda listo para descarga o despliegue.

---

## 🧪 Ejemplo práctico de pruebas

Este proyecto usa Node.js y contiene una prueba simple ubicada en:

