# Mars Photos App

Aplicación móvil desarrollada en Android con Jetpack Compose y Kotlin. Implementa la arquitectura recomendada por Google separando la capa de interfaz de usuario de la capa de datos mediante el patrón Repositorio y un contenedor de Inyección de Dependencias (DI) manual.

## Características

- **Jetpack Compose**: Interfaz de usuario declarativa y moderna.
- **Patrón Repositorio**: Abstracción del acceso a datos remotos mediante la interfaz `MarsPhotosRepository` y su implementación `NetworkMarsPhotosRepository`.
- **Inyección de Dependencias Manual**: Gestión centralizada del ciclo de vida y configuración del servicio de red mediante `AppContainer` y `DefaultAppContainer`.
- **ViewModel & StateFlow**: Manejo de estados de la interfaz (`Loading`, `Success`, `Error`) desacoplado de la vista con `MarsViewModel` y `ViewModelProvider.Factory`.
- **Retrofit & Kotlinx Serialization**: Consumo asíncrono de servicios REST de fotos de Marte con corrutinas de Kotlin.

## Requisitos

- Android Studio Iguana o superior
- JDK 17
- Dispositivo físico o emulador con Android 7.0 (API 24) o superior
