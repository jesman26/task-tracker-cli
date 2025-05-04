# Task Tracker CLI

Task Tracker CLI es una aplicación de línea de comandos para rastrear y administrar tus tareas. Puedes agregar, actualizar, eliminar y listar tareas, así como marcarlas como en curso o finalizadas.

## URL del Proyecto
[https://github.com/jesman26/task-tracker-cli/](https://github.com/jesman26/task-tracker-cli/)

## Requisitos Previos
- Node.js (v14 o superior)
- npm (v6 o superior)

## Instalación
1. Clona este repositorio:
   ```bash
   git clone https://github.com/jesman26/task-tracker-cli.git
   ```
2. Navega al directorio del proyecto:
   ```bash
   cd task-tracker-cli
   ```
3. Instala las dependencias:
   ```bash
   npm install
   ```

## Uso
### Comandos disponibles:
- **Agregar una tarea**:
  ```bash
  node src/index.js add "Descripción de la tarea"
  ```
- **Actualizar una tarea**:
  ```bash
  node src/index.js update <id> "Nueva descripción"
  ```
- **Eliminar una tarea**:
  ```bash
  node src/index.js delete <id>
  ```
- **Marcar una tarea como en curso**:
  ```bash
  node src/index.js mark-in-progress <id>
  ```
- **Marcar una tarea como finalizada**:
  ```bash
  node src/index.js mark-done <id>
  ```
- **Listar todas las tareas**:
  ```bash
  node src/index.js list
  ```
- **Listar tareas por estado**:
  - Tareas completadas:
    ```bash
    node src/index.js list done
    ```
  - Tareas pendientes:
    ```bash
    node src/index.js list todo
    ```
  - Tareas en curso:
    ```bash
    node src/index.js list in-progress
    ```

## Estructura del Proyecto
```plaintext
task-tracker-cli
├── src
│   ├── index.js          # Archivo principal de la CLI
│   ├── commands          # Comandos individuales
│   ├── utils             # Utilidades como manejo de archivos
│   └── types             # Tipos y definiciones
├── tasks.json            # Archivo JSON donde se almacenan las tareas
├── package.json          # Configuración del proyecto
└── README.md             # Este archivo
```

## Contribuciones
¡Las contribuciones son bienvenidas! Por favor, abre un issue o envía un pull request.

## Licencia
Este proyecto está bajo la licencia MIT.