# VectorLab Mictlán

Aplicación científica para comparar dos vectores en el plano. Incluye magnitudes, suma, resta, producto punto y una gráfica con escala común. La interfaz y las acciones están en `principal.mict`. La matemática y el plano están en `modulos/`. El mismo anfitrión ejecuta aplicaciones con otros controles y acciones.

Desde esta carpeta, ejecuta el anfitrión P1 con el archivo principal.

```bash
/ruta/al/SDK-build/host_ui -- "$PWD/principal.mict"
```

Los datos iniciales son A = (3, 4) y B = (5, 12). Las magnitudes son 5 y 13, la suma (8, 16), la resta (−2, −8) y el producto punto 63. Modifica una componente y pulsa Enter o Calcular. Usa Tab y Mayús+Tab para mover el foco. Los vectores se dibujan en azul y naranja. La misma unidad ocupa el mismo número de píxeles en ambos ejes.

La entrada usa punto decimal y admite exponentes. El valor absoluto de cada componente puede llegar a `1e100`. Una entrada inválida muestra un mensaje y conserva los últimos resultados correctos. Los cálculos usan números de doble precisión. Esta versión conserva los datos durante la sesión.

```bash
/ruta/al/SDK-build/mictlan_ciencia_consola "$PWD/pruebas/operaciones.mict"
```

Los scripts de consola anteriores se conservan en `../aplicacion`. [Repositorio del SDK](https://github.com/TuxMatic99/Mictlan-SDK).
