# Lime 🍋
Overview and use of LimeSeg
## Basic controlls

- CTRL + T abre el  **ROI manager**
- Seleccionar la herramienta de **elipse**, dibujar la semilla y pulsar T para añadir.
- Plugins -> Limeseg -> Sphere Seg para segmentar.
- **NO cerrar ninguna ventana**
- **Hay que esperar a que 3D deje de moverse o pararlo automáticamente**

## Main functions

### Reutilizar seeds pero mantener la misma configuración
Si las semillas están bien elegidas pero necesitamos modificar los parámetros de segmentación.

- Plugins → LimeSeg → ClearAll

Y procedemos a segmentar de nuevo

- Plugins → LimeSeg → Sphere Seg

### Nueva segmentación completa

En este caso no guardamos las semillas.
- Roi Manager -> Delete
-Plugins → Limeseg → Clear All

### Modificar seeds 🔭
Podemos añadir o eliminar seeds manteniendo las anteriores. Lo ideal es ir añadiendo semillas poco a poco e ir probando qué configuración es la mejor.

- LimeSeg → Clear All
- Roi Manager → Add/Delete Seeds
- LimeSeg → Sphere Seg

### Exportar resultados

LimeSeg nos permite guardar las células que hemos segmentado en formato ply, donde habrá una carpeta por cada célula. Hay que tener cuidado porque **se obreescribe lo anterior**

- LimeSeg → Show GUI
- Write To : Seleccionar Carpeta    
- Save State To XMLPLY

