# Voces de DriveRead

Copia propia de los modelos de voz [Piper](https://github.com/rhasspy/piper)
que usa [DriveRead](https://github.com/dancen001-lgtm/driveread), una app
que lee documentos en voz alta.

**Este repositorio no tiene código.** Solo están los modelos, en la
sección [Releases](../../releases), porque la app los descarga desde ahí.

## Por qué existe

Los modelos se bajaban del repositorio de otra persona. Eso funciona
hasta el día en que ese repositorio cambia de sitio o desaparece, y
entonces quien instale la app no puede descargar ninguna voz. Tener la
copia aquí quita ese riesgo: estos archivos no los mueve nadie más.

Todos los modelos se pueden redistribuir. Abajo está la licencia de cada
uno, y en [CREDITOS.md](CREDITOS.md) la atribución de los que la exigen.

## Las voces

| Nombre | Identificador | Región | Tamaño | Licencia del modelo | Licencia de los datos |
|---|---|---|---|---|---|
| Claudia | `es_MX-claude` | México | 63 MB | MIT | Apache 2.0 |
| David | `es_ES-davefx` | España | 60 MB | MIT | CC0 — dominio público |
| Sara | `es_ES-sharvard` | España | 73 MB | MIT | CC BY 3.0 |
| Samuel | `es_ES-sharvard-m` | España | 73 MB | MIT | CC BY 3.0 |
| Kristin | `en_US-kristin` | Estados Unidos | 64 MB | MIT — el autor la donó al dominio público | Dominio público — grabaciones de LibriVox |
| Norman | `en_US-norman` | Estados Unidos | 64 MB | MIT — el autor la donó al dominio público | Dominio público — grabaciones de LibriVox |
| John | `en_US-john` | Estados Unidos | 64 MB | MIT — el autor la donó al dominio público | Dominio público — grabaciones de LibriVox |
| Linda | `en_US-ljspeech` | Estados Unidos | 64 MB | MIT | Dominio público — LJ Speech, de Keith Ito |
| Cori | `en_GB-cori` | Reino Unido | 64 MB | MIT — el autor la donó al dominio público | Dominio público — grabaciones de LibriVox |

Son 8 archivos y 496 MB: Sara y Samuel salen del
mismo modelo, que tiene dos hablantes.

## Comprobar que un archivo está entero

Cada modelo tiene su huella SHA-256 en [HUELLAS.txt](HUELLAS.txt), y la
app la comprueba al descargarlo. Para verificarlo a mano:

```sh
sha256sum -c HUELLAS.txt
```

## Gracias

A **Michael Hansen** y a quienes hacen Piper, y a quienes grabaron y
publicaron las voces y los corpus con licencias que permiten esto.
