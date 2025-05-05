# 🧪 Plan de Pruebas – App de Diabetes

Este documento describe la estrategia de pruebas para la App de Gestión de la Diabetes. El objetivo es garantizar que la aplicación funcione correctamente, cumpla con los requisitos y ofrezca una experiencia de usuario estable.

---

## ✅ Objetivos de las Pruebas

- Verificar que las funcionalidades principales funcionen como se espera
- Asegurar que los datos se almacenen y recuperen correctamente
- Confirmar que la interfaz de usuario responda adecuadamente a las acciones del usuario
- Detectar errores de forma temprana y prevenir regresiones
- Validar el comportamiento de la app en diferentes dispositivos y plataformas

---

## 🔍 Tipos de Pruebas

### 1. Pruebas Manuales

Realizadas regularmente durante el desarrollo en dispositivos reales y emuladores.

#### Ejemplos:
- Añadir una lectura de glucosa → la entrada aparece en el historial
- Configurar un recordatorio → la notificación se activa a la hora correcta
- Eliminar una entrada → la entrada desaparece de la lista
- Reiniciar la app → los datos siguen disponibles
- Cambiar el idioma en ajustes → la interfaz se actualiza correctamente

---

### 2. Pruebas Unitarias

Enfocadas en probar la lógica de clases y funciones individuales, como:

- Creación y validación del modelo `GlucoseEntry`
- Lógica de programación de recordatorios
- Cálculos de datos (por ejemplo, promedios, tendencias)

Herramienta: `flutter_test`

---

### 3. Pruebas de Widgets

Simulan la interacción del usuario con los componentes de la interfaz.

Ejemplos:
- Rellenar y enviar un formulario
- Pulsar botones (ej. Guardar, Eliminar)
- Navegar entre pantallas

Herramienta: `flutter_test`

---

### 4. Pruebas en Dispositivos y Plataformas

Pruebas realizadas en Android e iOS para garantizar compatibilidad y coherencia.

#### Dispositivos:
- emulador de Android (Google Pixel 8, API 30+)
- emulador de iOS (iPhone 13)
- Dispositivo físico: Xiaomi Redmi Note 12 Pro Plus 5G

---

## 🧩 Herramientas de Prueba

- `flutter_test`: framework de pruebas integrado de Flutter
- `integration_test`: para pruebas completas de la app (opcional en el futuro)

---

## 📆 Calendario de Pruebas

| Fase                  | Tipo                         | Estado       |
|-----------------------|------------------------------|--------------|
| Durante el desarrollo | Pruebas manuales y unitarias | Por realizar |
| Antes del MVP         | Pruebas completas de widgets | Por realizar |
| Entrega final         | Pruebas manuales + resumen   | Por realizar |

---

## 📝 Notas

- Todos los resultados de las pruebas serán revisados y documentados antes de la entrega.
- Los errores y problemas visuales se registrarán en GitHub (issues o tablero del proyecto).
