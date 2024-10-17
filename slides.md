---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://images.pexels.com/photos/577585/pexels-photo-577585.jpeg
# some information about your slides (markdown enabled)
title: Tema 1. Entornos de desarrollo
info:
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# take snapshot for each slide in the overview
overviewSnapshots: true
---

# Tema 1. Entornos de desarrollo

### Trabajo realizado por:

Elena Expósito Lara

Alberto Nieto Lozano

Gregorio Ruiz López

Antonio Rodríguez Cortés

Daniel Santaflorentina Picchi

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Click para ir al índice<carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/ElenaExposito/Slidev-Tema1" target="_blank" alt="GitHub" title="Open in GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

## Índice

<br>
<br>

1. Software y programa. Tipos de Software
2. Relación hardware-software
3. Desarrollo de software
4. Lenguajes de programación
5. Fases o etapas en el desarrollo y ejecución del software

---
class: px-20
---

## 1. Software y programa. Tipos de Software

<br>
El software es el conjunto de programas informáticos que actúan sobre el hardware para ejecutar lo que el usuario quiera.

<div grid="~ cols-2 gap-2" m="t-2">

- <span v-mark="{ at: 1, color: 'red', type: 'underline' }">Sistema Operativo</span>: Tiene que estar instalado y configurado en el equipo para que las aplicaciones funcionen.
- <span v-mark="{ at: 2, color: 'red', type: 'underline' }">Software de programación</span>: Conjunto de herramientas que permiten desarrollar programas informáticos.
- <span v-mark="{ at: 3, color: 'red', type: 'underline' }">Aplicaciones Informáticas</span>: Conjunto de programas con diferentes finalidades.

<div class="flex flex-col items-center">
  <img class="w-full h-auto rounded mb-4 max-w-[200px]" src="https://ibiscomputer.com/wp-content/uploads/2019/01/sistemas-operativos-1.png" alt="Imagen de sistemas operativos">
  <img class="w-full h-auto rounded max-w-[200px]" src="https://img.freepik.com/vector-premium/fondo-plano-redes-sociales-ordenador_23-2147819105.jpg" alt="Imagen de redes sociales en un ordenador">
</div>
</div>

---

## 2. Relación Hardware-Software

<br>
Esta relación se puede manifestar de dos puntos de vista:

<div class="flex flex-col gap-6">
<br>
<div>
- <span v-mark="{ at: 1, color: 'orange', type: 'underline' }">PV. Sistema Operativo</span>: El S.O. se encarga de coordinar el hardware actuando como intermediario con las aplicaciones que estén funcionando.
</div>
<div>
- <span v-mark="{ at: 2, color: 'orange', type: 'underline' }">PV. Aplicaciones</span>: Una aplicación es un conjunto de programas que están escritos en un lenguaje que el hardware del equipo interpreta y ejecuta. Los lenguajes de programación usan sentencias legibles para el humano, pero el equipo solo puede leer 0 y 1, por lo que tiene que ocurrir una traducción para que el ordenador ejecute lo que esté escrito en el lenguaje de programación.
</div>
</div>

---

## 3. Desarrollo de Software

Es el proceso que ocurre desde que se concibe una <span v-mark="{ at: 1, color: 'orange', type: 'circle' }">idea</span> hasta que un programa está implementado en el ordenador y funcionando.

<br>

<div class="flex justify-center">
<img class="w-full h-auto rounded max-w-[400px]" src="https://www.solusoft.es/Info/Imagenes/desarrollo-de-software/img_hero.svg" alt="">
</div>

---

### 3.1. Ciclos de Vida de Software

<br>
<ul class="flex flex-col gap-4">

<li> <span v-mark="{ at: 1, color: 'red', type: 'underline' }">Modelo en Cascada</span>: Sin retorno entre etapas, requiere conocer todos los requisitos.</li>
<li> <span v-mark="{ at: 2, color: 'red', type: 'underline' }">Cascada con Realimentación</span>: Permite retroceder y corregir; ideal para proyectos con requisitos claros.</li>
<li> <span v-mark="{ at: 3, color: 'red', type: 'underline' }">Modelos Evolutivos</span>:
<ul class="flex flex-col gap-3 py-1">
    <li> <span v-mark="{ at: 4, color: 'orange', type: 'underline' }">Iterativo Incremental</span>: Fases se repiten y mejoran en cada ciclo.</li>
    <li> <span v-mark="{ at: 5, color: 'orange', type: 'underline' }">Modelo en Espiral</span>: Construcción en versiones mejoradas, incremento de funcionalidad.</li>
  </ul>
</li>
<Arrow x1="0" y1="300" x2="75" y2="250" color="orange" />
<Arrow x1="0" y1="300" x2="75" y2="290" color="orange"/>
</ul>

---

### 3.1. Herramientas de Apoyo al Desarrollo del Software

<br>
<div class="flex">
  <div class="flex flex-col gap-6">
    <ul class="flex flex-col gap-2"> Herramientas CASE para automatizar tareas y aumentar la productividad.
      <li>
        <ul>Desarrollo Rápido de Aplicaciones (RAD):
          <li>Desarrollo iterativo, prototipos y uso de CASE.</li>
        </ul>
      </li>
      <li>Beneficios: mejora en la planificación, agilidad, reutilización, estándares, y visualización gráfica de fases.</li>
    </ul>
    <ul class="flex flex-col gap-1"> Clasificación de herramientas CASE:
      <li>U-CASE: Planificación y análisis de requisitos.</li>
      <li>M-CASE: Análisis y diseño.</li>
      <li>L-CASE: Programación, pruebas y documentación.</li>
    </ul>
    <p>Ejemplos: ArgoUML, Use Case Maker, ObjectBuilder.</p>
  </div>
    <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/zfPntfZ/5herramientas-al-desarrollo-de-software.png" alt="">
</div>

---

### 4. Lenguajes de programación

<br>
<div class="flex gap-8">
  <div class="flex flex-col gap-5">
    <ul>Idioma artificial para que el hardware entienda y ejecute tareas.</ul>
    <ul class="flex flex-col gap-2">Tipos de Lenguajes:
      <li>Lenguaje Máquina</li>
      <li>Lenguaje Ensamblador</li>
      <li>Lenguajes de Alto Nivel</li>
      <li>Lenguajes Visuales</li>
    </ul>
  </div>
  <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/cCCrZLb/6-Lenguajes-de-programacion.png" alt="">
</div>

---

### 4.1. Concepto y Clasificación de los Lenguajes de Programación

<br>
<div class="flex flex-col gap-2 items-center">
<p>La elección del lenguaje de programación depende de las características del problema.</p>
<p>Clasificación de lenguajes según:</p>
<div class="flex content-start gap-2">
  <ul class="flex flex-col gap-1">Proximidad al lenguaje humano:
    <li>Alto nivel (más cercano al razonamiento humano).</li>
    <li>Bajo nivel (más cercano al funcionamiento interno de la computadora: Ensamblador, Máquina).</li>
  </ul>
  <ul>Técnica de programación:
    <li>Estructurados (ej. Pascal, C).</li>
    <li>Orientados a objetos (ej. C++, Java).</li>
    <li>Visuales (ej. Visual Basic.Net).</li>
  </ul>
</div>
</div>

---

### 4.2. Lenguajes de Programación Estructurados

<br>
<div class="flex gap-2 items-center">
  <div class="flex flex-col">
    <p>Definición de programación estructurada y tipos de sentencias: secuenciales, selectivas y repetitivas.</p>
    <p><span v-mark="{ at: 1, color: 'green', type: 'underline' }">Ventajas</span>: Lectura y mantenimiento sencillo, estructura clara.</p>
    <p><span v-mark="{ at: 2, color: 'red', type: 'underline' }">Inconvenientes</span>: Dificultad en manejar programas grandes, falta de reutilización eficaz de código.</p>
  </div>
  <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/CMdZgcr/10lenguaje-programacion-estructurado.png" alt="">
</div>

---

### 4.3. Lenguajes de Programación Orientados a Objetos

<br>
<div class="flex gap-2 items-center">
  <div class="flex flex-col">
    <p>Enfoque basado en objetos que colaboran para realizar acciones. Reutilizables para futuros proyectos.</p>
    <p><span v-mark="{ at: 1, color: 'green', type: 'underline' }">Ventajas</span>: Reutilización del código y facilidad para depuración.</p>
    <ul><span v-mark="{ at: 2, color: 'orange', type: 'underline' }">Características</span>:
      <li>Atributos y clases.</li>
      <li>Comunicación entre objetos mediante métodos.</li>
    </ul>
  </div>
  <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/gZJQGxF/11leng-orientado-a-objetos.png" alt="">
</div>

---

## 5. Fases en el Desarrollo de Software

<br>
<br>
<div class="flex ">
  <ol class="flex flex-col gap-3">
    <li>Análisis de requisitos: Funcionales y no funcionales.</li>
    <li>Diseño: Modelo funcional-estructural, selección de lenguajes y SGBD.</li>
    <li>Codificación</li>
    <li>Pruebas</li>
    <li>Documentación</li>
    <li>Explotación</li>
    <li>Mantenimiento</li>
  </ol>
 <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/kyKcc66/12fases-desarrollo-de-software.png" alt="">
</div>

---

### 5.1. Análisis de Requisitos

<br>
<div class="flex gap-2 items-center">
  <div>
    <p>Es la base del desarrollo del proyecto.</p>
    <ul class="flex flex-col gap-4">
      <li><span v-mark="{ at: 1, color: 'green', type: 'underline' }">Requisitos Funcionales</span>: 
        <ul>
          <li>Funciones, respuesta ante entradas, comportamiento en situaciones inesperadas</li>
        </ul>
      </li>
      <li><span v-mark="{ at: 2, color: 'red', type: 'underline' }">Requisitos No Funcionales</span>:
          <ul>
          <li>Tiempos de respuesta, legislación, manejo de simultaneidad</li>
          </ul>
      </li>
      <li>Comunicación clave entre analista y cliente</li>
      <li>Documento ERS (Especificación de Requisitos Software)</li>
    </ul>
  </div>
  <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/J2F1ycz/13analisis-requisitos.png" alt="">
</div>

---

### 5.2. Diseño del Software

<br>
<div class="flex">
  <ul class="flex flex-col self-center gap-4">
    <li>Creación del modelo funcional-estructural y división en partes.</li>
    <li>Decisiones importantes: entidades y relaciones de bases de datos, selección de lenguajes y SGBD.</li>
  </ul>
  <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/WKKz8Lm/14dise-osoftware.png" alt="">
</div>

---

### 5.3. Codificación. Tipos de código

<br>
<div>
<p>La codificación es convertir ideas o soluciones en instrucciones usando un lenguaje de programación, creando el código fuente que el ordenador lo ejecute.</p>
<div class="flex">
<div class="grid grid-cols-2 gap-1 p-3 border border-gray-300 rounded-lg text-center">
  <!-- Encabezados -->
  <div class="font-semibold bg-orange  rounded">Características deseables de todo código</div>
  <div class="font-semibold bg-orange  rounded">Estados del código</div>

  <!-- Fila 1 -->
  <div class=" border-b border-gray-300">Modularidad: dividirlo en trozos pequeños</div>
  <div class=" border-b border-gray-300">Código fuente</div>

  <!-- Fila 2 -->
  <div class=" border-b border-gray-300">Corrección: que cumpla lo que se le solicita</div>
  <div class=" border-b border-gray-300">Código objeto</div>

  <!-- Fila 3 -->
  <div class=" border-b border-gray-300">Fácil de leer: facilitar el desarrollo y mantenimiento futuros</div>
  <div class=" border-b border-gray-300">Código ejecutable</div>

  <!-- Fila 4 -->
  <div class=" border-b border-gray-300">Eficiencia: un buen uso de los recursos</div>
  <div class=" border-b border-gray-300"></div>

  <!-- Fila 5 -->
  <div class="">Portabilidad: implementación en cualquier equipo</div>
  <div></div>
</div>

<img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/BNyW1BG/1image-removebg-preview-5.png" alt="">
</div>
</div>

---

### 5.4. Fases en la obtención de código

<br>
<img class="w-full h-auto rounded max-w-[800px] flex self-center" src="https://i.ibb.co/fkr6Lmg/14-Fasesobtencioncodigo.png" alt="">

---

### 5.5. Máquinas virtuales

<br>
<div class="flex flex-col gap-4">
  <p>Es la ejecución de un ordenador completamente con el software en lugar de un hardware físico.</p>
  <ul class="flex flex-col gap-3">Características:
    <li><span v-mark="{ at: 1, color: 'orange', type: 'underline' }">Portabilidad</span>: Permiten que las aplicaciones se puedan ejecutar en diferentes sistemas.</li>
    <li><span v-mark="{ at: 2, color: 'orange', type: 'underline' }">Gestión de Memoria</span>: Asigna memoria para los objetos creados y liberan la memoria no utilizada.</li>
    <li><span v-mark="{ at: 3, color: 'orange', type: 'underline' }">Interacción con el Sistema Huésped</span>: Facilitan la comunicación con el sistema operativo para controlar los dispositivos de hardware.</li>
    <li><span v-mark="{ at: 4, color: 'orange', type: 'underline' }">Seguridad</span>: Garantizan que las aplicaciones cumplan con las normativas de seguridad.</li>
  </ul>
</div>

---

### 5.5.1. Frameworks

<br>
<br>
<div class="flex gap-2 items-center">
  <div class="flex flex-col gap-1">
    <p>Se trata de una plataforma software donde están definidos programas soporte, bibliotecas, lenguaje interpretado, etc., que ayuda a desarrollar y unir los diferentes módulos o partes de un proyecto.</p>
    <p><span v-mark="{ at: 1, color: 'green', type: 'underline' }">Ventajas</span>: desarrollo rápido, reutilización del código, diseño uniforme y portabilidad de aplicaciones.</p>
    <p><span v-mark="{ at: 2, color: 'red', type: 'underline' }">Desventajas</span>: dependencia del código y su instalación consume bastantes recursos.</p>
  </div>
  <img class="w-full h-auto rounded max-w-[300px] flex self-center" src="https://i.ibb.co/VShYtm7/18png-clipart-laravel-black-logo-tech-companies-thumbnail.webp" alt="">
</div>

---

### 5.5.2. Entornos de ejecución

<br>
<div class="flex">
<div class="flex flex-col gap-2">
  <p>Servicio de máquina virtual que sirve como base para la ejecución de programas.</p>
  <p>Está formado por la máquina virtual y la API.</p>
  <p>Funciona como intermediario entre el lenguaje fuente y el sistema operativo, y consigue ejecutar aplicaciones.</p>
</div>
<div class="flex flex-col gap-5">
  <img class="w-full h-auto rounded max-w-[400px] flex self-center" src="https://i.ibb.co/tbmWWtf/19maxresdefault.webp" alt="">
  <img class="w-full h-auto rounded max-w-[400px] flex self-center" src="https://i.ibb.co/q7YTXPr/1698242399109.png" alt="">
</div>
</div>

---

### 5.6. Pruebas

<br>
<div class="flex">
  <ul class="flex flex-col gap-5">En el desarrollo de software, se realizan tres tipos principales de pruebas:
    <li><span v-mark="{ at: 1, color: 'orange', type: 'underline' }">Pruebas unitarias</span>: Se prueban individualmente las diferentes partes del software para verificar su funcionamiento de manera aislada.</li>
    <li><span v-mark="{ at: 2, color: 'orange', type: 'underline' }">Pruebas de integración</span>: Tras superar las pruebas unitarias, se verifica cómo funcionan todas las partes del sistema juntas e interrelacionadas.</li>
    <li><span v-mark="{ at: 3, color: 'orange', type: 'underline' }">Beta Test</span>: Es la prueba final, realizada en el entorno real del cliente, bajo condiciones normales de uso, para asegurar que el software funcione correctamente en producción.</li>
  </ul>
<div class="flex flex-col gap-5">
  <img class="w-full h-auto rounded max-w-[600px] flex self-center" src="https://i.ibb.co/gVcw3q2/20-Integration-testing-e77bcac7ff.webp" alt="">
  <img class="w-full h-auto rounded max-w-[600px] flex self-center" src="https://i.ibb.co/MVDt9jN/20joven-empresario-que-usa-la-tableta-digital-mientras-trabaja-en-la-oficina-de-negocios.webp" alt="">
</div>
</div>

---

### 5.7. Documentación

<br>
<p>En el desarrollo de software, es crucial documentar todas las etapas para informar a los usuarios y facilitar futuras revisiones del proyecto. Los tres documentos principales son:</p>

<br>
<div class="flex justify-around">
  <ol class="flex flex-col gap-2">
    <li>Guía técnica</li>
    <li>Guía de uso</li>
    <li>Guía de instalación</li>
  </ol>
<img class="w-full h-auto rounded max-w-[400px]" src="https://i.ibb.co/kcqQRPH/Trello-Emblema-1300x867.png" alt="">
</div>

---

### 5.8. Explotación

<br>
<br>
<ul class="flex flex-col gap-5">Es la fase en la que los usuarios finales conocen y comienzan a utilizar la aplicación. Se compone de:
  <li><span v-mark="{ at: 1, color: 'orange', type: 'underline' }">Instalación</span>: Proceso de instalar la aplicación en el equipo del cliente</li>
  <li><span v-mark="{ at: 2, color: 'orange', type: 'underline' }">Puesta a puntos</span>: Configuración necesaria para que la aplicación funcione correctamente.</li>
  <li><span v-mark="{ at: 3, color: 'orange', type: 'underline' }">Funcionamiento</span>: La aplicación en uso en el entorno del cliente.</li>
</ul>

---

### 5.9. Mantenimiento

<br>
<div class="flex">
  <div class="flex flex-col gap-4">
    <p>Proceso de control, mejora y optimización del software.</p>
    <ul class="flex flex-col gap-4">Tipos de Cambios:
      <li><span v-mark="{ at: 1, color: 'orange', type: 'underline' }">Perfectivos</span>: Mejoran la funcionalidad del software.</li>
      <li><span v-mark="{ at: 2, color: 'orange', type: 'underline' }">Evolutivos</span>: Responden a nuevas necesidades del cliente.</li>
      <li><span v-mark="{ at: 3, color: 'orange', type: 'underline' }">Adaptativos</span>: Ajustes y actualizaciones.</li>
      <li><span v-mark="{ at: 4, color: 'orange', type: 'underline' }">Correctivos</span>: Solucionar errores.</li>
    </ul>
  </div>
  <img class="w-full h-auto rounded max-w-[400px]" src="https://i.ibb.co/6WgKFBL/Padre-imagen-mantenimiento-3.png" alt="">
</div>

---

<div class="flex flex-col gap-8 items-center">
  <h1>¡Gracias por la atención!</h1>
  <div class="flex flex-col gap-1 items-center">
  <h2>Trabajo realizado por:</h2>
    <p>Elena Expósito Lara</p>
    <p>Alberto Nieto Lozano</p>
    <p>Gregorio Ruiz López</p>
    <p>Antonio Rodríguez Cortés</p>
    <p>Daniel Santaflorentina Picchi</p>
  </div>
</div>
