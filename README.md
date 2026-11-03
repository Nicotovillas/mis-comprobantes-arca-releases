# Comprobantes — distribución

Este repositorio contiene únicamente instaladores, firmas y el manifiesto de actualizaciones de Comprobantes. El repositorio de desarrollo es privado. No se alojan claves, configuración, reportes ni historial de usuarios.

## Mac Apple Silicon

Descargá el ZIP de la última versión en [Releases](https://github.com/Nicotovillas/mis-comprobantes-arca-releases/releases/latest), descomprimilo y copiá Comprobantes.app a la carpeta Applications de tu usuario (`~/Applications`). Cerrá la copia anterior antes de reemplazarla. La app incluye el motor Python y el navegador necesario; no requiere instalar Rust o Python.

La distribución actual usa firma ad-hoc de macOS, sin notarización de Apple. Gatekeeper puede pedir autorización manual. La firma del actualizador es independiente y se verifica antes de instalar cada paquete.

La primera copia que permite actualizarse es 0.2.12: versiones anteriores necesitan un reemplazo manual. Las versiones nuevas se anuncian con un cartel al abrir; se pueden posponer y la instalación requiere pulsar Actualizar y reiniciar. Sólo se publica el destino macOS Apple Silicon (darwin-aarch64) por ahora.

## Archivos de cada Release

- ZIP: instalación manual.
- `.app.tar.gz` y `.sig`: paquete firmado para el actualizador.
- `latest.json`: versión, firma y URL pública del paquete.
- `SHA256SUMS.txt`: hashes de los archivos publicados.

Las credenciales siguen en el almacén nativo de la computadora. Las descargas y el historial siguen siendo locales. La consulta del canal no requiere token de GitHub ni acceso al repositorio privado.

Las compilaciones y firmas se hacen localmente. GitHub Actions está deshabilitado en este repositorio; no se contrata hosting ni servicios pagos.
