# Fotos Vallarta Sock

Imágenes de stock para contenidos automatizados en WordPress u otros CMS.

## Contenido

- 261 imágenes en formato WebP.
- Resolución horizontal de 1350 × 1080 px.
- Peso máximo de 512 KB por archivo.
- Sin marcas de agua.

## Estructura

Los archivos usan un prefijo numérico (`01_`, `02_`, … `13_`) que identifica el lote original. El resto del nombre conserva una referencia del lugar o tema de la foto.

```
final/
  01_LL-01.webp
  01_LL-02.webp
  ...
  13_LL-25.webp
```

## Uso

Este repositorio funciona como fuente de imágenes para flujos de publicación automatizada:

1. Listar los archivos disponibles mediante la API de GitHub o clonando el repositorio.
2. Elegir una imagen y descargarla desde `raw.githubusercontent.com`.
3. Subirla al CMS como media y asociarla al contenido.

Para evitar repeticiones, registra en tu CMS o en un archivo de estado qué imágenes ya fueron utilizadas.

## Repositorio público

Los archivos son accesibles sin autenticación. GitHub limita a 5,000 solicitudes por hora por token autenticado, suficiente para volúmenes de publicación bajos o moderados.

## Notas

- Las imágenes se distribuyen ya optimizadas; evita recomprimirlas para no perder calidad.
- GitHub no está pensado como CDN de producción. Si el tráfico o el volumen crece, migra los archivos a un almacenamiento con CDN (por ejemplo, Cloudflare R2 o S3).
- Verifica los derechos de uso de cada imagen antes de publicarla en sitios de terceros.
