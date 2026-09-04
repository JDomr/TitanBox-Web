# TBOX.ONE

Sitio oficial estático de Titan Box. Esta fase es local: no hay hosting, DNS, API, analítica, cookies, formularios ni dependencias de terceros.

## Vista previa local

Desde esta carpeta:

```sh
python3 -m http.server 4173
```

Abrir `http://localhost:4173/`. El servidor solo sirve archivos locales y no publica el sitio.

## Arquitectura

- HTML estático bilingüe: español en `/` y páginas inglesas estables bajo `/en/`.
- CSS local en `assets/css/site.css`; sin CDN, fuentes remotas ni JavaScript de terceros.
- Logo y tipografías proceden de los recursos locales oficiales de Titan Box y se copian a `assets/` para mantener este proyecto independiente.
- `robots.txt` y `sitemap.xml` están preparados para el dominio previsto `tbox.one`.

## Antes de publicar

Pendiente de revisión legal y operativa antes de desplegar:

1. Confirmar contenido final de Política de Privacidad, Términos y datos de contacto con asesoría legal.
2. Sustituir el estado pendiente del enlace a Google Play por la URL oficial publicada.
3. Sustituir los espacios de capturas por capturas oficiales aprobadas; no publicar placeholders como capturas reales.
4. Configurar hosting, HTTPS, DNS, cabeceras de seguridad y cualquier requisito de cookies/consentimiento que aplique al proveedor elegido.
5. Revisar metadatos, imagen Open Graph y accesibilidad tras incorporar activos finales.

## Despliegue futuro

El resultado se puede alojar como archivos estáticos en un hosting HTTPS. No requiere backend. Cualquier integración de formularios, analítica, fuentes remotas o terceros debe revisarse antes de añadirse porque cambia la declaración de privacidad.

## Git

Este repositorio es independiente de `TitanBox`. No configura remoto en esta fase.
