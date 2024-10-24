# Mejores Prácticas de Seguridad para Aplicaciones Android

## 1. Firma de Aplicaciones
- No firmar la aplicación con certificados de depuración. Utilice certificados firmados para producción para evitar manipulaciones y garantizar la seguridad.

## 2. Configuración de `AndroidManifest.xml`
- **Deshabilitar el modo de depuración**: Evite que el atributo `android:debuggable` esté habilitado en la versión de producción.
- **Asegurar componentes exportados**: Verifique que los servicios, receptores y proveedores de contenido exportados estén protegidos con permisos adecuados y no sean accesibles por aplicaciones no autorizadas.

## 3. Manejo de Permisos
- Solicite permisos de ubicación solo cuando sea necesario y asegúrese de que la aplicación explique claramente por qué necesita estos permisos.
- Mantenga el uso de permisos al mínimo para reducir el riesgo.

## 4. Compatibilidad de Versiones
- Evite el soporte para versiones de Android que ya no reciban actualizaciones de seguridad (recomendado: API 29 o superior).
