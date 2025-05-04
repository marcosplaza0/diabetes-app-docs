## 📄 Requisitos del Proyecto – App de Diabetes

Este documento define los requisitos funcionales y no funcionales de la *App de Gestión de la Diabetes*, desarrollada como proyecto final del ciclo de Desarrollo de Aplicaciones Multiplataforma.

---

## ✅ 1. Requisitos Funcionales

Estas son las funcionalidades principales que la app debe proporcionar para cumplir su propósito.

- **RF1**: El usuario puede registrar lecturas de glucosa en sangre, incluyendo fecha, hora y valor.
- **RF2**: El usuario puede registrar dosis de insulina con cantidad y hora.
- **RF3**: El usuario puede añadir notas a cada entrada (por ejemplo, comidas, actividad física, síntomas).
- **RF4**: La app muestra las lecturas anteriores en una lista con filtros (por ejemplo, por día, semana o rango).
- **RF5**: La app muestra gráficos de las tendencias de glucosa a lo largo del tiempo.
- **RF6**: El usuario puede configurar recordatorios para:
    - Inyecciones de insulina
    - Mediciones de glucosa
    - Citas médicas
- **RF7**: Todos los datos del usuario se almacenan localmente y se conservan incluso después de cerrar la app.
- **RF8**: El usuario puede editar o eliminar las entradas registradas.

---

## 📋 2. Requisitos No Funcionales

Estos definen cómo debe comportarse y funcionar la aplicación.

- **RNF1**: La app debe funcionar **sin conexión** (offline), sin necesidad de acceso a internet.
- **RNF2**: La app debe conservar todos los datos del usuario después de cerrarse o reiniciarse.
- **RNF3**: La app debe ser compatible con las plataformas **Android e iOS**.
- **RNF4**: La app debe estar desarrollada con **Flutter** y **Dart**.
- **RNF5**: La interfaz debe seguir las directrices de diseño de **Material Design**.
- **RNF6**: El idioma principal de la app debe ser **español**, con soporte opcional en inglés.
- **RNF7**: La app debe seguir buenas prácticas de accesibilidad (por ejemplo, tipografías legibles, contraste adecuado...).

---

## 📎 3. Restricciones

- **Restricción Tecnológica**: La aplicación debe desarrollarse utilizando el framework Flutter.
- **Restricción de Tiempo**: La primera versión del proyecto debe completarse y entregarse antes de la fecha límite académica.
- **Restricción de Plataforma**: Solo se admiten plataformas móviles (Android/iOS) en esta versión.

---

## 🚀 4. Consideraciones Futuras

Características que podrían añadirse después del lanzamiento de la versión MVP:

- **Exportación a PDF/CSV**: para compartir registros de glucosa con médicos o almacenarlos.
- **Respaldo y sincronización en la nube**: utilizando Firebase u otro servicio similar.
- **Modo oscuro**: interfaz opcional con tema oscuro o claro.