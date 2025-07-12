<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(:subTitulo="'1. Técnicas de recopilación de requisitos'")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.overflow-hidden

    .bg-color-4.mb-5(data-aos="fade-up")
      .row.justify-content-center.align-items-center
        .col-lg-auto.mb-3.mb-lg-0
          figure
            img(src='@/assets/curso/tema1/1.png', alt='')
        .col-lg
          .p-4
            p.mb-0(data-aos="fade-up") Cuando se enfrenta al desafío de construir un sistema de software, el primer paso que se debe dar es entender claramente lo que los usuarios necesitan. Esta tarea no es sencilla, pero existen diferentes técnicas de recopilación de requisitos que permiten obtener la información necesaria de manera organizada y confiable. A continuación, se deberá conocer cada técnica y aprender cuándo y cómo aplicarlas, utilizando ejemplos para que se visualice su utilidad (Gil Pascual, 2016).
    
    h2.mb-5(data-aos="fade-left") ¿Qué es la recopilación de requisitos?

    .row.mb-5
      .col-lg-5.order-lg-2.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema1/2.png", data-aos="zoom-in")
      .col-lg-7.order-lg-1
        .bg-color-5.h-100.py-5.px-5(data-aos="fade-left")
          p.mb-0 La recopilación de requisitos es el proceso mediante el cual se identifica, documenta y se comprenden las necesidades, expectativas y restricciones de los usuarios y otras partes interesadas, respecto al sistema que se va a desarrollar. Una buena recopilación de requisitos evita errores costosos, disminuye malentendidos y asegura que el software cumpla con su propósito (Gil Pascual, 2016).

    #t_1_1.titulo-segundo(data-aos="flip-up")
      h2 #[span 1.1] Entrevistas
    
    .bg-full-width.bg-color-3
      .p-4.p-md-5
        p Cuando se necesita comprender profundamente las necesidades, expectativas o problemas de un usuario o cliente, la entrevista se convierte en su mejor aliada (Genero Bocco et al., 2014). A través de las entrevistas, se tiene la oportunidad de hacer preguntas directas y adaptarlas en tiempo real, según las respuestas que se reciban.
        p.mb-5 Existen tres tipos de entrevistas que se pueden utilizar:

        div.row.justify-content-center.align-items-stretch
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema1/3.svg" alt="" style="width: 90px")
              h5.text-center Entrevistas estructuradas
              p.mb-0.text-center Son entrevistas donde todas las preguntas están previamente definidas. Son útiles cuando se desea obtener información específica y compararla entre diferentes usuarios (Genero Bocco et al., 2014).
        
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema1/4.svg" alt="" style="width: 90px")
              h5.text-center Entrevistas semiestructuradas 
              p.mb-0.text-center Mezclan preguntas planteadas con preguntas espontáneas basadas en las respuestas del usuario. Permiten descubrir detalles que no se habían anticipado.
        
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema1/5.svg" alt="" style="width: 90px")
              h5.text-center Entrevistas no estructuradas
              p.mb-0.text-center Son más conversacionales. Solo es tener algunos temas en mente y permitir que el flujo de la conversación guíe la obtención de requisitos (Gil Pascual, 2016).
    
    .bg-full-width.bg-color-6.mb-5
      .px-4.px-md-5
        .row.justify-content-center.align-items-center
          .col-lg-12
            .row.justify-content-center.align-items-center
              .col-lg-7(data-aos="fade-left").mb-3.mb-lg-0
                h5 Características de una buena entrevista:
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Preparar las preguntas con anticipación.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Crear un ambiente cómodo para el entrevistado.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Escuchar activamente.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Tomar notas o grabar (con permiso), para no perder información importante.
              .col-lg-5(data-aos="zoom-in")
                img.img-fluid(src='@/assets/curso/tema1/6.svg', style="max-width:486px", alt="" ).mx-auto.mx-lg-0.ms-lg-auto.mb-4.mb-lg-0
    
    .row.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema1/7.png", data-aos="zoom-in")
      .col-lg-8
        .bg-color-7.p-4.bordes(data-aos="fade-left")
          h5 Ejemplo:
          p Se está desarrollando una app de citas. En una entrevista semiestructurada a un usuario, preguntar: 
          p "¿Qué es lo más importante para usted al usar una app de citas?"
          p La respuesta puede abrir temas que no se habían considerado, como la importancia de filtros de privacidad o de intereses comunes.

    
        .bg-color-1.p-4(data-aos="fade-left")
          p.mb-0 <b>Tip importante</b>. No se enfoque solo en "qué" quiere el usuario, sino también en "por qué" lo quiere. Esa información es esencial para entender las verdaderas necesidades detrás de los requisitos.
    
    p.mb-5 Los pasos para implementar una entrevista, son:

    .bg-full-width.bg-fondo-1.mb-5
      .p-4.p-md-5
        .row.justify-content-center.align-items-center
          .col-lg-11
            ImagenInfografica.color-secundario
              template(v-slot:imagen)
                figure
                  img(src='@/assets/curso/tema1/8.svg', alt='', style="max-width: 1106px;").mx-auto
    
              .bg-color-white.box-shadow.p-3(x="23%" y="62.5%" numero="+")
                h5 Preparación de la entrevista
                h5 Definición de objetivos
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Establecer claramente qué información se necesita recolectar.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Asegurar que los objetivos de la entrevista se encuentren alineados con los requerimientos del proyecto.
                h5 Selección de participantes
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Elegir a los entrevistados claves que tienen experiencia o conocimientos relevantes para el proyecto.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Asegurar diversidad de perspectivas (usuarios, clientes, desarrolladores, etc.).
                h5 Diseño de las preguntas
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Formulación de preguntas claras, abiertas y específicas, que fomenten respuestas detalladas.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Considerar preguntas de tipo abierto (para obtener información rica) y cerradas (para obtener datos concretos).
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Agrupar preguntas por tema, para mantener el enfoque.
                h5 Planificación de la entrevista
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Definir la duración y el formato (presencial, virtual).
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Programar las entrevistas en horarios convenientes para los entrevistados.
    
              .bg-color-white.box-shadow.p-3(x="20.5%" y="41%" numero="+")
                h5 Consideraciones finales
                h5 Ética
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Respetar la confidencialidad y la privacidad de los entrevistados.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Solicitar el consentimiento informado, antes de la entrevista y para la grabación de la misma.
                h5 Mejora continua
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Evaluar el proceso de entrevista después de cada sesión para identificar posibles mejoras.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Ajustar las técnicas o el enfoque para futuras entrevistas.
    
              .bg-color-white.box-shadow.p-3(x="67%" y="15%" numero="+")
                h5 Análisis de la información recopilada
                h5 Organización y transcripción
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Organizar las notas y transcribir las grabaciones, para facilitar el análisis.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Agrupar la información en categorías temáticas (requisitos funcionales, necesidades del usuario, etc.).
                h5 Identificación de patrones y tendencias
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Buscar patrones comunes en las respuestas de los entrevistados.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Identificar posibles conflictos o diferentes enfoques entre los entrevistados.
                h5 Validación de los resultados
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Validar la información obtenida con los entrevistados para confirmar su precisión.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 En caso de dudas, realizar entrevistas de seguimiento o discusiones adicionales.
    
              .bg-color-white.box-shadow.p-3(x="76%" y="45%" numero="+")
                h5 Documentación y presentación de resultados
                h5 Resumen de los resultados
                p Evaluación y mejora de protocolos para garantizar la satisfacción y fidelización de los clientes.
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Elaborar un resumen claro y conciso de la información obtenida, destacando los puntos claves.
                h5 Presentación a las partes interesadas
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Preparar un informe o presentación para compartir con los interesados en el proyecto.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Asegurar que los resultados se presenten de manera comprensible para todos los involucrados.
    
              .bg-color-white.box-shadow.p-3(x="78%" y="74.5%" numero="+")
                h5 Conducción de la entrevista
                h5 Establecer un ambiente de confianza
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Crear un ambiente cómodo y respetuoso para que los entrevistados se sientan libres para compartir información.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Comenzar la entrevista con una breve introducción y aclarar el propósito de la misma.
                h5 Habilidades de escucha activa
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Prestar atención plena a lo que el entrevistado está diciendo.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Evitar interrupciones y hacer preguntas aclaratorias, cuando sea necesario.
                h5 Tomar notas o grabar la entrevista
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Tomar notas claras para capturar la información clave.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Si es posible, grabar la entrevista (con permiso), para una posterior transcripción y análisis.
                h5 Flexibilidad y adaptación
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Adaptar la entrevista, según el flujo de la conversación.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Estar preparado para explorar temas no anticipados, si surgen durante la conversación.

    #t_1_2.titulo-segundo(data-aos="flip-up")
      h2 #[span 1.2] Encuestas y cuestionarios
    
    p Cuando se necesita recopilar opiniones o necesidades de un grupo amplio de usuarios, en poco tiempo, las encuestas y cuestionarios son la mejor herramienta (Gil Pascual, 2016).
    p.mb-5 Se pueden diseñar:

    .row.justify-content-center.align-items-stretch.mb-4
      .col-lg-6.mb-3.mb-lg-0
        .bg-color-8.p-4(data-aos="fade-left").h-100
          .row.align-items-center
            .col-lg-auto
              img(src="@/assets/curso/tema1/9.svg", style="max-width: 90px").mx-auto
            .col-lg.text-white
              h5.mb-2 Preguntas cerradas
              p.mb-0 Con opciones de respuesta definidas (ideal para análisis estadístico).

      .col-lg-6.mb-3.mb-lg-0
        .bg-color-8.p-4(data-aos="fade-left").h-100
          .row.align-items-center
            .col-lg-auto
              img(src="@/assets/curso/tema1/9.svg", style="max-width: 90px").mx-auto
            .col-lg.text-white
              h5.mb-2 Preguntas abiertas
              p.mb-0 Donde el usuario responde libremente (útiles para captar nuevas ideas).

    .bg-full-width.bg-color-4.mb-5
      .px-4.px-md-5
        .row.justify-content-center.align-items-center
          .col-lg-12
            .row.justify-content-center.align-items-center
              .col-lg-7(data-aos="fade-left").mb-3.mb-lg-0
                h5 Características de una buena encuesta:
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Tiene preguntas claras, breves y no ambiguas.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Presenta un orden lógico (de lo general a lo específico).
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Limita el número de preguntas para no cansar al usuario.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Puede ser anónima, para fomentar respuestas más honestas.
              .col-lg-5(data-aos="zoom-in")
                img.img-fluid(src='@/assets/curso/tema1/10.svg', style="max-width:486px", alt="" ).mx-auto.mx-lg-0.ms-lg-auto.mb-4.mb-lg-0
    
    .bg-color-9(data-aos="fade-up")
      .row.justify-content-center.align-items-center
        .col-lg-auto.mb-3.mb-lg-0
          figure
            img(src='@/assets/curso/tema1/11.png', alt='')
        .col-lg
          .p-4
            h5.mb-0(data-aos="fade-up") Ejemplo:
            p Imagine que se debe crear una plataforma educativa en línea. Se ejecuta una encuesta que pregunta:
            p "¿Qué funcionalidades considera imprescindibles en una plataforma educativa?"
    
    .bg-color-10.p-4(data-aos="fade-left").h-100.mb-5
      p <b>Opciones</b>: foros de discusión, videollamadas, evaluaciones automáticas, recursos descargables.
      p En este caso, realizar una encuesta permite que se llegue a más personas rápidamente si es el objetivo del proceso. 
      p También se debe recordar que una encuesta o cuestionario se usa más para validar información, pero no se pueden obtener detalles profundos.
      p Las herramientas recomendadas son: Google Forms, SurveyMonkey, Typeform.

    #t_1_3.titulo-segundo(data-aos="flip-up")
      h2 #[span 1.3] Observación directa
    
    p.mb-5 La observación directa, permite ver cómo las personas trabajan realmente, en su ambiente natural, sin que medie la interpretación de sus palabras. Muchas veces, las personas hacen cosas que no son capaces de explicar o simplemente omiten detalles importantes, cuando se les pregunta (Fresno Chávez, 2018).

    .bg-full-width.bg-color-6.mb-5
      .px-4.px-md-5
        .row.justify-content-center.align-items-center
          .col-lg-12
            .row.justify-content-center.align-items-center
              .col-lg-7(data-aos="fade-left").mb-3.mb-lg-0.order-lg-2
                h5 Características de una buena observación:
                ul.lista-ul--color
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Se debe ser discreto para no alterar el comportamiento natural del usuario.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Anotar todo, comportamientos, dificultades, soluciones improvisadas.
                  li.mb-0.d-flex
                    i.far.fa-arrow-alt-circle-right
                    p.mb-0 Es posible realizar grabaciones (siempre solicitando permiso previo).
              .col-lg-5(data-aos="zoom-in").order-lg-1
                img.img-fluid(src='@/assets/curso/tema1/12.svg', style="max-width:486px", alt="" ).mx-auto.mx-lg-0.ms-lg-auto.mb-4.mb-lg-0

    .bg-full-width.bg-color-3.mb-5
      .px-4.px-md-5
        .row.mb-5
          .col-lg-3.order-lg-2.mb-3.mb-lg-0
            figure
              img(src="@/assets/curso/tema1/13.png", data-aos="zoom-in")
          .col-lg-9.order-lg-1
            h5 Ejemplo:
            p(data-aos="fade-left") Supongamos que se quiere mejorar el sistema de control de inventario de una tienda. Se debe ir al almacén y observar que los empleados registran productos, tanto en un software como en hojas de papel, generando duplicidad y errores. Esta información no se habría obtenido solo preguntándoles, porque muchas veces los usuarios normalizan sus malas prácticas.
        
            .bg-color-1.bordes.p-5(data-aos="fade-left")
              p.mb-0 <b>Importante</b>: la observación revela los "requisitos tácitos", aquellos que los usuarios no verbalizan, pero que son cruciales para el éxito del proyecto.

    #t_1_4.titulo-segundo(data-aos="flip-up")
      h2 #[span 1.4] Talleres de trabajo (workshops)
    
    p Un workshop es una técnica colaborativa donde se reúnen a todos los involucrados (usuarios finales, líderes de proyecto, stakeholders, etc.), para definir juntos, los requisitos (Fresno Chávez, 2018).
    p Aquí se fomenta la creatividad, la discusión y la construcción conjunta de soluciones.
    p.mb-5 Características de un workshop efectivo:

    .bg-full-width.bg-color-11.mb-5
      .px-4.px-md-5
        .row.justify-content-center.align-items-stretch.mb-5
          .col-lg-3.mb-4(data-aos="zoom-in-up")
            .custom-image-card-2.h-100
              img.custom-image-card__image(src="@/assets/curso/tema1/14.png" alt="")
              .custom-image-card__text.p-4
                p.mb-0 Planificar previamente, la agenda del taller.
          .col-lg-3.mb-4(data-aos="zoom-in-down")
            .custom-image-card-2.h-100
              img.custom-image-card__image(src="@/assets/curso/tema1/15.png" alt="")
              .custom-image-card__text.p-4
                p.mb-0 Definir objetivos claros para la sesión.
          .col-lg-3.mb-4(data-aos="zoom-in-down")
            .custom-image-card-2.h-100
              img.custom-image-card__image(src="@/assets/curso/tema1/16.png" alt="")
              .custom-image-card__text.p-4
                p.mb-0 Utilizar dinámicas o actividades para fomentar la participación.
          .col-lg-3.mb-4(data-aos="zoom-in-down")
            .custom-image-card-2.h-100
              img.custom-image-card__image(src="@/assets/curso/tema1/17.png" alt="")
              .custom-image-card__text.p-4
                p.mb-0 Nombrar un moderador que guíe la conversación y evite que se desvíe.

    .row.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema1/18.png", data-aos="zoom-in")
      .col-lg-8
        .bg-color-12.p-4.bordes-1(data-aos="fade-left")
          h5 Ejemplo:
          p Cuando se está trabajando en un sistema de gestión hospitalaria. Se realiza un taller donde participan doctores, enfermeras, personal administrativo y desarrolladores. Cada grupo aporta sus necesidades específicas, permitiendo construir una visión integral del sistema.
          p.mb-0 Las herramientas que se pueden usar en un workshop, son: pizarras físicas, post-its, mapas mentales, diagramas de flujo.
    
        .bg-color-4.p-4(data-aos="fade-left")
          p.mb-0 <b>Tip</b>. Siempre se deben documentar las conclusiones de los talleres y, si es posible, pedir a los participantes que validen o firmen un acta de acuerdos.

    #t_1_5.titulo-segundo(data-aos="flip-up")
      h2 #[span 1.5] Revisión de documentos existentes
    
    p Muchas veces no se tiene que partir de cero. Revisar documentos ya existentes, puede ahorrar mucho tiempo y evitar errores (Gil Pascual, 2016).
    p.mb-5 Qué tipo de documentos se deben revisar:

    .row.justify-content-center.align-items-stretch.mb-4
      .col-lg-3.mb-3.mb-lg-0
        .bg-color-8.p-4(data-aos="fade-left").h-100
          .row.align-items-center
            .col-lg-auto
              img(src="@/assets/curso/tema1/19.svg", style="max-width: 90px").mx-auto
            .col-lg.text-white
              p.mb-0.text-small Manuales de usuario, de sistemas actuales.
      .col-lg-3.mb-3.mb-lg-0
        .bg-color-8.p-4(data-aos="fade-left").h-100
          .row.align-items-center
            .col-lg-auto
              img(src="@/assets/curso/tema1/20.svg", style="max-width: 90px").mx-auto
            .col-lg.text-white
              p.mb-0.text-small Reportes de fallos, de versiones anteriores.
      .col-lg-3.mb-3.mb-lg-0
        .bg-color-8.p-4(data-aos="fade-left").h-100
          .row.align-items-center
            .col-lg-auto
              img(src="@/assets/curso/tema1/21.svg", style="max-width: 90px").mx-auto
            .col-lg.text-white
              p.mb-0.text-small Procedimientos internos de la empresa.
      .col-lg-3.mb-3.mb-lg-0
        .bg-color-8.p-4(data-aos="fade-left").h-100
          .row.align-items-center
            .col-lg-auto
              img(src="@/assets/curso/tema1/22.svg", style="max-width: 90px").mx-auto
            .col-lg.text-white
              p.mb-0.text-small Contratos, normativas legales, requisitos de certificaciones.

    .bg-color-9(data-aos="fade-up")
      .row.justify-content-center.align-items-center
        .col-lg-auto.mb-3.mb-lg-0.order-lg-2
          figure
            img(src='@/assets/curso/tema1/23.png', alt='')
        .col-lg.order-lg-1
          .p-4
            h5(data-aos="fade-up") Características de una buena revisión documental:
            ul.lista-ul--color
              li.mb-3.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 Identificar la fuente y asegurar su confiabilidad.
              li.mb-3.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 Analizar qué requisitos siguen vigentes y cuáles deben actualizarse.
              li.mb-3.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 Extraer datos relevantes, de manera organizada.
    
    .bg-color-10.p-4(data-aos="fade-left").h-100.mb-5
      h5 Ejemplo:
      p Si se debe diseñar una app bancaria, sería vital que se revisen los reglamentos de seguridad financiera del país, así como los manuales de procedimientos internos, que actualmente maneja el banco.
      p <b>Consejo</b>. No se debe limitar a leer los documentos: cuestione su vigencia y relevancia. La revisión documental siempre debe ser crítica.

    #t_1_5.titulo-segundo(data-aos="flip-up")
      h2 #[span 1.5] Brainstorming y Focus Groups
    
    p.mb-5 Ambas técnicas son muy útiles cuando se quieren generar nuevas ideas o identificar necesidades no evidentes (Gil Pascual, 2016).

    .bg-full-width.bg-fondo-slider.mb-5
      .p-4.p-md-5
        SlyderA(tipo="b").bg-white
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.mb-3.mb-lg-0
              figure
                img(src="@/assets/curso/tema1/24.png")
            .col-lg-7
              h5 Brainstorming (lluvia de ideas)
              ul.lista-ul--color
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Reúna a un grupo de personas y permita que propongan ideas libremente.
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 No hay críticas durante la generación de ideas (todas las propuestas son válidas en un principio).
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Después, filtramos y evaluamos las ideas.
    
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.mb-3.mb-lg-0
              figure
                img(src="@/assets/curso/tema1/25.png")
            .col-lg-7
              h5 Focus Groups
              ul.lista-ul--color
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Reúna a un pequeño grupo de usuarios representativos.
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Se debe guiar una discusión estructurada sobre las necesidades, problemas y expectativas.
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Tomar notas de percepciones comunes, diferencias de opinión y prioridades.

    .row.mb-5
      .col-lg-4.mb-3.mb-lg-0.order-lg-2
        figure
          img(src="@/assets/curso/tema1/26.png", data-aos="zoom-in")
      .col-lg-8.order-lg-1
        .bg-color-7.p-4.bordes(data-aos="fade-left")
          h5 Características de una sesión efectiva:
          ul.lista-ul--color
            li.mb-2.d-flex
              i.far.fa-arrow-alt-circle-right
              p.mb-0 Hay un facilitador imparcial que anima a todos a participar.
            li.mb-2.d-flex
              i.far.fa-arrow-alt-circle-right
              p.mb-0 Se registran todas las ideas y comentarios.
            li.mb-2.d-flex
              i.far.fa-arrow-alt-circle-right
              p.mb-0 Se analizan las sesiones para identificar patrones y tendencias.

    
        .bg-color-1.p-4(data-aos="fade-left")
          h5 Ejemplo:
          p.mb-0 Al desarrollar una app de fitness personalizada, realizar un focus group con personas de diferentes edades y estilos de vida. Descubra que, para los usuarios jóvenes, es clave la gamificación (recompensas y logros), mientras que los adultos mayores, priorizan la facilidad de uso y la accesibilidad.

    .bg-full-width.border-top.color-primario
      .p-4.p-md-5
        h2(data-aos="fade-left") MATERIAL COMPLEMENTARIO
        .row.material-complementario
          .col-12.col-md-6.col-lg-7
            p Los invitamos a explorar el material complementario de este curso, en esta sección encontrará recursos que le permitirán profundizar  y enriquecer su aprendizaje en los temas tratados en esta unidad.

            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://elibro.net/es/ereader/tecnologicadeloriente/113783" target="_blank" rel="noopener noreferrer") Manovich, L. (2014) El software toma el mando. Editorial UOC. 


            p.d-flex.my-4
              img.me-3(src='@/assets/template/icono-yt.svg' :style="{'max-width':'16px'}")
              a(href="https://www.youtube.com/watch?v=VI5D1I90IhQ" target="_blank" rel="noopener noreferrer") Arcaya, M. (2020, 24 de julio). Técnicas de recolección de datos para el análisis y diseño de un sistema de información. [Vídeo] YouTube. 



          .col-12.col-md-6.col-lg-3.offset-lg-1
            figure
              img(src='@/assets/componentes/material-complementario.svg', alt='')

</template>

<script>
export default {
  name: 'Tema1',
  data: () => ({}),

  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
}
</script>

<style lang="sass"></style>
