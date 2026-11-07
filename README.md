# ⚡ WinOptimizador Pro v2.0

**WinOptimizador Pro** es una utilidad de mantenimiento, auditoría y optimización para Windows moderna y ligera, desarrollada en **C# (Windows Forms)** y **PowerShell** para limpiar y exprimir al máximo el rendimiento del sistema operativo.

Diseñado con una interfaz en **Modo Oscuro**, tarjetas dinámicas con monitoreo en tiempo real y una arquitectura modular basada en configuración externa (`config/servicios.txt`).

---

## 🛠️ Características Principales

* **📦 Perfiles Separados (Windows 10 Home y Pro):** Pestañas dedicadas para auditar, desactivar o restaurar servicios innecesarios (telemetría, Xbox Live, mapas, Hyper-V, indexación, etc.) con contadores en tiempo real.
* **🟢 Monitoreo de Estado en Vivo:** Consulta directa al Registro y al controlador de servicios de Windows para mostrar si cada servicio está *Automático, Manual o Desactivado* y si se encuentra *En ejecución o Detenido*.
* **🔍 Buscador Inteligente en Tiempo Real:** Barra de filtrado instantáneo por nombre del servicio, código interno o función.
* **ℹ️ Botón de Información Contextual:** Cada tarjeta incluye un botón **Info** que despliega una ventana emergente explicando en lenguaje sencillo qué hace ese servicio y cuándo es seguro apagarlo.
* **🔄 Restauración Inteligente:** Recupera el estado original de los servicios usando respaldos locales (`respaldo_servicios.json`) o valores predeterminados de fábrica de Windows.
* **⏪ Punto de Restauración Preventivo:** Crea un punto de restauración oficial en Windows antes de aplicar cambios.
* **🧹 Limpieza Flash:** Elimina de manera silenciosa los archivos temporales de usuario (`%temp%`), la caché de Windows y vacía el DNS.
* **⚡ Máximo Rendimiento:** Desbloquea y activa el plan de energía oculto de alto rendimiento de Windows mediante comandos nativos elevados.
* **🛡️ Optimización de Windows Defender:** Limita el consumo de CPU del antivirus al 20% durante análisis en segundo plano para evitar tirones al jugar o estudiar.
* **🛠️ Caja de Herramientas Avanzada:** Accesos directos rápidos a utilidades nativas del sistema (`dxdiag`, `msinfo32`, `cleanmgr`, `mrt`, `msconfig`, `gpedit.msc`, `netplwiz`).

---

## 🚀 Requisitos y Ejecución 

1. Asegúrate de contar con Windows 10/11 (.NET Framework 4.0 o superior preinstalado).
2. Descarga el proyecto manteniendo las carpetas assets y config junto a OptimizadorPro.exe.
3. Ejecuta OptimizadorPro.exe como Administrador (indispensable para aplicar los cambios en los servicios y el Registro del sistema).

---

## 👤 Autor y Licencia

* **Autor:** Lester R (Lester Rosado) — Desarrollo de software y diseño de interfaz.

* **Licencia:** Uso gratuito personal (Freeware). Todos los derechos reservados. Queda prohibida su redistribución modificada o copia sin autorización del autor.

---


## 📂 Estructura de Carpetas

Para su correcto funcionamiento, mantén la siguiente estructura junto al ejecutable:

```text
Optimizador/
├── OptimizadorPro.exe
├── assets/
│   └── icono.ico
└── config/
    └── servicios.txt
