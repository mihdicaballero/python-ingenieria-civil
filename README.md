# python-ingenieria-civil

Análisis y diseños creados por estudiantes del curso «Python para Ingeniería Civil: Cálculo Estructural y Reportes».

Cada carpeta es un problema resuelto con el método del curso: un plan, el cálculo en funciones, una tabla de resultados y una verificación contra un caso conocido. Puedes usarlos, corregirlos y subir los tuyos. Un problema no es de nadie: si encuentras un error o le agregas un caso, lo mejoras ahí mismo.

## Cómo se organiza

Una carpeta por tema y, adentro, una carpeta por problema, con un nombre corto que diga qué resuelve. Sin nombres de persona: el problema es del repositorio, y GitHub ya guarda quién escribió cada línea.

| Tema | Qué va |
|:--|:--|
| [`hormigon`](problemas/hormigon) | Chequeos y dimensionado de vigas, columnas, losas |
| [`acero`](problemas/acero) | Perfiles, uniones, placas base |
| [`fundaciones`](problemas/fundaciones) | Zapatas, pilotes, tensores |
| [`cargas`](problemas/cargas) | Combinaciones, sismo, viento, cargas por nivel |
| [`procesar-modelo`](problemas/procesar-modelo) | Leer y ordenar las tablas que exporta el software de cálculo |
| [`utilidades`](problemas/utilidades) | Planillas de doblado, conversiones, granulometría y lo que no entre arriba |

Si tu problema no entra en ninguno, ponlo en `utilidades`; cuando haya varios parecidos, se abre un tema nuevo.

Cada problema lleva tres cosas. Puedes partir de la carpeta [`_plantilla`](problemas/_plantilla):

```
problemas/hormigon/flecha-viga-simple/
    flecha-viga-simple.ipynb
    LEEME.md
    datos/
        vigas.xlsx
```

- **El notebook**, con la forma del curso: empieza con el plan (qué entra, qué se calcula, qué sale, contra qué se verifica) y termina con la verificación. Súbelo ejecutado, con las salidas a la vista, para que se pueda leer sin correrlo.
- **`LEEME.md`**, cinco líneas: qué resuelve, con qué norma, qué datos necesita, contra qué se verificó y qué no cubre.
- **`datos/`**, solo si el notebook lee archivos, y solo con un ejemplo chico.

**Un notebook sin plan o sin verificación no entra.** Es justamente lo que le permite a otro confiar en él.

## Qué no se sube

- **Datos de proyectos reales.** Nombres de clientes, de obras o de colegas, planos, modelos. Cambia los datos por un ejemplo inventado antes de subir.
- **Normas, libros o páginas escaneadas.** Cita el artículo; no subas el PDF.
- **Los notebooks del curso.** Sube lo que hiciste tú a partir de ellos, no el material de las clases.
- **Archivos pesados.** Si pasa de unos pocos megas, no es un ejemplo.

## Subir un problema nuevo

Todo desde el navegador, sin instalar nada:

1. Crea una cuenta gratuita en github.com, si no tienes una.
2. Pulsa **Fork** arriba a la derecha. Eso crea una copia tuya, donde puedes escribir.
3. Arma en tu computadora la carpeta del problema, con el notebook y el `LEEME.md`.
4. En tu copia, entra a `problemas/` y al tema que corresponde, pulsa **Add file → Upload files** y arrastra la carpeta entera.
5. Escribe una línea que diga qué subiste y pulsa **Commit changes**.
6. Pulsa **Contribute → Open pull request** y confirma. Se revisa que tenga plan y verificación, y queda publicado.

## Mejorar uno que ya está

Si un problema tiene un error, le falta un caso o se puede hacer más claro, lo corriges: abre el archivo, pulsa el lápiz (**Edit**), o baja el notebook, corrígelo y vuelve a subirlo encima en la misma carpeta. Explica en una línea qué cambiaste y por qué, y abre el pull request.

Si el cambio toca un resultado, la verificación tiene que seguir pasando, o el pull request tiene que explicar por qué el valor esperado estaba mal. Un cambio que hace pasar la verificación tocando el valor esperado, sin explicar de dónde sale el nuevo, no entra.

## Reusar el problema de otro

GitHub muestra los notebooks en pantalla, así que puedes leer el plan y los resultados antes de bajar nada. Para bajarlo, abre el notebook y pulsa *Download raw file*; si usa archivos de `datos/`, bájalos también y respeta la misma carpeta. Para abrirlo en Colab sin bajarlo, cambia `github.com` por `colab.research.google.com/github` en la dirección del notebook.

Antes de usar un número que salga de acá, trátalo como cualquier código que no escribiste: lee el plan, mira contra qué se verificó y córrelo con un caso que tú ya tengas resuelto.

**Lo que hay en este repositorio se comparte como está, bajo la [licencia MIT](LICENSE). La responsabilidad del cálculo que entregas sigue siendo tuya.**
