---
layout: post
title: "Introducción a WebdriverIO"
---

# Testing de Software
Es el ejercicio de comparar el resultado actual de una aplicación, con el resultado esperado.
Nosotros escribimos pruebas en un formato estándar para definir cómo se prueba. 
Hoy nos vamos a centrar en un tipo de pruebas en particular.

# Testing Automatizado

Algunas tareas son repetitivas y difíciles de seguir 
* Se opta por una automatización que agiliza las pruebas.
* Se reduce el error humano al tener menos interacciones.
* Son robustas, ya que siempre devuelven el mismo resultado (o es lo que se espera)

**NOTA**: No todo se puede automatizar.

# ¿Qué es NPM?

Es un gestor de paquetes de NodeJS para instalar dependencias. Solo se requiere tener instalado el NodeJS en nuestro equipo.

# ¿Qué es Cucumber?

Es un framework para escribir escenarios de prueba en Gherkin.
Gherkin es un lenguaje para comunicar entre los diferentes equipos (Dev, QA, Negocio).

Usamos las siguientes palabras clave:

~~~gherkin
Given para las precondiciones
When para la acción que dispara un evento
Then para validar un resultado posterior
~~~

# ¿Qué es WebdriverIO?
Es un framework para pruebas de UI que usa Typescript como lenguaje.
Soporta pruebas para web y para mobile (Appium), y viene con soporte nativo para pruebas en la nube (BrowserStack, SauceLabs).

Podemos crear escenarios de pruebas  con Gherkin y definir los pasos (steps) con typescript para que el framework genere un comportamiento. 

# Selectores
Son elementos que nos permiten identificar partes del HTML, y realizar operaciones sobre los mismos. Algunos de los selectores más importantes son:
- **`id`** : Son aquellos que vienen con un identificador único. Los IDs son únicos, es decir, no pueden existir más de un elemento con el mismo ID.

    ~~~html
    <p id="super-parrafo"> Este es un párrafo de ejemplo </p>
    ~~~

- **`class`**: Es un identificador que utilizamos para asignar atributos a más de un elemento en el HTML.
    ~~~html
    <p class="conceptos"> Los párrafos tienen como identificador </p>
    <p class="conceptos"> class serán destacados en color especial </p>
    ~~~
- **`xpath`**: Es la ruta completa hacia un elemento desde el elemento raíz. Existen dos tipos (absoluto y relativo), en el cual, uno se define desde el elemento raíz, mientras que el segundo usa comodines para accede a un determinado elemento.  

## Material adicional
[¿Qué es un patrón de diseño?](https://refactoring.guru/es/design-patterns/what-is-pattern)

[¿Qué es Cucumber y cómo agilizar el testing?](https://elminimoviable.es/que-es-cucumber-y-como-agilizar-el-testing/)

[WebdriverIO: Web Test Automation desde cero con Cucumber y Typescript](https://www.youtube.com/watch?v=Nqtpk22sDqI)
