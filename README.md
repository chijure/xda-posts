# XDA Posts

Colección de 20 publicaciones exportadas del foro XDA Developers en formato BBCode. Incluye kernels, ROMs, recoveries y guías para dispositivos LG y Alcatel.

## Estructura
- `alcatel/`: 1 post (Phoenix Kernel V1 para POP C1/C2/C3).
- `lge/`: 19 posts de la línea Optimus (L1 II, L3, L7 II, G3 Stylus, etc.).
  - `lge/e410/`: ROMs y recoveries para LG L1 II (CWM, TWRP, CM10/11, guías de root/bootloader).
  - `lge/e400/`: Kernel y Aroma installer para LG L3.
  - `lge/p350/`: Kernel Phoenix RC1 para Optimus Me.
  - `lge/vee7/`: Kernel Phoenix v02 para LG L7 II.
  - `lge/style/`: Kernel Phoenix V2 para G3 Stylus.
  - `lge/`: recursos generales (logos y plantillas de capturas).

## Formato
- Cada archivo `.bbcode` conserva el marcado original de XDA (`[B]`, `[IMG]`, `[LIST]`, etc.).
- El nombre del archivo suele codificar dispositivo, tipo de publicación y versión/fecha, por ejemplo: `[L1 II][KERNEL][4.1.2][ver 07] Phoenix [2015-07-23].bbcode`.

## Cómo usarlo
- Explorar el contenido: `rg --files` o `rg --files lge/e410`.
- Buscar por dispositivo o palabra clave: `rg "TWRP" lge`.
- Vista rápida de un post: `sed -n '1,80p' "lge/e410/[RECOVERY] TWRP 2.8.0.1 for LG L1II.bbcode"`.
- Convertir a otro formato (ej. Markdown) con herramientas como `pandoc` si la tienes instalada: `pandoc -f bbcode -t markdown <archivo>`.

## Añadir más posts
- Guarda el `.bbcode` en la carpeta del fabricante/dispositivo correspondiente.
- Usa nombres descriptivos siguiendo el patrón existente para facilitar las búsquedas.
