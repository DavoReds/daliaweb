+++
title = "Jango"
taxonomies.tags = ["rust", "software"]
+++

Una aplicación para manejar plantillas desde el terminal.

<!-- more -->

## ¿Qué Es?

Una aplicación para usar plantillas inspiradas en _Jinja_. Es como solía estar hecha esta página. Fue hecha con la intención de ser usada con archivos Markdown y HTML, pero no hay motivos para no usarla con cualquier otro archivo de texto que use plantillas del formato [Tera](https://keats.github.io/tera/).

Todo el código y una guía de cómo usar _Jango_ (en inglés) se encuentra en el [repositorio](https://github.com/DavoReds/jango).

## ¿Cómo Lo Uso?

Como [esta página](@/proyectos/daliaweb.md) ya no está hecha con él, mi uso principal de _Jango_ es en mis notas para [Obsidian](https://obsidian.md).

Mi bóveda tiene la siguiente estructura (Hay más carpetas, pero no son relevantes para esta explicación):

```
.
├── Diario
│   └── ...
├── Plantillas
│   ├── diario.md
│   └── nota.md
└── Zettelkasten
    └── ...
```

Con _Jango_, cada vez que necesito una nueva entrada en mi diario, sólo tengo que ejecutar el siguiente comando:

```sh
jango args Plantillas/diario.md <output>
```

Y una nueva entrada será creada con toda la información que requiero para sólo entrar y escribir lo que necesito.
