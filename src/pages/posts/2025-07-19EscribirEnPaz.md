---
layout: ../layouts/layBlog.astro

title: Haciendo un pequeño blog en php
author: SuliShade
description: "Investigando como hacer un blog sin hacer una odisea"
#image:
#    url: "https://docs.astro.build/default-og-image.png"
#    alt: "The word astro against an illustration of planets and stars."
pubDate: 2025 07 19
tags: ["programacion"]
---

## Investigación sobre cómo poder escribir tranquilamente en Neocities sin hacer una odisea

![chica anime escribiendo en la pc a 4 manos](https://sulishade.neocities.org/img/blog/type-computer-squid-girl.webp)

¡Bueeenas! He estado toda la tarde hoy haciendo una gran investigación de **CÓMO PINCHES ESCRIBIR EN PAZ** en formato puro HTML. La verdad, puede que haya mejores maneras, pero te voy a contar mi aventura.

Hoy tenía ganas de programar. Me puse como objetivo estar algunos días dándole full a la programación porque para algo estoy estudiando esta carrera, ¿no? Así que me puse manitas a la obra a mejorar un blog en PHP, cosa que no debería haber hecho porque la idea era hacer un blog de cero, pero bueno, yo qué sé, igual aprendí. El caso es que, la verdad, mientras hacía el proyecto me di cuenta de algo muy importante: PHP es demasiado cómodo para hacer lo que quiero hacer. Es literal programar páginas web y unir bases de datos. La verdad, nunca me había puesto a hacer algo así. He aprendido un montón, pero mientras hacía todo esto, una pregunta rondaba por mi cabeza: ¿si aplico todo esto a mi blog?

No te voy a mentir… ¿todo este trabajo literal para solo mi portafolio? Ok, es buen plan, ¿pero no hay alguna manera de aplicar todo esto a esta gran página web? Pues por azares del destino encontré la respuesta.

Lo primero que se me ocurrió fue comenzar con un nuevo programa, el cual transformara archivos de Markdown en HTML. Me parece una gran idea, pero hay unos pequeños problemas: sí o sí me toca enlazar manualmente todo lo que escriba, cosa que la verdad es muuuy molesta y me ahorra 2% del trabajo. En el PHP he implementado un sistema de tags, cosa que me parece completamente necesaria debido a la ambición del proyecto y a que escribo como un enfermo de diferentes temas que no tienen mucha relación entre sí. También estoy demasiado acostumbrado a usar Markdown ya que llevo ya un buen tiempo usando Obsidian. Entonces, ¿qué hago? Decidí mirar si podría montar todo un sistema en Python, pero me di cuenta de que es demasiado ambicioso y que no iba a ningún lado. Pero ahí me di cuenta de que la respuesta la tenía al frente mío.

Si has usado alguna vez Linux o has descargado algo por internet desde la terminal, sabes que existe un comando llamado `wget`, un comando simple que te permite descargar cosas desde internet por la línea de comandos. Pero no solo eso: te permite también descargar sitios web y cosas por el estilo. PHP te hace el sitio completo, así que pensé: ¿qué pasa si descargo mi sitio de PHP con wget? **¡EUREKA!**

Aquí te dejo el comando:

```
wget -r -p -k -e robots=off --html-extension --convert-links --restrict-file-names=windows -U Mozilla http://homepage_here.php
```

Es literalmente hermoso. En unos pocos segundos tenía mi sitio web completo en HTML en mi PC. No sé cómo describirlo, pero fue una sensación de **¡LO HICE, LO HICE, CHINGADAMADRE!** Aunque quizás es la cosa más sencilla de todas jajajaja.

También voy a anexar algunas páginas web que he encontrado si quieres escribir y convertir tus archivos de Markdown a HTML:

- [https://stackedit.io/](https://stackedit.io/)
- [https://markdowntohtml.com/](https://markdowntohtml.com/)

Espero que te haya gustado mi aventura con mi página web :3
