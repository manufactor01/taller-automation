---
layout: post
title: "Practicas con WebdriverIO"
---

## Checking de ambientes
1. Acceder al siguiente [link](https://github.com/manufactor01/starter-webdriverio) y clonar el repositorio de pruebas.

2. Abrir el proyecto en consola y ejecutar el comando **`npm install`**. (En caso de fallar, ejecute el comando **`npm install --legacy-peer-deps`**).

3. Ejecutar el comando **`npm run start-web`**.

Con estos pasos, nos aseguramos de que se ejecutan las pruebas definidas en el framework.

## Ejercicios
Vamos a trabajar con la página [Saucedemo](https://www.saucedemo.com/), una página de prácticas para el testing automatizado.

Para esta página se pide:

1. Crear un archivo **`Gherkin`** con nombre **`saucedemo.feature`**, y con el editor de texto, escribir el escenario de pruebas para el siguiente caso:

    _"Login correcto (ver credenciales del recuadro oscuro)."_

    Se recomienda realizar una pequeña [prueba exploratoria](https://www.atlassian.com/es/continuous-delivery/software-testing/exploratory-testing) para conocer la página de pruebas.

2. Crear los *"Step Definitions"* en el archivo **`stepDefinitions.ts`** para los escenarios definidos y realizar las implementaciones necesarias para ejecutar las pruebas.

    Se pueden apoyar de [Tidy Gherkin](https://chrome.google.com/webstore/detail/tidy-gherkin/nobemmencanophcnicjhfhnjiimegjeo?hl=en-GB) para hacer la escritura de los stepDefinitions desde los escenarios en Gherkin.

3. Una vez implementado, ejecutar las pruebas con el comando **`npm run start-web`**. Al finalizar, ejecutar el comando **`npm run clean-report`** para generar el reporte, con las capturas de la última prueba ejecutada. Para abrir el reporte, se tiene que ejecutar el comando **`npm run open-report`**.

4. Crear los escenarios de prueba e implementar los pasos en el archivo de *"Step Definitions"* para los siguientes casos:

    * _Login incorrecto._

    * _El usuario se loguea en la aplicación, y agrega elementos al carrito._

    * Un caso que se te ocurra probar.

5. Crear un archivo **`saucedemo.page.ts`** y definir una clase llamada **`SaucedemoPage`** que contenga las implementaciones para obtener los selectores de la página. Una vez definida la clase, importarlo en los **`stepDefinitions.ts`** y obtener los elementos de la página usando los métodos definidos para la clase **`SaucedemoPage`**.

    Esta modificación se conoce como el patrón [Page Object Model](https://www.tutorialselenium.com/2019/02/05/page-object-model-selenium-webdriver/), que garantiza que las pruebas sean más escalables al definir la responsabilidad de obtener y manipular los elementos de la web mediante una clase *"pages"*. 