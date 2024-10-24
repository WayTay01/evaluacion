# Programa de Mejoras de Seguridad para AplicacionMapa_AY

## Objetivo
Reducir el riesgo de seguridad de la aplicación y mejorar la calificación de seguridad general, abordando los problemas encontrados en el análisis.

## Plan de Acción
### 1. Correcciones Inmediatas (Dentro de 1 Mes)
- **Deshabilitar depuración**: Cambiar `android:debuggable` a `false` en `AndroidManifest.xml`.
- **Actualizar firma**: Reemplace el certificado de depuración por uno de producción.

### 2. Mediano Plazo (Dentro de 3 Meses)
- **Revisar permisos exportados**: Verifique los permisos utilizados por los componentes exportados y realice ajustes para asegurar que no sean accesibles por aplicaciones no autorizadas.
- **Actualizar compatibilidad de versiones**: Modifique el `minSdk` para eliminar soporte a versiones obsoletas y no seguras de Android.

### 3. Largo Plazo (Dentro de 6 Meses)
- **Revisión de permisos**: Evalúe todos los permisos solicitados por la aplicación y reduzca al mínimo los necesarios para evitar posibles abusos.
- **Pruebas periódicas de seguridad**: Implemente un proceso regular de auditorías de seguridad para garantizar que la aplicación se mantenga segura con el tiempo.
