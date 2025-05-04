# 🧱 Arquitectura de la Aplicación – App de Diabetes

Este documento describe la arquitectura técnica de la App de Gestión de la Diabetes, incluyendo las partes principales, herramientas y decisiones de diseño utilizadas en el desarrollo.

---

## ⚙️ Tecnologías Utilizadas

- **Flutter** – Framework de interfaz para desarrollo multiplataforma
- **Dart** – Lenguaje principal de programación
- **Almacenamiento Local** – (Por definir: Hive, SQLite...)
- **Gráficas** – Paquete `fl_chart` o similar para visualización de datos
- **Notificaciones** – `flutter_local_notifications` para recordatorios

---

## 🧭 Vista General de la Arquitectura

La aplicación sigue una **arquitectura por capas**, con separación de responsabilidades:

```plaintext
Capa de Presentación (UI)
│
├── Gestión de Estado (ej. Provider)
├── Capa de Datos
│   ├── Almacenamiento Local (ej. Hive)
│   └── Modelos (GlucoseEntry, Reminder, etc.)
```

---

## 📱 Pantallas y Navegación

*Nota: Las pantallas y las vistas son cosas diferentes.*

- **HomeScreen** – Resumen diario y acceso rápido al registro
- **LogEntryScreen** – Formulario para añadir glucosa o insulina
- **HistoryScreen** – Diferentes formas de visualizar tendencias y resúmenes de glucosa
- **ChartScreen** – Vista gráfica de las tendencias de glucosa
- **ReminderScreen** – Gestión de recordatorios
- **SettingsScreen** – Idioma, tema, copia de seguridad (futuro)

La navegación usará **`Navigator 2.0`** o un paquete como `go_router` para un enrutamiento escalable.

---

## 🧩 Componentes Principales

*Nota: Los siguientes componentes son conceptuales y pueden evolucionar a medida que se desarrolla la app.*

### 1. Modelos
- `GlucoseEntry`: almacena valor, fecha/hora y notas
- `InsulinDose`: tipo, unidades, timestamp
- `Reminder`: tipo, hora, repetición

### 2. Servicios
- `StorageService`: gestiona lectura/escritura en la base de datos
- `NotificationService`: configura y cancela recordatorios locales

### 3. Providers / Controladores
- Responsable de mantener el seguimiento de los datos de la aplicación en tiempo real y asegurarse de que la interfaz de usuario se actualice correctamente cuando esos datos cambien.

---

## 🧪 Estrategia de Pruebas

- Pruebas unitarias para la lógica de los modelos
- Pruebas de widgets para componentes de la interfaz
- Pruebas manuales en dispositivos Android/iOS

---

## 🔜 Consideraciones Futuras

- Añadir `CloudService` (ej. Firebase) para sincronización
- Usar almacenamiento cifrado para proteger datos sensibles