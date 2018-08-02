---
title: "Pyton"
subtitle: "Introducción"
author: "jcb"
date: "23 de julio de 2018"
output: 
  ioslides_presentation:
    logo: ./images/LOGOUNC.gif
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(python.reticulate = FALSE)
```


## El lenguaje Python

 * Lenguaje de programación multipropósito y multiplataforma
    * Muy versátil, apto para aplicaciones de escritorio, de servidor y/o aplicaciones web
    * Independiente del sistema operativo
 * Creado por el holandés Guido Van Rossum a fines de la década de 1980
    * Previsto para inetractuar el sistema operativo _amoeba_
        * Un sistema de tiempo compartido que hiciera que una red entera de computadoras pareciera a los ojos de un usuario como una máquina única.
        * Actualmente el desarrollo del sistema operativo parece detenido.

<div class="notes">
A separate presenter window can also be opened (ideal for when you are presenting on one screen but have another screen that is private to you). The window stays in sync with the main presentation window and also shows presenter notes and a thumbnail of the next slide. To enable presenter mode add ?presentme=true to the URL of the presentation. For example:

my-presentation.html?presentme=true

The presenter mode window will open and will always re-open with the presentation until it is disabled with:

my-presentation.html?presentme=false
</div>

---

## Caracerísticas de Python

 * Lenguaje de alto nivel
    * Se asemeja al lenguaje humano, con una sintaxis semejante al idioma inglés
        * Una persona que domine el idioma inglés, podrá deducir qué hace un programa escrito en python aún sin saber programar.
    * Gramática clara y legible
        * Extremadamente fácil de aprender
           * Prescinde de símbolos especiales (punto y coma al final de cada sentencia, etc)
           * La curva de aprendizaje del lenguaje es empinada (en poco tiempo se aprende mucho)

---

## Caracerísticas de Python

 * Interactivo
     * Se puede modificar un programa mientras éste se encuentra activo
     * Los programas interactivos durante su ejecución pueden leer datos del teclado y escribir resultados en la pantalla
 * Interpretado
     * El código no necesita ser preprocesado por un compilador
     * Cada instrucción se traduce a lenguaje máquina y - si no se detectan errores - se ejecuta inmediatamente

---
        
## Caracerísticas de Python
 * Fuertemente tipado
    * Distingue claramente el tipo de la variable (entera, carácter, etc)
    * Si se pretende utilizar una variable de un determinado tipo cuando debe ser de otro, se produce un error
 * El tipado es dinámico
    * Se establece el tipo de una variable de manera dinámica, es decir, en tiempo de ejecución
    * No es necesario declarar previamente el tipo de la variable.
        
## Caracerísticas de Python
 * Lenguaje orientado a objetos
    * Paradigma de programación que usa objetos y sus interacciones
    * Los objetos son entidades que combinan estado (atributo), comportamiento (método) e identidad
 * Biblioteca estándar muy amplia
    *  Contiene módulos (escritos en lenguaje C) que proporcionan acceso a las funcionalidades propias del sistema operativo

---

## Código fuente y bytcode

Python es un lenguaje interpretado. Sin embargo el intérprete genera archivos binarios que son los que se ejecutan.
Este proceso se realiza de manera transparente a partir de los archivos fuente (.py) y el código generado se conoce como _bytcode_ y utiliza la extensión .pyc

El programador no interviene en el proceso

El intérprete de Python lee el archivo fuente, genera el _bytcode_ y lo ejecuta, aumentando la velocidad y eficiencia en la ejecución

La causa de este proceso es que, una vez generado el archivo .pyc, Python no vuelve a leer el archivo fuente, salvo que este último haya cambiando

---

## Legibilidad del código

Normalmente, un código bien escrito no necesita comentarios, salvo para explicar:

* Suposiciones
* Decisiones y/o detalles importantes
* Problemas a resolver y/o superar

Los comentarios detallan el _por qué_ mientras que del código se desprende el _cómo_

Si resulta necesario comentar el código más allá de lo comentado, debería reescribirse de manera legible

Cuando se crea una función corresponde agregar cadenas de documentación (_docstrings_)

---

## Ejemplo


```{python}
x = 'hola mundo python'
print(x.split(' '))

```
---
