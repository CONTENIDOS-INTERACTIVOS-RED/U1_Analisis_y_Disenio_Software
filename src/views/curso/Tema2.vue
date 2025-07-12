<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(:subTitulo="'2. Priorización de necesidades'")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.overflow-hidden

    .row.mb-5
      .col-lg-4.order-lg-2.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema2/1.png", data-aos="zoom-in")
      .col-lg-8.order-lg-1
        p(data-aos="fade-left") Una vez recopilados los requisitos de un proyecto, no todos pueden implementarse al mismo tiempo, ni con la misma urgencia. Es aquí donde la priorización de necesidades se convierte en un proceso crucial. Priorizar significa decidir qué requisitos deben atenderse primero, basándose en criterios claros y objetivos. Una adecuada priorización permite optimizar recursos, reducir riesgos y entregar valor al usuario lo antes posible (Echeverri et al., 2013).
    
        .bg-color-1.p-4(data-aos="fade-left")
          .row.align-items-start
            .col-lg-auto
              img(src="@/assets/curso/tema2/2.svg", style="max-width: 90px").mx-auto
            .col-lg
              p.mb-0 La correcta gestión de prioridades no solo mejora el resultado final del proyecto, sino que también fortalece la comunicación entre los diferentes involucrados, evitando malentendidos y frustraciones.

    #t_2_1.titulo-segundo(data-aos="flip-up")
      h2 #[span 2.1] Criterios para priorizar (valor de negocio, urgencia, viabilidad técnica)
    
    p.mb-5 Para realizar una priorización efectiva, es fundamental establecer criterios que sirvan de guía en la toma de decisiones. Entre los criterios más importantes se destacan:
  
    .bg-full-width.bg-fondo-slider.mb-5
      .p-4.p-md-5
        SlyderA(tipo="b").bg-white
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.mb-3.mb-lg-0
              figure
                img(src="@/assets/curso/tema2/3.png")
            .col-lg-7
              h5 Valor de negocio
              p El valor de negocio se refiere al impacto positivo que un requisito tiene sobre los objetivos estratégicos de la organización. Un requisito con alto valor de negocio puede aumentar ingresos, reducir costos, mejorar la satisfacción del cliente o fortalecer la ventaja competitiva (Universidad Politécnica Salesiana, 2021).
              h5 Ejemplo:
              ul.lista-ul--color
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 En una aplicación de comercio electrónico, la implementación de un sistema de pago seguro, puede tener un altísimo valor de negocio, puesto que incrementa la confianza de los usuarios y mejora la tasa de conversión de ventas.
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.mb-3.mb-lg-0
              figure
                img(src="@/assets/curso/tema2/4.png")
            .col-lg-7
              h5 Urgencia
              p La urgencia mide qué tan rápido debe atenderse una necesidad. Algunos requisitos son críticos porque están ligados a eventos próximos, fechas de lanzamiento o cambios regulatorios.
              h5 Ejemplo:
              ul.lista-ul--color
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Si una Ley exige que todas las plataformas de servicios financieros implementan autenticación biométrica antes de fin de año, este requisito debe priorizarse de manera inmediata, independientemente de su dificultad.
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.mb-3.mb-lg-0
              figure
                img(src="@/assets/curso/tema2/5.png")
            .col-lg-7
              h5 Viabilidad técnica
              p No todos los requisitos son igual de fáciles de implementar. La viabilidad técnica evalúa si el equipo cuenta con los recursos, conocimientos y tecnología necesarios, para llevar a cabo el requisito en el plazo deseado (Echeverri et al., 2013).
              h5 Ejemplo:
              ul.lista-ul--color
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Si se plantea integrar Inteligencia Artificial a una app de mensajería, pero el equipo no tiene experiencia previa en Machine <em>Learning</em>, la implementación podría no ser viable a corto plazo y requeriría capacitación previa o contratación de expertos.
    
    .row.mb-5
      .col-lg-2.order-lg-2.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema2/6.svg", data-aos="zoom-in")
      .col-lg-10.order-lg-1
        h2 Importancia de combinar criterios
        .bg-color-5.p-5(data-aos="fade-left")
          p.mb-0 La priorización efectiva siempre es un balance entre el valor de negocio, la urgencia y la viabilidad técnica. No basta que un requisito sea muy valioso si es inviable, ni que sea urgente si no aporta al negocio.
    
    #t_2_2.titulo-segundo(data-aos="flip-up")
      h2 #[span 2.2] Métodos de priorización
    
    p.mb-5 Existen diversos métodos que ayudan a priorizar requisitos de manera sistemática (Echeverri et al., 2013). Algunos de los más utilizados en la industria son:

    .row.align-items-start.mb-5
      .col-lg-4.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema2/7.png", alt="").mb-4.mb-lg-0
      .col-lg-8
    
        AcordionA(tipo="b")
          .div(titulo="Método MoSCoW")
            p Este método clasifica los requisitos en cuatro categorías:
            ul.lista-ul--color
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Must have</em></b> (Debe tener): esenciales para el funcionamiento del sistema.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Should have</em></b> (Debería tener): importantes, pero no críticos.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Could have</em></b> (Podría tener): deseables, pero prescindibles.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Won’t have this time</em></b> (No tendrá esta vez): se dejarán fuera de esta versión.
            h5 Ejemplo:
            p Al desarrollar una app bancaria:
            ul.lista-ul--color
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Must have</em></b>. Transferencias de dinero.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Should have</em></b>. Notificaciones en tiempo real.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Could have</em></b>. Personalización de temas de la interfaz.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 <b><em>Won'thave</em></b> : Integración con criptomonedas (por ahora).
            p Este método ofrece una visión rápida y comprensible para todos los involucrados, lo que facilita la toma de decisiones.
    
          .div(titulo="Método 100 puntos")
            p Cada participante del equipo asigna 100 puntos para repartir entre los requisitos, de acuerdo con la importancia que perciba (Universidad Politécnica Salesiana, 2021).
            h5 Ejemplo:
            ul.lista-ul--color
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 Si se tienen cinco requisitos, un gerente podría asignar 40 puntos al requisito más valioso, 30 a otro importante, y distribuir el resto entre los demás.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 El requisito que acumule más puntos, será el de mayor prioridad.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 Este método es particularmente útil, cuando se necesita alcanzar consenso en equipos diversos.
    
          .div(titulo="Análisis de costo-beneficio")
            p Consiste en comparar el beneficio esperado de implementar un requisito, frente al costo que implica desarrollarlo.
            h5 Ejemplo:
            ul.lista-ul--color
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 Si implementar una nueva función cuesta $5,000 pero se estima que generará $20,000 adicionales en ventas, podría considerarse prioritario.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 En cambio, si otra función cuesta $10,000 y el retorno estimado es de solo $2,000, se podría postergar o descartar.
              li.mb-0.d-flex
                i.far.fa-arrow-alt-circle-right
                p.mb-0 Esta técnica ayuda a justificar decisiones frente a la alta dirección, o ante inversores.
    
    #t_2_3.titulo-segundo(data-aos="flip-up")
      h2 #[span 2.3] Herramientas de apoyo en la priorización
    
    p.mb-5 Para facilitar el proceso de priorización, existen diversas herramientas que permiten visualizar y analizar las decisiones, de forma colaborativa:

    .bg-full-width.bg-fondo-slider.mb-5
      .p-4.p-md-5
        SlyderA(tipo="b").bg-white
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema2/8.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Matrices de priorización
              p Una matriz de priorización es una cuadrícula que permite clasificar requisitos, según dos o más criterios, como valor de negocio y esfuerzo técnico (Echeverri et al., 2013).
              h5 Ejemplo de ejes:
              ul.lista-ul--color
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Eje X. Esfuerzo (bajo a alto).
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Eje Y. Valor (bajo a alto).
              h5 Interpretación:
              ul.lista-ul--color
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Los requisitos con alto valor y bajo esfuerzo se priorizan primero.
                li.mb-0.d-flex
                  i.far.fa-arrow-alt-circle-right
                  p.mb-0 Los de bajo valor y alto esfuerzo podrían descartarse o posponerse.
    
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema2/9.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 Tableros Kanban
              p Aunque tradicionalmente se usan para gestión de tareas, los tableros Kanban también pueden adaptarse a la priorización inicial de requisitos. Dividir las columnas en categorías como “Alta prioridad”, “Media prioridad” y “Baja prioridad”, facilita la visualización.
          .row.align-items-center.p-4.p-md-5
            .col-lg-5.order-2
              figure
                img(src="@/assets/curso/tema2/10.png")
            .col-lg-7.order-1.mb-3.mb-lg-0
              h5 <em>Software</em> especializado
              p Herramientas como Jira, Trello, Monday.com o ClickUp, ofrecen funcionalidades para priorizar requisitos utilizando etiquetas, votos del equipo, tablas de esfuerzo vs. valor, y automatizaciones que apoyan la toma de decisiones (Echeverri et al., 2013).
    
    .bg-full-width.bg-color-3
      .p-4.p-md-5
        #t_2_4.titulo-segundo(data-aos="flip-up")
          h2 #[span 2.4] Resolución de conflictos entre prioridades
        
        p.mb-5 En muchos proyectos, surgirán conflictos entre los diferentes interesados, respecto a qué requisitos deben tener prioridad. Para resolver estos conflictos de manera efectiva, se deben seguir ciertos principios:

        div.row.justify-content-center.align-items-stretch.mb-5
          div.col-lg-3.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema2/11.svg" alt="" style="width: 90px")
              h5.text-center Escuchar y entender los intereses
              p.mb-0.text-center Antes de decidir, es fundamental entender por qué cada parte considera su requisito prioritario (Universidad Politécnica Salesiana, 2021). A veces, el trasfondo revela necesidades más profundas, que permiten encontrar soluciones creativas.
        
          div.col-lg-3.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema2/12.svg" alt="" style="width: 90px")
              h5.text-center Usar criterios objetivos
              p.mb-0.text-center Basarse en criterios previamente establecidos (valor de negocio, urgencia, viabilidad técnica) disminuye el componente emocional en las discusiones y facilita la negociación.
        
          div.col-lg-3.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema2/13.svg" alt="" style="width: 90px")
              h5.text-center Facilitar el consenso
              p.mb-0.text-center El facilitador del proyecto debe promover una cultura de diálogo, donde todos los involucrados sientan que su opinión fue escuchada, aunque no siempre sea aceptada.
          div.col-lg-3.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/tema2/14.svg" alt="" style="width: 90px")
              h5.text-center Escalar conflictos cuando sea necesario
              p.mb-0.text-center Si el conflicto persiste, se puede recurrir a la dirección del proyecto o al comité de <em>stakeholders</em> para que definan las prioridades estratégicas.

    .row.mb-5
      .col-lg-2.order-lg-2.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/tema2/15.svg", data-aos="zoom-in")
      .col-lg-10.order-lg-1
        h2 Ejemplo de resolución de conflicto
        .bg-color-5.p-5(data-aos="fade-left")
          p En un proyecto de desarrollo de <em>Software</em> educativo, el área de marketing insistía en priorizar el diseño visual, mientras que los docentes preferían que se priorizara la facilidad de uso. 
          p.mb-0 El equipo de desarrollo propuso una solución intermedia: un primer lanzamiento enfocado en funcionalidad básica, seguido de una segunda fase que mejorará la estética visual. Esta estrategia fue aceptada por ambas partes.


    .bg-full-width.border-top.color-primario
      .p-4.p-md-5
        h2(data-aos="fade-left") MATERIAL COMPLEMENTARIO
        .row.material-complementario
          .col-12.col-md-6.col-lg-7
            p Los invitamos a explorar el material complementario de este curso, en esta sección encontrará recursos que le permitirán profundizar  y enriquecer su aprendizaje en los temas tratados en esta unidad.

            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://elibro.net/es/lc/tecnologicadeloriente/titulos/66410" target="_blank" rel="noopener noreferrer") Díaz, J. Harari, I. & Amadeo, A. P. (2013). Guía de recomendaciones para diseño de <em>Software</em> centrado en el usuario: ( ed.). D - Editorial de la Universidad Nacional de La Plata. 


            p.d-flex.my-4
              img.me-3(src='@/assets/template/icono-yt.svg' :style="{'max-width':'16px'}")
              a(href="https://youtu.be/ccSS4C5GYxs?si=l7pZASsTR5A1-h9y" target="_blank" rel="noopener noreferrer") MobilizaAcademy (2021, 23 de julio) Las mejores metodologías ágiles para el Desarrollo de <em>Software</em>. [Video] YouTube. 



          .col-12.col-md-6.col-lg-3.offset-lg-1
            figure
              img(src='@/assets/componentes/material-complementario.svg', alt='')

</template>

<script>
export default {
  name: 'Tema2',
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
}
</script>

<style lang="sass"></style>
