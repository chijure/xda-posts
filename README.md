# XDA Posts

Colección de 37 publicaciones exportadas o preparadas para el foro XDA Developers en formato BBCode. Incluye kernels, ROMs, recoveries y guías para dispositivos Huawei, LG y Alcatel.

## Estructura
- `alcatel/`: 1 post (Phoenix Kernel V1 para POP C1/C2/C3).
- `huawei/`: 8 posts para Huawei Y210 y Y220-U05 (CM7, CM9, CM10, CM10.1, TWRP y stock).
  - `huawei/y210/`: TWRP 3.1.1 y CyanogenMod 7, 9 y 10 para Huawei Y210, con capturas en `screenshots/{cm7,cm9,cm10}`.
  - `huawei/y220/`: TWRP 3.1.1-0.1, ROM stock C482B206 para TWRP y CyanogenMod 7 y 10.1 para Huawei Y220-U05, con capturas en `screenshots/{twrp,cm7,cm101}`.
- `lge/`: 28 posts de la línea Optimus, G2 Mini y L50 (L1 II, L3, L4 II, L5 II, L7 II, G3 Stylus, D625, D213, etc.).
  - `lge/e410/`: ROMs y recoveries para LG L1 II (CWM, TWRP, CM10/11, guías de root/bootloader).
  - `lge/d625/`: desbloqueo del bootloader, TWRP 3.1.1-1 y CyanogenMod 11 para LG G2 Mini LTE D625 (Tegra 4i).
  - `lge/e400/`: Kernel y Aroma installer para LG L3.
  - `lge/p350/`: Kernel Phoenix RC1 para Optimus Me.
  - `lge/d213/`: root y desbloqueo del bootloader, TWRP 3.1.1-0.1 y LineageOS 11 para LG L50 D213 (MT6572).
  - `lge/vee4ss/`: CyanogenMod 10 para LG L4 II E440g.
  - `lge/vee5ss/`: desbloqueo del bootloader y CyanogenMod 10 para LG L5 II E450g.
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
