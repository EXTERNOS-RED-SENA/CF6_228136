<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 4
      h1 Gestión del conocimiento
    
    .bloque-texto-g.color-secundario.p-3.p-sm-4.p-md-5(data-aos="flip-up" data-aos-duration="1000")
      .bloque-texto-g__img(
        :style="{'background-image': `url(${require('@/assets/curso/tema4/1.png')})`}"
      )
      .bloque-texto-g__texto.p-4
        p.mb-0 La gestión del conocimiento en el contexto de datos masivos representa un desafío que va más allá del simple almacenamiento de información. Implica la creación de un ecosistema que facilite la captura, organización, distribución y evolución del conocimiento organizacional relacionado con datos y análisis. Este capítulo explora las estrategias y mejores prácticas para gestionar efectivamente el conocimiento en proyectos de analítica avanzada.
    
    Separador
    .titulo-segundo
      h2#t_4_1 4.1 Organización de la información
    p La organización efectiva de la información constituye la base de una gestión del conocimiento exitosa. Un sistema bien estructurado permite no solo almacenar información, sino también facilitar su descubrimiento y utilización cuando se necesita. La arquitectura de información debe considerar tanto las necesidades actuales como la escalabilidad futura.
    p Para comprender mejor las diferentes dimensiones de la organización de información en proyectos de datos masivos, consideremos la siguiente taxonomía de activos de conocimiento:
    .titulo-sexto.color-acento-contenido
      p.mb-0 #[b Tabla 3.] Taxonomía sugerida sobre activos de conocimiento
    
    .tabla-a.color-primario.mb-4
      table
        caption.fw-normal #[strong Fuente.] OIT, 2024.
        thead
          tr.text-white.text-center(style="background-color:#03A9F4;")
            th Tipo de activo
            th Contenido principal
            th Método de organización
            th Frecuencia de actualización
            th Herramientas recomendadas
        tbody.text-center
          tr.bg-white
            td Documentación técnica
            td Especificaciones, arquitectura, código
            td Sistema jerárquico por componentes
            td Alta - con cada cambio
            td Git, Confluence, Sphinx
          tr.bg-white
            td Conocimiento procedimental
            td Flujos de trabajo, procedimientos, guías
            td Organización por procesos
            td Media - cambios en procesos
            td Wiki, Notion, Sharepoint
          tr.bg-white
            td Metadatos
            td Diccionarios de datos, linaje
            td Estructura relacional
            td Alta - cambios en datos
            td Data catalogs, neo4j
          tr.bg-white
            td Mejores prácticas
            td Guías, estándares, lecciones aprendidas
            td Categorización temática
            td Baja - revisión periódica
            td Confluence, gitbook
          tr.bg-white
            td Artefactos de modelo
            td Modelos, pipelines, configuraciones
            td Versionamiento semántico
            td Alta - iteración continua
            td MLflow, DVC, Git LFS
          tr.bg-white
            td Conocimiento contextual
            td Decisiones, razonamiento, contexto
            td Organización temporal y por proyecto
            td Media - eventos significativos
            td Confluence, Jira
    .row.justify-content-center.mb-2
      .col-lg-10
        .fondo-color-sistema-j.p-2
          .row.align-items-center
            .col-md-auto
              figure.mb-4.mb-md-0
                img.mx-auto(src="@/assets/curso/tema4/2.svg",style="max-width: 90px;")
            .col
              p.mb-0 Esta taxonomía proporciona un marco de referencia para organizar sistemáticamente los diferentes tipos de conocimiento generados en proyectos de analítica, facilitando su gestión y acceso efectivo.
    Separador
    .titulo-segundo(data-aos="flip-up")
      h2#t_4_2 4.2 Control de versiones
    .row.justify-content-center.mb-5
      .col-sm-12.col-lg-7
        p.mb-3 El control de versiones en la gestión del conocimiento trasciende la mera gestión de cambios en documentos. Implica mantener un registro coherente de la evolución del conocimiento organizacional, incluyendo el contexto y razonamiento detrás de cada modificación.
        p.mb-0 El proceso de control de versiones en la gestión del conocimiento sigue un flujo complejo que integra múltiples aspectos y consideraciones. La siguiente infografía ilustra la interrelación entre los diferentes elementos del sistema de control de versiones y su impacto en la gestión del conocimiento organizacional:
      .col-sm-12.col-lg-5.d-none.d-lg-block
          img(src="@/assets/curso/tema4/3.png")
    .row.justify-content-center.mb-4.bgcolor-1.p-4
      .col-sm-12.col-lg-7
        .titulo-sexto.color-acento-contenido
          p.mb-0 #[b Figura 2.] Ecosistema de control de versiones en gestión del conocimiento
        
        figure.mb-2
          img(src="@/assets/curso/tema4/5.svg", alt='La Figura 2 se denomina « Ecosistema de control de versiones en gestión del conocimiento» y muestra un sistema integral que enlaza distintos elementos de la gestión del conocimiento, desde su captura inicial hasta su distribución y actualización en la organización.')
        figcaption.fw-normal #[em #[b Fuente]: OIT, 2024.]
    .row.align-items-center.mb-4
      .col-sm-12.col-lg-7
        p.mb-4 Como se observa en el diagrama, el control de versiones actúa como un sistema integrado que conecta diferentes aspectos de la gestión del conocimiento, desde la captura inicial hasta la distribución y actualización del conocimiento organizacional. Elementos clave en el control de versiones incluyen:
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 Políticas de versionamiento claramente definidas
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 Sistemas de nomenclatura estandarizados
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 Procesos de revisión y aprobación
        .fondo-color-sistema-f.py-3.px-4
          p.mb-0 Mecanismos de trazabilidad

      .col-sm-12.col-lg-5.d-none.d-lg-block
        figure.mb-4.mb-lg-0
          img(src="@/assets/curso/tema4/4.svg")
    
    
    Separador
    .titulo-segundo(data-aos="flip-up")
      h2#t_4_3 4.3 Mejores prácticas de mantenimiento
    p.mb-5 El mantenimiento efectivo del conocimiento organizacional requiere un enfoque sistemático y proactivo. Las mejores prácticas de mantenimiento aseguran que el conocimiento permanezca relevante, accesible y útil a lo largo del tiempo. La revisión periódica del conocimiento almacenado resulta esencial para mantener su validez y utilidad. Este proceso debe incluir la identificación de contenido obsoleto, la actualización de información desactualizada y la incorporación de nuevo conocimiento relevante.
    .row.align-items-center.mb-4
      .col-sm-12.col-lg-7
        p.mb-4 El mantenimiento del conocimiento debe considerar múltiples dimensiones:
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 #[b Dimensión tecnológica:] asegurar que la infraestructura y herramientas de gestión del conocimiento funcionen eficientemente y se mantengan actualizadas.
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 #[b Dimensión organizacional:] establecer roles y responsabilidades claras para el mantenimiento del conocimiento, incluyendo la designación de expertos en dominios específicos.
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 #[b Dimensión cultural:] fomentar una cultura de compartir y mantener el conocimiento, donde la documentación y actualización de información se consideren parte integral del trabajo.

      .col-sm-12.col-lg-5.d-none.d-lg-block
        figure.mb-4.mb-lg-0
          img(src="@/assets/curso/tema4/6.png")
    .row.justify-content-center.mb-5
      .col-sm-12.col-lg-5.d-none.d-lg-block
        img(src="@/assets/curso/tema4/7.png")
      .col-sm-12.col-lg-7
        p.mb-4 La automatización juega un papel cada vez más importante en el mantenimiento del conocimiento. Las herramientas modernas pueden ayudar a identificar contenido desactualizado, verificar enlaces rotos y sugerir actualizaciones basadas en cambios en sistemas relacionados.
        p.mb-4 La gestión de dependencias entre diferentes elementos de conocimiento requiere especial atención. Cuando se actualiza un componente, es necesario evaluar y actualizar todos los elementos relacionados para mantener la coherencia del sistema de conocimiento.
        p.mb-0 El monitoreo continuo de la utilización y efectividad del conocimiento proporciona insights valiosos para el mantenimiento. Las métricas de uso, feedback de usuarios y patrones de acceso pueden ayudar a identificar áreas que requieren atención o mejora.
    p.mb-5 La documentación del proceso de mantenimiento en sí mismo resulta fundamental. Esto incluye:
    .row.align-items-center.mb-4
      .col-sm-12.col-lg-7
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 Registro de decisiones de mantenimiento.
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 Documentación de procedimientos de actualización
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 Historiales de cambios y sus motivaciones
        .fondo-color-sistema-f.py-3.px-4.mb-4
          p.mb-0 Lecciones aprendidas durante el proceso
        p.mb-0 La sostenibilidad a largo plazo del sistema de gestión del conocimiento depende de la capacidad para adaptarse a cambios en las necesidades organizacionales, tecnologías emergentes y prácticas evolutivas en el campo de la analítica de datos.

      .col-sm-12.col-lg-5.d-none.d-lg-block
        figure.mb-4.mb-lg-0
          img(src="@/assets/curso/tema4/8.png")


</template>

<script>
export default {
  name: 'Tema4',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
