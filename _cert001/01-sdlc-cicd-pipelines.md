---
title: "Implementar pipelines CI/CD"
permalink: /cert001/sdlc-cicd-pipelines/
excerpt: "Los pipelines de CI/CD se diseñan para optimizar implementaciones y despliegues con mayor rapidez."
last_modified_at: 2021-06-07T08:48:05-04:00
redirect_from:
  - /theme-setup/
toc: true
---


Imagínate que estás construyendo un coche con un equipo de amigos. En lugar de que cada uno construya una parte enorme (motor, chasis, ruedas) por separado durante meses y al final intenten juntarlo todo (lo que sería un caos de piezas que no encajan), deciden hacerlo de otra manera.

Esta nueva manera se llama **CI/CD**, que son las siglas de **Integración Continua** y **Entrega Continua**. Piénsalo como una cadena de montaje moderna para crear software.

## CI: Integración Continua (Juntar las piezas a cada rato)

La parte de **CI (Integración Continua)** es como si cada vez que un amigo termina de ajustar un tornillo o conectar un cable (un pequeño cambio en el código), lo añade inmediatamente al coche principal (la rama principal del código). Se espera que esto ocurra con frecuencia, idealmente a diario.

Pero aquí viene la magia: en cuanto añade su pieza, **un robot supervisor (un proceso automático) revisa todo el coche al instante**. Este robot hace varias cosas:
*   **Comprueba que el coche sigue arrancando** (que el código se puede compilar).
*   **Hace pruebas para asegurarse de que la nueva pieza no ha roto nada que ya funcionaba** (esto se llama pruebas automatizadas, como las pruebas unitarias).

Si el robot detecta un problema (por ejemplo, una prueba falla), avisa al equipo de inmediato para que lo arreglen al momento. Hacer cambios pequeños y frecuentes hace que, si algo sale mal, sea muchísimo más fácil y rápido de encontrar y arreglar.

## CD: Entrega Continua (Dejar el coche listo para entregar)

Una vez que el robot da el visto bueno, pasamos a la parte de **CD (Entrega Continua)**. Esto significa que el coche (tu software) está automáticamente empaquetado y listo para ser entregado al cliente. Aquí hay dos sabores:

1.  **Entrega Continua (Continuous Delivery):** El proceso automático deja el coche listo y con las llaves puestas, pero **una persona tiene que pulsar el botón final** para entregárselo al cliente.
2.  **Implementación Continua (Continuous Deployment):** Este es el nivel pro. Aquí, el robot no solo prepara el coche, sino que **lo conduce él mismo hasta la puerta del cliente sin que nadie tenga que intervenir**. El software se actualiza para los usuarios de forma totalmente automática.

## ¿Y por qué mola tanto el CI/CD?

*   **Menos dolores de cabeza:** Te despides de las integraciones gigantes y terroríficas. Al hacer pequeños cambios, los errores son más pequeños y fáciles de solucionar.
*   **Más velocidad:** Puedes lanzar nuevas funcionalidades y mejoras a tus usuarios mucho más rápido, en lugar de esperar meses.
*   **Mejor calidad:** Como todo se prueba constantemente de forma automática, te aseguras de que el producto sea estable y de alta calidad.
*   **Seguridad desde el principio:** La seguridad no es algo que se mira al final. Se integra en cada paso del proceso, desde analizar el código en busca de fallos hasta proteger contraseñas y datos sensibles.
*   **Clientes más contentos:** Los usuarios reciben mejoras constantemente y pueden dar su opinión mucho antes. Esto ayuda al equipo a construir lo que la gente realmente necesita.

En resumen, **CI/CD es una forma de trabajar en equipo que usa la automatización para construir, probar y entregar software de manera rápida, segura y fiable**. Al principio puede costar un poco acostumbrarse a este ritmo, pero a la larga, los beneficios de ser más ágil y preciso son enormes.
