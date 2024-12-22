---
title: "Usando Quarto Live para tutoriales interactivos"
subtitle: "Regular talk"
excerpt: ""
date: 2022-10-14
date_end: "2022-10-14"
author: "Yanina Bellini Saibene"
location: "Online (Latinoamérica)"
event: "LatinR 2024| Conferencia Latinoamericana sobre Uso de R en Investigación + Desarrollo"
event_url: https://latinr.org/
draft: false
# layout options: single, single-sidebar
layout: single
categories:
- Talk
- R
- Español
- Community
- Education
links:
- icon: book
  icon_pack: fas
  name: Slides
  url: https://docs.google.com/presentation/d/1mycE6LacXfIPl_1GxWF8CZhwizUhiCFxJ7NU58grwpw/edit?usp=sharing
- icon: youtube
  icon_pack: fab
  name: video 
  url: https://youtu.be/xRA4QD_U0Z4
---




Palabras clave:  educación, ejercicios programación, R, Python

## Abstract
Quarto Live es una extensión para Quarto que permite ejecutar código de R y Python 
de forma interactiva en un documento web mediante WebAssembly. 
Esta extensión se presenta como la evolución del paquete {learnr} para generar 
tutoriales y documentación interactiva, con la ventaja que se pueden publicar 
los documentos generados en servicios web estáticos como Netlify o GitHub Pages.  
En esta charla presentaremos la experiencia de traducir tutoriales de learnr a 
Quarto Live y de generar tutoriales desde cero, incluyendo como publicarlos.

### Quarto Live 

La extensión proporciona:

* Bloques de código R y Python interactivos, con tematización automática, resaltado de sintaxis y autocompletado.

* Ejercicios con tips opcionales, soluciones y algoritmos de calificación personalizados.

* Posibilidad de mostrar gráficos interactivos del lado del cliente, imágenes y widgets HTML.

### R-Universe

R-universe permite a los usuarios y desarrolladores de paquetes R publicar, descubrir, 
aprender y desarrollar paquetes de R.  Ofrece las versiones WebAssembly de los paquetes 
que están en R-Universe.  Estas versiones son necesarias para poder usarlas con Quarto Live. 
R-Universe tiene todos los paquetes presentes en CRAN y Bioconductor, 
lo que asegura poder contar con la versión de WebAssembly de casi cualquier paquete que necesitemos.

### Tutoriales

Utilizando estas dos herramientas traducimos una serie de tutoriales de learnr a 
Quarto Live sobre temas de visualización y análisis de texto con R. 
También generamos una serie de tutoriales nuevos para enseñar a programar con R 
desde cero que complementan el material de la serie Aprendiendo a Programar en 
30 lecciones desarrollada para darle clases a adolescentes y utilizada también 
para formar periodistas con cambios en el conjunto de datos utilizado. 
Algunos de estos tutoriales también se utilizaron en la materia Programación II 
de una carrera de grado de Licenciatura en Ciencia de Datos. 

### Lecciones aprendidas

Quarto Live todavía no presenta todas las funcionalidades que presenta el paquete learnr, 
como por ejemplo, ejercicios con preguntas de opción múltiple. 
Anque mostraremos alternativas para generar este tipo de pregunta con una solucion “casera” 
y otros paquetes.

Tampoco tiene una opcion en castellano de las cajas de código y otros elementos. 
Aunque sí permite una integración con el paquete gradethis para proveer feedback 
automático a los estudiantes durante el tutorial. 
También permite una integración más natural con diapositivas de clase.

Tambien esta faltando la funcionalidad de grabar las respuestas de 
los estudiantes para enviarlas y poder corregirlas.  
En learnr se puede realizar utilizando otros paquetes como   

Las ventajas más grandes de Quarto Live son:

* Se puede publicar sin necesidad de crear un paquete e instalarlo o la necesidad de contar con un servidor Shiny.

* Se puede usar también con Python, no solo con R. 

Al igual que con los tutoriales de learnr, nuestra experiencia es que 
los estudiantes valoran este tipo de material como repaso de contenidos vistos en clase. 

El desarrollo de Quarto y WebR es muy activo, por lo que pensar en migrar los tutoriales 
de learnr a esta plataforma es una buena idea, como también generar tus nuevos tutoriales 
utilizando directamente esta nueva extensión de Quarto. 
