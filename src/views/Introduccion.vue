<template lang="pug">
.curso-main-container.introduccion
  BannerInterno(subTitulo="Introducción")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5

    .row
      .col-lg-4.order-lg-2.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/intro/1.png", data-aos="zoom-in")
      .col-lg-8.order-lg-1
        p.mb-5(data-aos="fade-left") En el proceso de desarrollo de software, uno de los pasos más críticos es la recolección y análisis de requisitos. Esta unidad introduce a los estudiantes en el arte de entender, capturar y organizar las necesidades del cliente o usuario final, una tarea esencial para garantizar el éxito de cualquier proyecto tecnológico. El estudio de esta unidad es fundamental porque permite identificar correctamente, qué debe hacer el sistema antes de pasar al diseño y la implementación, reduciendo costos, tiempos y errores futuros.
    
        .bg-color-1.p-4(data-aos="fade-left")
          p.mb-0 Dominar el proceso de recolección y análisis de requisitos, no solo incrementa las probabilidades de éxito en el desarrollo de software, sino que también potencia habilidades de comunicación, análisis crítico y resolución de problemas, competencias muy valoradas en la industria. En su vida profesional, los estudiantes trabajarán frecuentemente con clientes o usuarios que tal vez no sepan expresar sus necesidades de manera técnica, por lo que contar con un buen proceso de recolección y análisis, será crucial para transformar esas necesidades en soluciones reales.
    
    .bg-full-width.bg-color-3
      .p-4.p-md-5
        p Por ejemplo, el éxito de aplicaciones como Uber o Amazon, no solo radicó en su programación, sino en la correcta comprensión de lo que sus usuarios realmente necesitaban.
        p.mb-5 La unidad está organizada con la siguiente temática principal:
        div.row.justify-content-center.align-items-stretch
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/intro/2.svg" alt="" style="width: 90px")
              h5.text-center Técnicas de recopilación de requisitos
              p.mb-0.text-center Aprenderemos métodos como entrevistas, encuestas, talleres y observación directa, para obtener información relevante de los usuarios.
        
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/intro/3.svg" alt="" style="width: 90px")
              h5.text-center Priorización de necesidades
              p.mb-0.text-center Se estudiarán estrategias para clasificar y jerarquizar los requisitos más importantes, facilitando la toma de decisiones de diseño y desarrollo.
        
          div.col-lg-4.mb-4(data-aos="zoom-in-up")
            div.bg-color-white.box-shadow.px-4.py-5.h-100
              img.mx-auto.d-block.mb-4(src="@/assets/curso/intro/4.svg" alt="" style="width: 90px")
              h5.text-center Herramientas de análisis
              p.mb-0.text-center Exploramos herramientas que ayudan a organizar y visualizar la información recolectada, como los diagramas de casos de uso, matrices de trazabilidad, y mapas de empatía.
      
    .row.mb-5
      .col-lg-5.mb-3.mb-lg-0
        figure
          img(src="@/assets/curso/intro/5.png", data-aos="zoom-in")
      .col-lg-7
        .bg-color-2.px-5.py-4.h-100(data-aos="fade-left")
          p.mb-0.text-white Se espera que los estudiantes participen activamente en las actividades prácticas, fomentando el trabajo en equipo, la comunicación efectiva y el pensamiento crítico. Además, se recomienda haber repasado conceptos básicos de comunicación efectiva y metodologías ágiles, dado que serán de utilidad durante el proceso de recolección y análisis. El compromiso con la práctica y la retroalimentación, será clave para lograr los resultados de aprendizaje esperados.
</template>
