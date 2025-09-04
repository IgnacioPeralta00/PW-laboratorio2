# PW-laboratorio2

### Pregunta 10
"Actualice la página en su navegador y pregúntese ¿Hay cambios en la visualización del sitio web? Porqué se
dan estos cambios entre tan pocas líneas de diseño CSS."

Al hacer uso de las DevTools en el navegador (F12), se puede observar el icono de **grid** al lado del contenedor al que se le aplicó, mientras que antes aparecia flex. El cambio de diseño ocurre porque flex y grid son dos sistemas de layout diferentes. Al aplicar:

```css .container {
    display: grid;
    grid-template-columns:
        1fr 1fr minmax(10px, 1fr) 3fr repeat(5fr, 1fr) 50px auto 100px 1fr;
}
```

Se crea una estructura de *grid* (o rejillas) con:
- Múltiples columnas de diferentes tamaños
- Uso de unidades fraccionarias (fr)
- Valores fijos (50px, 100px)
- Valores automáticos (auto)
- Valores mínimos/máximos (minmax())