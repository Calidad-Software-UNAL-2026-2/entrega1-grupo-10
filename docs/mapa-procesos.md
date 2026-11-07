# Mapa de Procesos y Modelo de Ciclo de Vida

> Generado con el workflow de flujo único. La definición formal del
> modelo de ciclo de vida (justificación, orden, relación entre
> procesos) se documenta en la wiki, página `04c-Modelo-Ciclo-Vida`,
> no en este archivo.

## Proceso: 6.4.2 Definición de necesidades y requisitos de los interesados

- **Entradas:** Enunciado de VetReminder, extensión del modelo verbal (01-Extension-Modelo-Verbal)
- **Actividades:** Identificar a los actores, definir las necesidades del negocio y las de cada interesado
- **Salidas:** Actores (02b-Actores), necesidades del negocio (02c-Necesidades-Negocio) y de los interesados (02d-Necesidades-Interesados)
- **Recursos:** Wiki de GitHub, BABOK v3, docente o monitor para aclarar dudas

## Proceso: 6.4.3 Definición de requisitos del sistema/software

- **Entradas:** Necesidades del negocio y de los interesados, requisitos de interfaz (02e-Requisitos-Interfaz)
- **Actividades:** Redactar los requisitos funcionales como historias de usuario con criterios de aceptación, los no funcionales con métrica y umbral, asociarlos a su módulo y establecer la línea base
- **Salidas:** Módulos y requisitos como Issues, vista «Registro de Requisitos» del Project
- **Recursos:** Formularios de Issues (módulo, RF y RNF), GitHub Projects

## Proceso: 6.4.4 Definición de la arquitectura

- **Entradas:** Requisitos del incremento, requisitos de interfaz, restricciones tecnológicas (React Native y Firebase)
- **Actividades:** Definir los componentes (app móvil, portal veterinario, servicios de Firebase, conectores con las clínicas), sus interfaces y cómo se cumplen los RNF de disponibilidad, rendimiento y seguridad
- **Salidas:** Documento y diagrama de arquitectura
- **Recursos:** Herramienta de diagramas (draw.io), documentación de Firebase y React Native

## Proceso: 6.4.5 Definición del diseño

- **Entradas:** Arquitectura, requisitos del incremento
- **Actividades:** Diseñar el modelo de datos en Firestore, las pantallas y la navegación, y aplicar las pautas de accesibilidad
- **Salidas:** Modelo de datos, prototipos de pantallas, especificación de diseño por módulo
- **Recursos:** Herramienta de prototipado (Figma u otra), pautas WCAG 2.1

## Proceso: 6.4.7 Implementación

- **Entradas:** Especificación de diseño, requisitos del incremento
- **Actividades:** Programar los módulos, escribir las pruebas unitarias y revisar el código en pull requests
- **Salidas:** Código fuente versionado, pruebas unitarias
- **Recursos:** React Native, Firebase SDK, GitHub, entorno de desarrollo

## Proceso: 6.4.8 Integración

- **Entradas:** Módulos implementados, servicios externos configurados
- **Actividades:** Integrar los módulos nuevos con los existentes y con los servicios externos y ejecutar pruebas de integración
- **Salidas:** Versión integrada del incremento, reporte de pruebas de integración
- **Recursos:** GitHub Actions, entorno de pruebas de Firebase, cuentas de prueba de FCM y APNs

## Proceso: 6.4.9 Verificación

- **Entradas:** Versión integrada, requisitos con sus criterios de aceptación y métricas
- **Actividades:** Ejecutar las pruebas funcionales con los criterios Dado/Cuando/Entonces, las pruebas de rendimiento y de seguridad y registrar los defectos
- **Salidas:** Reporte de verificación, defectos registrados como Issues
- **Recursos:** Jest y herramientas de pruebas de React Native, Firebase Test Lab, dispositivos Android e iOS

## Proceso: 6.4.10 Transición

- **Entradas:** Versión verificada, notas de la versión
- **Actividades:** Preparar los binarios, publicarlos en Google Play y App Store, desplegar el portal veterinario y capacitar a los veterinarios de las clínicas piloto
- **Salidas:** Versión publicada en las tiendas, portal en producción
- **Recursos:** Cuentas de desarrollador de Google y Apple (INT-09), Firebase Hosting

## Proceso: 6.4.11 Validación

- **Entradas:** Versión publicada, necesidades del negocio y de los interesados
- **Actividades:** Hacer pruebas de aceptación con dueños y veterinarios, aplicar el cuestionario SUS y recoger retroalimentación para el siguiente incremento
- **Salidas:** Acta de aceptación del incremento, puntaje SUS, ajustes para el siguiente incremento
- **Recursos:** Grupo piloto de usuarios, cuestionario SUS, formulario de retroalimentación

