+++
title = "DaliaWeb"
extra.toc = true
taxonomies.tags = ["software"]
+++

Lo que estás leyendo ahora mismo.

<!-- more -->

## El Pasado

Originalmente, esta página estaba hecha usando [Jango](@/proyectos/jango.md), una herramienta que hice yo misma para crear plantillas y poblarlas con el contenido de archivos Markdown. A esto le sumé [Magick.css](https://css.winterveil.net/), un tema hecho para estilar HTML semántico. Hice mis ajustes para usar [Catppuccin](https://catppuccin.com), como hago con todas las cosas que uso.

## El Presente

En su estado actual, este sitio está hecho usando [Zola](https://www.getzola.org/), un generador de sitios estáticos escrito en Rust. La parte visual aprovecha el tema [Anemone](https://github.com/Speyll/anemone), aunque con una considerable parte de él modificada para traducirla al español (y para usar Catppuccin otra vez). Otros temas fueron probados, pero este fue el que más se acomodaba a lo que quería hacer con el sitio sin abstraer demasiada funcionalidad, que últimamente sólo restringe la libertad de lo que puedo hacer si quiero hacer más que sólo un blog.

## El Motivo

¿Por qué rehacer la página desde 0 si estaba funcionando perfectamente? Esta es una pregunta incluso más difícil de responder considerando que ya había hecho un programa entero sólo para hacer mi sitio web (en Rust, btw). Pero cuando encontré un blog personal escrito en Zola, quise investigar qué era y encontré un programa que tomó decisiones muy parecidas a las que yo tomé con _Jango_. Está escrito en Rust, usa [Tera](https://keats.github.io/tera/) como sistema de plantillas y hasta TOML como lenguaje para el encabezado de los archivos Markdown.

Yo hice _Jango_ como ejercicio de aprendizaje más que otra cosa. Ya era consciente de las mil y una alternativas mejores que existían cuando comencé a escribirlo, pero quería entender cómo funciona un programa de ese estilo, o como mínimo, cómo implementaría yo las funcionalidades que quería de un generador estático. Obviamente tenía sus limitaciones, tanto que tuve que escribir mi propio script para procesar mi directorio de plantillas usando GNU Parallel. Una vez sentí que entendía lo que estaba haciendo más o menos, el valor de usar mi propia solución decreció considerablemente. Tenía mis dudas de pasarme a herramientas más maduras como Hugo y Astro, pero dudé porque no quería transformar todo mi proyecto (y/o escribir JavaScript). Pero con Zola, los cambios que hice fueron por decisión propia y no por ser forzada a hacerlo. Además, Zola está hecho en Rust.

## La Filosofía

Ahora, ¿por qué usar cualquiera de estas herramientas en lugar de hacer un sitio web a la vieja usanza o, en su lugar, usar cantidades gargantuescas de JS por ningún motivo? Como tal vez se notará por mi tono, no soy muy fan del ecosistema web moderno. Especialmente en el uso extremo de JavaScript para reemplazar tecnologías nativas de la web. Mi página web es un proyecto muy simple, y por ende, quiero usar herramientas simples. Sí, es perfectamente posible que Zola sea un proyecto muy complejo internamente, pero la funcionalidad que expone no es magia, son cosas que yo misma podría haber terminado implementando con el suficiente tiempo y necesidad.

## El Futuro

Desde la re escritura de todo el sitio, me siento bastante cómoda con el estado en que se encuentra el proyecto. Mi objetivo ahora es ponerme a escribir de verdad, tanto en el [blog](@/blog/_index.md), como mis propios proyectos narrativos. La escritura siempre ha sido mi pasión, y es momento de dejar de procrastinar en ella escribiendo código.

## El Futuro Perdido

Originalmente quería albergar mis escritos narrativos en este mismo sitio, pero creo que he decidido en contra de eso. Aunque me guste mucho el estilo visual que tiene ahora mi sitio, no es el más apropiado para leer algo menos orientado a la tecnología. Por esto, he decidio que eventualmente haré otro proyecto para tener mis escritos allí, donde no tengan que entrar en un conflicto estilístico con lo que hay aquí ahora. Cuando este nuevo sitio esté listo, podrás leer todo sobre él [aquí](@/proyectos/_index.md).
