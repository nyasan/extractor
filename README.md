extractor
=========

Proyecto de extracción de datos de distintas fuentes con exportación a otras distintas.
Inicialmente creado con el objetivo de servir como fuente de datos al proyecto [__Memoria__](https://github.com/init-sfw/memoria)


## Versión actual

En la segunda versión de la app se hace una evolución a una arquitectura más seria pero aún inmadura, a modo de POC y con necesidad de mucha refactorización.

Sin tests, sin resoluciones arquitectónicas eficientes y sin performance.
Escribe JSON de salida procesable por [Memoria](https://github.com/init-sfw/memoria).

Se encuentra procesando unas 500 páginas de Wikipedia, con requests individuales, sobre torneos de fútbol (responden al template  [Ficha de torneo de fútbol](http://es.wikipedia.org/wiki/Plantilla:Ficha_de_torneo_de_f%C3%BAtbol) de las que extrae el infobox correspondiente y lo transforma en un evento operable por Memoria.

## Ejecución

El proyecto está desarrollado en Java y consta de una arquitectura inestable y con chanchadas.
La parametrización es manual desde el código, sin interfaz.
La salida falta ser parseada por un conversor de MediaWiki a HTML o lo que el formato de evento de [Memoria](https://github.com/init-sfw/memoria) necesite.

## Próximo paso

La próxima versión tendrá como objetivo permitir trabajar con alguna otra plantilla de Wikipedia desde una parametrización interna.

## Más información

Más información sobre la investigación en marcha puede encontrarse en este documento (necesita permiso de acceso): https://docs.google.com/document/d/1oZ-4i0lSLBRiJDw0nS-wjFz4FVfhr-J-E1FOV8u3hv0
