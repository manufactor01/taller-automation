---
layout: post
title: "Introducción a WebdriverIO"
---

# Testing de Software
Es el ejercicio de comparar el resultado actual de una aplicación, con el resultado esperado.
Nosotros escribimos pruebas en un formato estándar para definir cómo se prueba. 
Hoy nos vamos a centrar en un tipo de pruebas en particular.

# Testing Automatizado
Algunas tareas son repetitivas y difíciles de seguir -> Se opta por una automatización que agiliza las pruebas.
-> Se reduce el error humano al tener menos interacciones.
-> Son robustas, ya que siempre devuelven el mismo resultado (o es lo que se espera)

**NOTA**: No todo se puede automatizar

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

## Tidy Gherkin

# ¿Qué es WebdriverIO?
Es un framework para pruebas de UI que usa Typescript como lenguaje.
Soporta pruebas para web y para mobile (Appium), y viene con soporte nativo para pruebas en la nube (BrowserStack, SauceLabs).

Podemos crear escenarios de pruebas  con Gherkin y definir los pasos (steps) con typescript para que el framework genere un comportamiento. 

# Selectores

## Selectors HUB

# Comprendiendo el framework
