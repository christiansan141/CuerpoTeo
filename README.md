# TEO CONTROL R1 - Carcasa

Carcasa impresa en 3D para la tarjeta TEO CONTROL R1 (RPI-TK), controlador de fajon termico.
Disenada en Autodesk Fusion (documento CARA_TEO, carpeta CLAUDE).

## Archivos

| Archivo | Contenido |
|---|---|
| `CARA_TEO.f3d` | Archivo fuente de Fusion (historial parametrico completo) |
| `CARA_TEO.step` | Cara + cuerpo en STEP (intercambio CAD) |
| `stl/TEO_CARA_Y_CUERPO.stl` | Ambas piezas orientadas para imprimir |
| `stl/TEO_CARA.stl` / `stl/TEO_CUERPO.stl` | Piezas por separado |

## Especificaciones

- Material: PETG
- Altura total: 28 mm (cara 2 mm + cuerpo 26 mm); 15.4 mm libres bajo la PCB
- Cara: 60 x 121.8 mm, ventana OLED 24 x 14 mm con esquinas R1.5 y borde suavizado R0.6
- Interior: 122 mm de largo (incluye compartimento del convertidor AC-DC)
- Paredes y fondo: 2 mm
- Union cara-cuerpo: escalon (holgura 0.2 mm/lado) + 4 tornillos M3 con insertos termicos (piloto 4.0 mm, prof. 10 mm), simetricos a 4.5 mm de cada borde
- Barrera de 1.1 mm entre convertidor AC-DC y tarjeta
- Salidas de cables por el fondo: 4 ranuras de 7.5 mm (simetricas)
- Anclajes para brida en la salida de 120 V (borneras)
- Orejas con hueco de 4 mm en los 4 lados, 10 mm bajo la cara, con nervios a 45 grados
- Agujeros para buzzer y rejillas de ventilacion en la franja expuesta

## Impresion

- Cara: superficie visible sobre la cama
- Cuerpo: fondo sobre la cama
- Insertos termicos M3 con cautin a ~240 C (PETG)

## Pendientes

- NFC embebido detras del QR (bolsillo interno + pausa de capa)
- Aislamiento Kapton/papel pescado entre convertidor y rele si hace falta
