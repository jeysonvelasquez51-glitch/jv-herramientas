# jv-herramientas

Publicación de las actualizaciones de la suite **Justicia Virtual · LegalTools**.

## Qué hay aquí

Este repositorio **no contiene código**. Solo:

| Archivo | Qué es |
|---|---|
| `version.json` | Versión publicada, firmas y enlaces de descarga |

Los ejecutables van como **adjuntos de cada release**, no en el repositorio.

## Cómo se actualizan las herramientas

Cada herramienta consulta `version.json` una vez al día. Si hay una versión más nueva,
**avisa y pregunta**: nada se instala sin que el usuario lo acepte.

Al aceptar, se descarga el ejecutable y se comprueba su **firma Ed25519** contra la clave
pública que la herramienta ya lleva dentro. Un archivo alterado —o subido por cualquiera
que no tenga la clave privada— no supera esa verificación y no se instala.

## Descargar a mano

Las versiones están en [Releases](../../releases/latest). Los ejecutables **necesitan una
licencia** para funcionar; sin ella no abren.

Para una instalación nueva no basta con el ejecutable: hacen falta las dependencias
(Ghostscript, Tesseract, ffmpeg, navegador). Solicite el instalador completo.
