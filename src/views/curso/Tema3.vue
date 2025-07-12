<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(:subTitulo="'3. Herramientas de análisis'")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.overflow-hidden

    .bg-color-2.mb-5(data-aos="fade-up")
      .row.justify-content-center.align-items-center
        .col-lg-auto.mb-3.mb-lg-0
          figure
            img(src='@/assets/curso/tema3/1.png', alt='')
        .col-lg
          .p-4
            p.mb-0.text-white(data-aos="fade-up") Las herramientas de análisis son fundamentales en el ciclo de vida del desarrollo de <em>Software</em>, porque facilitan la organización, documentación y comunicación de los requisitos del sistema. Estas herramientas permiten, que tanto los usuarios como los desarrolladores, compartan una visión común del producto que se desea crear. El uso adecuado de herramientas de análisis permite obtener resultados más precisos, evitando errores costosos y mejorando la calidad final del sistema (Genero Bocco et al., 2014).
    
    .bg-full-width.bg-color-13
      .p-4.p-md-5
        p.mb-5 En el contexto de la ingeniería de <em>Software</em>, existen diversas herramientas que se utilizan en la fase de análisis de requisitos, y en este tema se abordarán tres de las más importantes:

        .row.justify-content-center.align-items-stretch
          .col-lg-4.mb-4(data-aos="zoom-in-up")
            .custom-image-card-2.h-100
              img.custom-image-card__image(src="@/assets/curso/tema3/2.png" alt="")
              .custom-image-card__text.p-4
                p.mb-0 Diagramas de casos de uso.
          .col-lg-4.mb-4(data-aos="zoom-in-down")
            .custom-image-card-2.h-100
              img.custom-image-card__image(src="@/assets/curso/tema3/3.png" alt="")
              .custom-image-card__text.p-4
                p.mb-0 Historias de usuario.
          .col-lg-4.mb-4(data-aos="zoom-in-down")
            .custom-image-card-2.h-100
              img.custom-image-card__image(src="@/assets/curso/tema3/4.png" alt="")
              .custom-image-card__text.p-4
                p.mb-0 Matrices de trazabilidad de requisitos.
    
    .bg-full-width.bg-color-10.mb-5
      .px-4.px-md-5.py-4
        .row.align-items-center
          .col-lg-auto
            img(src="@/assets/curso/tema3/5.svg", style="max-width: 90px").mx-auto
          .col-lg
            p.mb-0 Cada una de estas herramientas juega un papel crucial en garantizar que el <em>Software</em> se construya de acuerdo con los requerimientos definidos y que, además, se puedan realizar cambios de manera controlada.

    #t_3_1.titulo-segundo(data-aos="flip-up")
      h2 #[span 3.1] Diagramas de casos de uso
    
    .row.mb-5
      .col-lg-5.order-lg-2.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema3/6.png", data-aos="zoom-in")
      .col-lg-7.order-lg-1
        p.mb-5(data-aos="fade-left") Los diagramas de casos de uso son una de las herramientas más representativas en el análisis de requisitos, especialmente cuando se trabaja en sistemas orientados a usuarios (Zapata Jaramillo, 2006).
    
        .bg-color-4.p-4(data-aos="fade-left")
          p.mb-0 El propósito de estos diagramas es representar las interacciones entre los actores (usuarios o sistemas externos) y el sistema que se está desarrollando, destacando las funcionalidades o casos de uso que el sistema debe cumplir.
    
    .row.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema3/7.png", data-aos="zoom-in")
      .col-lg-8
        h2(data-aos="fade-left") ¿Por qué usar diagramas de casos de uso?
        p Los diagramas de casos de uso permiten obtener una vista general del sistema desde el punto de vista del usuario.
    
        .bg-color-1.p-4.mb-3(data-aos="fade-left")
          .row.align-items-start
            .col-lg-auto
              img(src="@/assets/curso/tema3/8.svg", style="max-width: 90px").mx-auto
            .col-lg
              p.mb-0 Son útiles en las primeras fases del proyecto para clarificar las necesidades del cliente, debido a que permiten visualizar de manera sencilla y clara, qué hace el sistema, quién lo usa y cómo se interactúa con él.
        p Los elementos de un diagrama de casos de uso, son:
    

    .bg-full-width.bg-fondo-slider.mb-5
      .p-4.p-md-5
        SlyderA(tipo="b").bg-white
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/9.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Actores
              p Los actores son aquellos que interactúan con el sistema. Pueden ser personas, sistemas u otras entidades externas que se comunican con el sistema en desarrollo. Los actores pueden ser primarios (como un usuario o administrador) o secundarios (como un sistema de pago).
    
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/10.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Casos de uso
              p Son las funcionalidades o servicios que el sistema proporciona. Se representan mediante un óvalo dentro del diagrama y describen el comportamiento esperado del sistema, en respuesta a una solicitud del actor.
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/11.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Relaciones
              p Las relaciones entre actores y casos de uso, se representan con líneas, indicando las interacciones. Además, existen relaciones entre los casos de uso, como la inclusión o extensión de casos de uso, lo que permite definir flujos alternativos o escenarios especiales.

    .bg-color-6.p-4.mb-3.bordes-2(data-aos="fade-left")
      h5 Ejemplo práctico
      p.mb-0 Imaginemos que estamos desarrollando un sistema para una tienda en línea. Los actores principales serían el cliente y el administrador. Los casos de uso principales podrían incluir registrar una cuenta, iniciar sesión, buscar productos y realizar un pedido.
    
    p.mb-5 Diagrama de casos de uso, para una tienda en línea:

    .titulo-figura.mb-4
      h5 Figura 1.
      span Ejemplo de caso de uso
    .row.justify-content-center.align-items-center.mb-5
      .col-lg-7.mb-3.mb-lg-0
        .bg-color-9.p-5
          figure
            img(src="@/assets/curso/tema3/12.svg", data-aos="zoom-in")
      .col-lg-5
        .bg-color-5.p-4(data-aos="fade-left")
          h5 Descripción del diagrama:
          ul.lista-ul--color
            li.mb-0.d-flex
              i.far.fa-arrow-alt-circle-right
              p.mb-0 El cliente puede realizar varias acciones, como registrarse, buscar productos o realizar pedidos.
            li.mb-0.d-flex
              i.far.fa-arrow-alt-circle-right
              p.mb-0 El administrador puede gestionar el inventario de productos, ver estadísticas de ventas y administrar pedidos.
          p Este diagrama ayuda a identificar rápidamente, las principales funcionalidades que el sistema debe proporcionar y cómo los usuarios interactúan con él.
        figure
          img(src="@/assets/curso/tema3/13.png", data-aos="zoom-in")

    #t_3_2.titulo-segundo(data-aos="flip-up")
      h2 #[span 3.2] Historias de usuario
    
    p.mb-5 Las historias de usuario son una herramienta clave en el desarrollo ágil de <em>Software</em>, ya que permiten capturar y comunicar de manera clara las necesidades reales de los usuarios desde su propia perspectiva.

    .bg-full-width.bg-color-8.mb-5
      .px-4.p-md-5
        .row.justify-content-center.align-items-center
          .col-lg-8.order-2.text-white
            h2.mb-4(data-aos="flip-up") Historias de usuario
            p.mb-4(data-aos="fade-right") En el PDF <b>Historias de usuario</b>, se abordan los elementos fundamentales que las componen, sus características, beneficios, tipos y herramientas asociadas, con el fin de facilitar su uso en proyectos colaborativos. Este enfoque centrado en el usuario promueve una comprensión compartida entre los equipos y garantiza el desarrollo de soluciones útiles, priorizadas y alineadas con el valor que se espera entregar.
    
            a.anexo.mb-4.bg-white.w-fit(:href="obtenerLink('/downloads/Anexo_1.pdf')" target="_blank")(data-aos="flip-up")
              .anexo__icono(:style="{'background-color': '#FCDFDB'}")
                img(src="@/assets/template/icono-pdf.svg")
              .anexo__texto
                p <strong>Anexo. </strong> Historias de usuario.
    
          .col-lg-4.order-1.mb-3.mb-lg-0
            figure(data-aos="zoom-in")
              img(src='@/assets/curso/tema3/14.png', alt='')

    #t_3_3.titulo-segundo(data-aos="flip-up")
      h2 #[span 3.3] Matriz de trazabilidad de requisitos
    
    .row.mb-5
      .col-lg-4.order-lg-2.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema3/15.png", data-aos="zoom-in")
      .col-lg-8.order-lg-1
        .bg-color-4.p-4(data-aos="fade-left")
          .row.align-items-start
            .col-lg-auto
              img(src="@/assets/curso/tema3/16.svg", style="max-width: 90px").mx-auto
            .col-lg
              p.mb-0 La matriz de trazabilidad de requisitos, es una herramienta fundamental en la gestión de proyectos de desarrollo de <em>Software</em>, especialmente cuando se busca asegurar que todos los requisitos del proyecto se han cumplido adecuadamente y se han implementado de acuerdo con lo solicitado. Su principal función es conectar los requisitos del sistema con los entregables y las pruebas realizadas, lo que permite verificar que todos los aspectos del proyecto han sido cubiertos (Genero Bocco et al., 2014).
    
    .row.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema3/17.png", data-aos="zoom-in")
      .col-lg-8
        h2(data-aos="fade-left") ¿Qué es una matriz de trazabilidad de requisitos?
        p.mb-5 Una matriz de trazabilidad de requisitos es un documento o herramienta que ayuda a mapear y vincular los requisitos con los elementos de diseño, las implementaciones y las pruebas correspondientes en el proceso de desarrollo del <em>Software</em>. El objetivo es asegurar que cada requisito tenga una correspondencia directa con las actividades de desarrollo y validación, que se deben realizar.
    
        .bg-color-1.p-4(data-aos="fade-left")
          p.mb-0 Esta matriz generalmente se presenta en forma de una tabla, en la que se listan los requisitos a un lado y se relacionan con los diferentes componentes del proyecto (como casos de prueba, código fuente, documentos de diseño, etc.) en columnas.
    
    .bg-full-width.bg-color-10.mb-5
      .px-4.px-md-5
        .row.justify-content-center.align-items-center
          .col-lg-12
            .row.justify-content-center.align-items-center
              .col-lg-7(data-aos="fade-left").mb-3.mb-lg-0
                p.mb-0 El objetivo principal de la matriz es proporcionar una visión clara de cómo cada requisito se implementa, y en qué fase del proyecto se valida, asegurando que no se omita ningún detalle importante. También se convierte en una herramienta útil para los gerentes de proyecto y los equipos de calidad, quienes pueden utilizarla para comprobar que todos los requisitos han sido cubiertos (Genero Bocco et al., 2014).
              .col-lg-5(data-aos="zoom-in")
                img.img-fluid(src='@/assets/curso/tema3/18.svg', style="max-width:486px", alt="" ).mx-auto.mx-lg-0.ms-lg-auto.mb-4.mb-lg-0
    
    h2(data-aos="fade-left") Estructura de la matriz de trazabilidad
    p.mb-5 La matriz de trazabilidad de requisitos, se estructura principalmente con las siguientes columnas:

    .row.align-items-start.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema3/19.png", alt="").mb-4.mb-lg-0
      .col-lg-8
        AcordionA(tipo="b")
          .div(titulo="Requisito ID")
            p Cada requisito debe tener un identificador único que permite hacer referencia a él de manera rápida y fácil. Este ID puede seguir una numeración secuencial o alguna nomenclatura que refleje la jerarquía o categoría del requisito.
    
          .div(titulo="Descripción del requisito")
            p Aquí se describe el requisito de manera clara y precisa, especificando lo que se necesita lograr.
    
          .div(titulo="Fuente del requisito")
            p En esta columna, se puede registrar la fuente o el origen del requisito, como el cliente, los usuarios, la documentación existente o cualquier otra fuente de información relevante.
    
    .row.align-items-start.mb-5
      .col-lg-4.mb-3.mb-lg-0.order-lg-2
        figure
          img(src="@/assets/curso/tema3/20.png", alt="").mb-4.mb-lg-0
      .col-lg-8.order-lg-1
        AcordionA(tipo="b")
          .div(titulo="Elementos relacionados")
            p Esta columna incluye todos los elementos relacionados con el requisito, como los casos de prueba, las funcionalidades del sistema, los documentos de diseño o las tareas de desarrollo. Esto ayuda a vincular cada requisito con los entregables específicos del proyecto.
    
          .div(titulo="Estado de implementación")
            p Aquí se indica si el requisito ha sido implementado, está en progreso, o aún no se ha comenzado a desarrollar. Esto da una visión clara del progreso del proyecto en relación con los requisitos.
    
          .div(titulo="Resultado de las pruebas")
            p Esta columna registra el estado de las pruebas realizadas para verificar que el requisito ha sido correctamente implementado. Puede incluir resultados como "Aprobado", "Requiere revisión", "Fallido", etc.
    
    h2(data-aos="fade-left") Ejemplo de una matriz de trazabilidad de requisitos
    p.mb-5 A continuación, se presenta un ejemplo sencillo de cómo se puede estructurar una matriz de trazabilidad de requisitos:
  
    .row.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema3/21.png", data-aos="zoom-in")
      .col-lg-8
        p(data-aos="fade-left") En este ejemplo, el requisito R1 describe que el sistema debe permitir el registro de usuarios, con la fuente del requisito indicada como "Cliente". La columna "Elementos Relacionados" indica que esta funcionalidad está relacionada con la pantalla de registro. El estado de implementación está marcado como "Implementado" y las pruebas realizadas han sido aprobadas.
    
        .bg-color-1.p-4(data-aos="fade-left")
          .row.align-items-start
            .col-lg-auto
              img(src="@/assets/curso/tema3/22.svg", style="max-width: 90px").mx-auto
            .col-lg
              p.mb-0 Este tipo de tabla permite a los equipos de desarrollo y calidad, tener una visión clara y rápida del estado de los requisitos y sus implementaciones correspondientes, asegurando que no se pase por alto ningún detalle y que cada requisito tenga una implementación validada.
    
    h2(data-aos="fade-left") Beneficios de la matriz de trazabilidad de requisitos
    p.mb-5 La matriz de trazabilidad de requisitos ofrece múltiples beneficios para la gestión del proyecto:

    .bg-full-width.bg-fondo-slider.mb-5
      .p-4.p-md-5
        SlyderA(tipo="b").bg-white
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/23.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Aseguramiento de calidad
              p La matriz asegura que cada requisito del sistema se implemente y se valide adecuadamente. Esto es fundamental para la calidad del producto final, dado que minimiza el riesgo de que se omitan requisitos o funcionalidades importantes (Zapata Jaramillo, 2006).
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/24.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Gestión de cambios
              p Si se presentan cambios en los requisitos durante el desarrollo, la matriz facilita el seguimiento de estos cambios. Se pueden identificar rápidamente los impactos de un cambio y ajustar el trabajo de desarrollo y prueba en consecuencia.
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/25.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Transparencia y visibilidad
              p Proporciona a todos los miembros del equipo, así como a los <em>stakeholders</em>, una visión clara de cómo se está avanzando con respecto a los requisitos. Esto fomenta una mejor comunicación y colaboración.
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/26.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Facilita la auditoría y el control
              p La trazabilidad de requisitos es una herramienta clave para auditorías y revisiones de calidad, ya que se puede demostrar cómo se ha abordado cada requisito y qué pruebas se han realizado para verificar su cumplimiento.
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema3/27.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Mejora la documentación
              p La matriz de trazabilidad actúa como un documento de referencia que permite hacer un seguimiento detallado del cumplimiento de los requisitos en todo el ciclo de vida del proyecto. Esto puede ser útil para futuras versiones del sistema o para la entrega final del producto (Genero Bocco et al., 2014).
    
    h2(data-aos="fade-left") Tipos de trazabilidad de requisitos
    p.mb-5 Existen diferentes tipos de trazabilidad de requisitos, según la fase del proyecto que se esté gestionando:

    .row.align-items-start.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema3/28.png", alt="").mb-4.mb-lg-0
      .col-lg-8
    
        AcordionA(tipo="b")
          .div(titulo="Trazabilidad hacia adelante (<em>Forward Traceability</em>)")
            p Este tipo de trazabilidad asegura que cada requisito se haya implementado y que cada parte del sistema se derive directamente de un requisito. Es decir, que cada funcionalidad desarrollada esté vinculada a un requisito específico (Genero Bocco et al., 2014).
    
          .div(titulo="Trazabilidad hacia atrás (<em>Backward Traceability</em>)")
            p Permite verificar que cada elemento del sistema, como el código o los documentos de diseño, esté asociado con un requisito original. Esto es útil para confirmar que no se han introducido elementos en el sistema que no correspondan con los requisitos iniciales (Zapata Jaramillo, 2006).
    
    .bg-full-width.bg-color-3
      .p-4.p-md-5
        h2(data-aos="fade-left") Herramientas para crear y gestionar matrices de trazabilidad de requisitos
        p.mb-5 Existen varias herramientas que pueden facilitar la creación y gestión de matrices de trazabilidad de requisitos, algunas de ellas incluyen:

        div.row.justify-content-center.align-items-stretch.mb-5
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema3/29.svg" alt="" style="width: 90px")
              h5.text-center Jira
              p.mb-0.text-center Jira es una herramienta popular para la gestión de proyectos ágiles. Tiene soporte para la creación de historias de usuario y la gestión de requisitos, y puede integrarse con otras herramientas de trazabilidad.
        
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema3/30.svg" alt="" style="width: 90px")
              h5.text-center DOORS
              p.mb-0.text-center IBM Rational DOORS es una herramienta especializada en la gestión de requisitos que permite crear matrices de trazabilidad complejas, facilitando la gestión y el seguimiento de los requisitos a lo largo de todo el ciclo de vida del proyecto.
        
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema3/31.svg" alt="" style="width: 90px")
              h5.text-center Trello
              p.mb-0.text-center Aunque no es una herramienta específica para trazabilidad, Trello puede ser configurado para gestionar requisitos y sus relaciones con las tareas del proyecto.


    .bg-full-width.border-top.color-primario
      .p-4.p-md-5
        h2(data-aos="fade-left") MATERIAL COMPLEMENTARIO
        .row.material-complementario
          .col-12.col-md-6.col-lg-7
            p Los invitamos a explorar el material complementario de este curso, en esta sección encontrará recursos que le permitirán profundizar  y enriquecer su aprendizaje en los temas tratados en esta unidad.

            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://elibro.net/es/lc/tecnologicadeloriente/titulos/27006" target="_blank" rel="noopener noreferrer") Parroquín, P. (2009). Identificación de competencias para el diseño de un modelo educativo en ingeniería de <em>Software</em>: ( ed.). Universidad Autónoma de Ciudad Juárez. 


            p.d-flex.my-4
              img.me-3(src='@/assets/template/icono-yt.svg' :style="{'max-width':'16px'}")
              a(href="https://www.youtube.com/live/ZxQNLDKaLNM?si=m18YV3I1dlWrbPAp" target="_blank" rel="noopener noreferrer") Ministerio TIC Colombia (2021, 28 de septiembre) Uso de herramientas o <em>Software</em> libre para el análisis de vulnerabilidades - 28 Sep. [Video] YouTube  

          .col-12.col-md-6.col-lg-3.offset-lg-1
            figure
              img(src='@/assets/componentes/material-complementario.svg', alt='')

</template>

<script>
export default {
  name: 'Tema3',
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
}
</script>

<style lang="sass"></style>
