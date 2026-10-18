# TVM — Guía interactiva del Teorema del Valor Medio

Sitio web educativo construido con [Quarto](https://quarto.org) que presenta el
Teorema del Valor Medio (Lagrange), cinco ejercicios resueltos con pistas y
soluciones desplegables, una interpretación gráfica generada con Python y una
presentación Reveal.js.

## Contenido

- **Teorema del Valor Medio**: enunciado formal con entorno de teorema, ecuación
  numerada y referencia cruzada.
- **Ejercicios**: cinco problemas en LaTeX con pistas y soluciones plegables
  (callouts).
- **Tabla resumen**: funciones, intervalos, pendientes medias y valores de `c`
  para cada ejercicio.
- **Interpretación geométrica**: gráfico generado con Python (matplotlib) que
  muestra la tangente paralela a la secante.
- **Presentación**: cuatro diapositivas en Reveal.js con tema oscuro y
  transiciones animadas.

## Estructura

    tvm-quarto/
    ├── _quarto.yml          # Configuración del sitio
    ├── index.qmd            # Teorema, ejercicios, tabla y gráfico
    ├── presentacion.qmd     # Presentación Reveal.js
    ├── images/
    │   └── tvm-grafico.png  # Gráfico generado por Python
    └── docs/                # Sitio renderizado (generado)

## Requisitos

- [Quarto](https://quarto.org/docs/download/) 1.9 o superior
- Python 3.11+ con `jupyter`, `numpy` y `matplotlib`
- (Opcional) Un entorno virtual con `virtualenvwrapper`

## Cómo construir el sitio

```bash
# Activar el entorno con Python
workon tvm

# Previsualizar en local
quarto preview

# Renderizar a docs/
quarto render
