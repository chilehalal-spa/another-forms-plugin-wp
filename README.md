# Another Forms Plugin (Pro)

Sistema de formularios modular.

Se usa en: chilehalal.cl, chisi.cl.

## Instalación

1. Descarga `another-forms-plugin.zip` desde la
   [última release](https://github.com/chilehalal-spa/another-forms-plugin-wp/releases/latest).
   No uses el botón "Code → Download ZIP": ese zip trae otro nombre de carpeta.
2. En WordPress: *Plugins → Añadir nuevo → Subir plugin*, elige el zip y activa.

## Uso

Shortcodes: `[another_form]`.

## Actualizaciones

El plugin se actualiza desde las releases de este repositorio, como cualquier
plugin de wordpress.org: aparecen en *Escritorio → Actualizaciones* y se pueden
dejar automáticas en *Plugins → Activar actualizaciones automáticas*.

WordPress revisa cada 12 horas; la respuesta de GitHub se guarda 6 horas.

## Publicar una versión nueva

1. Sube `Version:` en `another-forms-plugin.php` (por ejemplo `1.9.0`).
2. Haz commit y push.
3. Crea y sube el tag con el mismo número:

   ```bash
   git tag v1.9.0
   git push origin v1.9.0
   ```

La Action [Release](.github/workflows/release.yml) verifica que el tag coincida
con la versión, arma `another-forms-plugin.zip` y publica la release. Desde ese
momento los sitios ven la actualización.

## Licencia

GPL-2.0-or-later. Ver [LICENSE](LICENSE).
