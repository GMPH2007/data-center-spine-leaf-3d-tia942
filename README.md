# 🏛️ Data Center 3D/4D: Red Spine-Leaf 100G & Canalizaciones ANSI/TIA-942

[![ANSI/TIA-942 Rated 1-4](https://img.shields.io/badge/Standard-ANSI%2FTIA--942-00f0ff?style=for-the-badge&logo=shield)](https://github.com/GMPH2007/data-center-spine-leaf-3d-tia942)
[![Three.js WebGL](https://img.shields.io/badge/WebGL-Three.js%203D%2F4D-f59e0b?style=for-the-badge&logo=three.js)](https://github.com/GMPH2007/data-center-spine-leaf-3d-tia942)
[![Network](https://img.shields.io/badge/Topology-Spine--Leaf%20100G-10b981?style=for-the-badge)](https://github.com/GMPH2007/data-center-spine-leaf-3d-tia942)
[![Live Demo](https://img.shields.io/badge/Demo%20Online-GitHub%20Pages-a855f7?style=for-the-badge&logo=github)](https://GMPH2007.github.io/data-center-spine-leaf-3d-tia942/)

---

## 📌 Datos Académicos y Proyecto

* **Institución:** Instituto de Educación Superior Tecnológico Público **"Hermanos Cárcamo"** – Paita, Piura, Perú
* **Programa Académico:** Arquitectura de Plataformas y Servicios de Tecnologías de la Información
* **Módulo Formativo:** Diseño de Arquitectura de Data Center (Módulo 3) – **Sesión 05**
* **Estudiante:** **Gerson Misael Pintado Huaman**
* **Docente Responsable:** **Ing. Javier Eduardo Jaramillo Atoche**
* **Caso Práctico:** Sistema de Transporte de Información, Red Spine-Leaf 100G, Canalizaciones Panduit FiberRunner y Gestión Térmica en Sala Blanca para ***Mar del Norte Logistics S.A.C.*** (Zona Portuaria de Paita)

---

## 🌐 Enlace a la Simulación Interactiva en Vivo

> **Prueba el simulador 3D/4D directamente en tu navegador sin instalar nada:**  
> 👉 **[https://GMPH2007.github.io/data-center-spine-leaf-3d-tia942/](https://GMPH2007.github.io/data-center-spine-leaf-3d-tia942/)**

---

## 🚀 Características Principales del Proyecto

### 1. Cuatro Arquitecturas Físicas Diferenciadas (ANSI/TIA-942)
* **🔴 Categoría 1 (Tier I: Básico - Capacidad Simple $N$):** Sala básica de 4 gabinetes en una sola fila, 1 solo switch Spine, 1 solo CRAC y 1 canalización aérea simple. Sin redundancia: cualquier corte de luz o cable apaga todo el Data Center.
* **🟠 Categoría 2 (Tier II: Componentes Redundantes $N+1$):** 6 gabinetes en 2 filas escalonadas, 2 switches Spine y 2 unidades CRAC ($N+1$). Una sola canalización aérea amarilla compartida con puente central.
* **🔵 Categoría 3 (Tier III: Mantenimiento Concurrente):** 8 gabinetes en 2 filas enfrentadas con **Pasillo Frío Confinado (Cold Aisle Containment)** con techo y puertas de cristal. **Dos canalizaciones físicas independientes (Ruta A Amarilla y Ruta B Azul Cian) separadas por más de 4 metros**.
* **💎 Categoría 4 (Tier IV: Tolerante a Fallos $2(N+1)$):** **Dos salas blancas físicamente aisladas** divididas por un **Muro Cortafuegos RF-120** central con ventanal de inspección técnica. Sistemas gemelos activos-activos con doble canalización (Cian y Púrpura).

### 2. Inyector Interactivo de Fallas Críticas
* **🔌 ¿Qué pasa si se va la Luz? (Blackout Mode):** La sala entra en penumbra y se encienden luces estroboscópicas rojas de emergencia. Demuestra apagón total en Tier I, transferencia a UPS y arranque de generador en Tier II, y continuidad sin pestañeo en Tier III/IV.
* **❄️ ¿Qué pasa si falla el Aire Frío? (CRAC Failure):** El aire frío se detiene y la temperatura sube a 41.5 °C en Tier I (alerta térmica ASHRAE) frente al arranque inmediato del CRAC de reserva en Tier II, III y IV.
* **✂️ ¿Qué pasa si se corta la Fibra?:** Demuestra corte de servicio en Tier I/II vs conmutación en menos de 10 ms a la **Ruta B (Canalización Secundaria)** en Tier III y IV.

### 3. Modos Avanzados de Inspección
* **🌡️ Termografía Infrarroja FLIR:** Vista térmica en falso color (azul 18°C a rojo 38°C) para validar el cumplimiento del estándar **ASHRAE TC 9.9**.
* **🔬 Modo Rayos X:** Racks transparentes en malla cian para inspeccionar el conexionado Top of Rack (ToR) y patch cords internos.
* **🚁 Dron Cinematográfico (Auto-Órbita):** Vuelo continuo de 360° para exposiciones y presentaciones en proyector.
* **▶️ Exposición Guiada en 5 Fases:** Asistente interactivo paso a paso con botón de **Auto-Tour**.

---

## 📁 Contenido del Repositorio

| Archivo / Carpeta | Descripción |
| :--- | :--- |
| **[`index.html`](index.html)** | Simulador web interactivo 3D/4D principal (ejecutable en navegador o GitHub Pages). |
| **[`Simulacion_3D_DataCenter_Pintado.ipynb`](Simulacion_3D_DataCenter_Pintado.ipynb)** | Cuaderno interactivo de Google Colab con visualización Three.js en celda de salida. |
| **[`Caso_Practico_y_Mapa_Conceptual_Data_Center_Misael_Pintado.pdf`](Caso_Practico_y_Mapa_Conceptual_Data_Center_Misael_Pintado.pdf)** | Informe técnico completo en PDF listo para entrega académica (Caso Práctico + Mapa Conceptual). |
| **[`Caso_Practico_y_Mapa_Conceptual_Data_Center_Misael_Pintado.docx`](Caso_Practico_y_Mapa_Conceptual_Data_Center_Misael_Pintado.docx)** | Informe técnico editable en formato Microsoft Word. |
| **[`Presentacion_Data_Center_Misael_Pintado.pdf`](Presentacion_Data_Center_Misael_Pintado.pdf)** | Diapositivas de exposición ejecutiva en PDF. |
| **[`Presentacion_Data_Center_Misael_Pintado.pptx`](Presentacion_Data_Center_Misael_Pintado.pptx)** | Diapositivas de exposición editables en formato Microsoft PowerPoint (16 slides estilo Canva). |
| **`assets/`** | Librerías Three.js offline, controles orbitales, diagramas de red y mapa conceptual HD. |
| **`Demostracion_*.png`** | Capturas de pantalla en alta resolución de las 4 categorías, modos FLIR, Rayos X y fallas. |

---

## 🛠️ Instrucciones de Ejecución

### Opción A: Ver en Línea (Recomendado)
Abre directamente el enlace de GitHub Pages:  
👉 **[https://GMPH2007.github.io/data-center-spine-leaf-3d-tia942/](https://GMPH2007.github.io/data-center-spine-leaf-3d-tia942/)**

### Opción B: Ejecución Local
1. Clona el repositorio o descarga el archivo ZIP:
   ```bash
   git clone https://github.com/GMPH2007/data-center-spine-leaf-3d-tia942.git
   ```
2. Abre el archivo `index.html` haciendo doble clic en él con cualquier navegador (Chrome, Edge, Firefox, Brave). No requiere servidores locales.

### Opción C: Ejecución en Google Colab
1. Sube el archivo `Simulacion_3D_DataCenter_Pintado.ipynb` a [Google Colab](https://colab.research.google.com/).
2. Ejecuta la celda de Python para renderizar la simulación 3D dentro del notebook.

---

## 📜 Normativas y Estándares Aplicados
* **ANSI/TIA-942-B:** Telecommunications Infrastructure Standard for Data Centers.
* **ANSI/TIA-568.3-D:** Optical Fiber Cabling Components Standard (OM4 MPO-12).
* **ANSI/TIA-568.2-D:** Balanced Twisted-Pair Telecommunications Cabling and Components (Cat 6A).
* **ANSI/TIA-569-E:** Telecommunications Pathways and Spaces (Canalizaciones Panduit FiberRunner).
* **ANSI/TIA-606-C:** Administration Standard for Telecommunications Infrastructure.
* **ASHRAE TC 9.9:** Thermal Guidelines for Data Processing Environments (Clase A1/A2).

---
*IESTP Hermanos Cárcamo – Paita • 2026*
