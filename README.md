# TEO CONTROL R1 - Carcasa

Carcasa impresa en 3D para la tarjeta TEO CONTROL R1 (RPI-TK), controlador de fajon termico.
Disenada en Autodesk Fusion (documento CARA_TEO, carpeta CLAUDE).

## Archivos

| Archivo | Contenido |
|---|---|
| `CARA_TEO.f3d` | Archivo fuente de Fusion (historial parametrico completo) |
| `CARA_TEO.step` | Cara + cuerpo en STEP (intercambio CAD) |
| `stl/TEO_CARA_Y_CUERPO.stl` | Ambas piezas orientadas para imprimir |
| `stl/TEO_CARA.stl` / `stl/TEO_CUERPO.stl` / `stl/TEO_CONTRAMARCO.stl` | Piezas por separado |

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
- Marco de sujecion continuo (10 mm hacia afuera, 3 mm de espesor), 12 mm bajo la cara, con 16 huecos de 4 mm y nervios a 45 grados por encima
- Contramarco de 3 mm con los mismos 16 huecos: se atornilla bajo el marco y pellizca la tela del fajon
- Agujeros para buzzer y rejillas de ventilacion en la franja expuesta

## Impresion

- Cara: superficie visible sobre la cama
- Cuerpo: fondo sobre la cama (el marco necesita soporte)
- `stl/CARA_CUERPO_TEO.stl`, `stl/CARA_TEO.stl`, `stl/CUERPO_TEO.stl`, `stl/AGARRE_TEO.stl`: ya orientados y apoyados en Z=0
- `CUERPO_TEO.stl` y `CARA_CUERPO_TEO.stl` traen soportes integrados bajo el marco: 148 aletas de 0.8 mm cada 2.5 mm,
  0.2 mm por debajo del marco y 0.6 mm separadas de la pared. Imprimir con los soportes del laminador desactivados
  y retirar las aletas a mano
- Insertos termicos M3 con cautin a ~240 C (PETG)

## Pendientes

- NFC embebido detras del QR (bolsillo interno + pausa de capa)
- Aislamiento Kapton/papel pescado entre convertidor y rele si hace falta
