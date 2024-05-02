+++
title = "Tasker"
extra.toc = true
taxonomies.tags = ["rust", "software"]
+++

Una aplicación de terminal para administrar tus tareas.

<!-- more -->

## ¿Qué Es Tasker?

La idea es que sean tres aplicaciones: Una de línea de comando, una con interfaz de terminal y una aplicación gráfica; todas hechas en Rust. Sólo la primera está implementada debido a la absurda cantidad de aplicaciones de tareas que ya existen, entonces decidí priorizar otros proyectos por el momento.

## ¿Cómo Funciona?

Tasker guarda tus tareas en un archivo [RON](https://github.com/ron-rs/ron). Estas tareas tienen los siguientes campos:

| Campo       | Obligatorio                  | Tipo    |
| ----------- | ---------------------------- | ------- |
| Descripción | Sí                           | String  |
| Estado      | Sí ("Por hacer" por defecto) | Enum    |
| Proyecto    | No                           | String  |
| Etiquetas   | No                           | HashSet |

También puedes configurar algunos campos de la aplicación con un archivo [TOML](https://toml.io/en/). Puedes averiguar dónde debe estar este archivo en tu plataforma con el comando `tasker-cli paths`.

| Campo      | Tipo                               |
| ---------- | ---------------------------------- |
| name       | String                             |
| language   | String, sólo "Spanish" ó "English" |
| to_do_path | Path                               |

Puedes ver los detalles de cómo está todo esto implementado [aquí](https://github.com/DavoReds/tasker).

## El Futuro De La Aplicación

No elimino la posibilidad de terminar implementando las otras dos encarnacioines de la aplicación, que serían interoperables entre sí y leerían del mismo archivo de tareas.

Hay un par de ajustes que me gustaría hacerle a la versión de CLI y que seguramente terminarán siendo implementadas en las próximas semanas. Específicamente quiero hacer que los comandos sean más limpios y menos confusos de usar. Hay también otros temas que me gustaría explorar en cuanto a cómo están guardadas las tareas (desde investigar codificación binaria hasta usar SQLite), pero ese tema es menos probable porque implicaría romper las tareas de todos los usuarios. Obviamente habría que implementar un comando para migrar las tareas de un formato a otro, pero muy pocas personas prestan atención a cuando actualizan sus programas.

Veremos dónde termina esto si decido trabajar en las otras versiones.
