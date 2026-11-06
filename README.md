
# Mictlán Lab

Laboratorio visual desarrollado con Mictlán.

## Objetivo

Construir una aplicación de referencia para probar y
mejorar las capacidades de Mictlán como lenguaje de
programación de propósito general.

## Arquitectura

- mictlan-core: intérprete y máquina virtual.
- mictlan-sdk: interfaces y bibliotecas reutilizables.
- mictlan-lab: aplicación que utiliza esas bibliotecas.

Mictlán Lab no debe modificar directamente el núcleo
ni contener implementaciones duplicadas del SDK.

## Requisitos actuales

- Debian GNU/Linux x86_64.
- Mictlán Core compilado.
- Mictlán SDK compilado.
- Raylib y OpenGL funcionales.

## Ejecutar

Desde el directorio ~/Proyectos/Mictlan:

    ./build-sdk-debug/host_ui \
      mictlan-lab/aplicacion/inicio.lat

## Funcionalidades verificadas

- Ventana gráfica.
- Etiquetas.
- Botones.
- Eventos.
- Actualización del estado visual.
- Cierre de ventana.

## Próximo objetivo

Crear un lienzo 2D reutilizable, permitiendo dibujar
figuras geométricas desde programas escritos en Mictlán.

## Estado

Prototipo local experimental.
Todavía no constituye una distribución pública.
