---
layout: workshop      # NO CAMBIAR ESTO 
carpentry: "swc"    # qué tipo de Carpentry (ya sea "lc", "dc" o "swc")
venue: "LatinR"        # nombre breve del espacio donde se lleva adelante el taller, sin dirección (por ejemplo, "Universidad de Buenos Aires")
address: "University of Palermo"      # dirección completa del espacio donde se realizará el taller (por ejemplo, "Aula 3, Av. Córdoba 1234, Buenos Aires, Argentina")
country: "Argentina"      # código ISO del país, dos letras en minúscula como por ejemplo "fr" (ver https://en.wikipedia.org/wiki/ISO_3166-1)
language: "es"     # código ISO del idioma, dos letras en minúscula como por ejemplo "fr" (ver https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "-34.597238, -58.415996"       # latitud y longitud del espacio en formato decimal (por ejemplo, "41.7901128,-87.6007318" - usar http://www.latlong.net/)
humandate: "Sep 5, 2018"    # fechas del taller en formato legible (por ejemplo, "Feb 17-18, 2020")
humantime: "09:00 - 13:00"    # hora del taller en formato legible (por ejemplo, "9:00 am - 4:30 pm")
startdate: 2018-09-05      # fecha de inicio del taller en formato YYYY-MM-DD (por ejemplo, 2015-01-01)
enddate: 2018-09-05        # fecha de finalización del taller en formato YYYY-MM-DD, por ejemplo 2015-01-02
instructor: ["Florencia D'Andrea", "Rayna Harris"] # lista de nombres de las instructoras separados por comas y entre corchetes, como ["Florencia D'Andrea", "Rayna Harris"]
helper: ["estar determinado"]     # lista de nombres de las **helpers** separados por comas y entre corchetes, como ["Carrie Fisher", "Frances Allen", "Margaret Hamilton"]
email: ["rayna.harris@gmail.com"]    # lista de direcciones de correo electrónico de contacto con la **host** ó **lead instructor**, separadas por comas y entre corchetes, como ["ada.lovelace@ejemplo.org", "carrie.fisher@ejemplo.org", "hedy.lamarr@example.org"]
collaborative_notes: https://docs.google.com/document/d/1b_9CkoRPvhzwQnZU7AAzSzD1T5MMqsiXAJAWo6xjo_c/edit?usp=sharing            # optional: URL de las notas colaborativas del taller, por ejemplo un Etherpad o documento de Google Docs 
eventbrite:           # optional: clave alfanumérica de registro en Eventbrite, por ejemplo "1234567890AB" (si se está utilizando Eventbrite)
---



<h2 id="general">Información General</h2>

{% comment %}
  INTRODUCCIÓN 

  Edita el párrafo introductorio general debajo si quieres modificar la presentación.
  
{% endcomment %}

Los estudiantes, científicos y profesiones pasan cada vez más tiempo creando y utilizando software, escribiendo códigos y analizando datos sin que nunca se les enseñe cómo hacerlo de manera eficiente. [The Carpentries](https://carpentries.org) es una organización sin fines de lucro y una comunidad centrada en enseñar habilidades de codificación y ciencia de datos. Nuestra comunidad de voluntarios desarrolla lecciones de código abierto y enseña talleres en todo el mundo. Ofrecemos clases de español para enseñar ["R para análisis científico reproducible"](https://swcarpentry.github.io/r-novice-gapminder-es/), ["Control de versiones con Git"](https://swcarpentry.github.io/git-novice-es/), ["El terminal de Unix"](https://swcarpentry.github.io/shell-novice-es/). Nuestros esfuerzos actuales y futuros se enfocarán en continuar traduciendo más lecciones, apoyando traducciones de lecciones existentes, y construyendo comunidades de carpintería en América Latina de manera más amplia.

{% if page.latlng %}
<p id="where">
  <strong>Dónde: </strong>
  {{page.address}}.
  Obtener direcciones con:
  <a href="//www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16">OpenStreetMap</a>
  o
  <a href="//maps.google.com/maps?q={{page.latlng}}">Google Maps</a>.
</p>
{% endif %}

{% comment %}
  FECHA

  Este bloque muestra la fecha y enlaces a Google Calendar.
{% endcomment %}
{% if page.humandate %}
<p id="when">
  <strong>Cuándo:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% comment %}
  REQUERIMIENTOS ESPECIALES
  
  Modifica este bloque si hay algún requerimiento especial.
{% endcomment %}
<p id="requirements">
  <strong>Requerimientos:</strong> Las asistentes deben traer una computadora portátil con sistema operativo Mac, Linux o Windows (no tablet, Chromebook, etc.), que tenga permisos de administradora habilitados. Deben tener algunos paquetes de software específicos instalados. 
	

**Esta lección supone que tienes el software R y RStudio instalado en tu computadora.** 
R se puede descargar [aquí](https://cran.r-project.org/mirrors.html).
RStudio es un entorno de desarrollo integrado para R.
Se puede descargar [aquí](https://www.rstudio.com/products/rstudio/download/).
Necesitaras la versión de escritorio para tu computadora.


</p>


{% comment %}
  ACCESIBILIDAD

  Modifica este bloque si existen barreras de accesibilidad o instrucciones especiales.
{% endcomment %}
<p id="accessibility">
  <strong>Accesibilidad:</strong> Los materiales se entregaran antes del taller, también se encuentra disponible material impreso si se pide a los organizadores con anticipación. Si podemos ayudar a facilitar el aprendizaje (por ejemplo, con intérpretes de lenguaje de señas, o instalaciones para lactancia) por favor contáctanos (utilizando los detalles de contacto listados debajo) e intentaremos proveerlos.
</p>

{% comment %}
  DIRECCIONES DE CORREO ELECTRÓNICO DE CONTACTO

  Muestra los correos electrónicos de contacto definidos en el archivo de configuración.
{% endcomment %}
<p id="contact">
  <strong>Contacto</strong>:
  Por favor escribe a
  {% if page.email %}
    {% for email in page.email %}
      {% if forloop.last and page.email.size > 1 %}
        o
      {% else %}
        {% unless forloop.first %}
        ,
        {% endunless %}
      {% endif %}
      <a href='mailto:{{email}}'>{{email}}</a>
    {% endfor %}
  {% else %}
    a ser anunciado
  {% endif %}
  para más información.
</p>

<hr/>

{% comment %}
  SCHEDULE



 Muestra el cronograma del taller. Edita los ítems y horarios en la tabla para ajustarlos a tu planificación. Puede que quieras modificar 'Día 1' y 'Día 2' para mostrar fechas concretas o días de la semana.

{% endcomment %}
<h2 id="schedule">Cronograma</h2>

{% comment %} NO EDITAR LOS ENLACES A LAS ENCUESTAS {% endcomment %}
<p><em>Encuestas</em></p>
{% if page.carpentry == "swc" %}
<p>Por favor, asegúrese de completar estas encuestas antes y después del taller.</p>
<p><a href="{{ site.swc_pre_survey }}{{ site.github.project_title }}">Encuesta pre-taller</a></p>
<p><a href="{{ site.swc_post_survey }}{{ site.github.project_title }}">Encuesta post-taller</a></p>

{% elsif page.carpentry == "dc" %}
  <p>Por favor, asegúrese de completar estas encuestas antes y después del taller.</p>
<p><a href="{{ site.dc_pre_survey }}{{ site.github.project_title }}">Pre-workshop Survey</a></p>
<p><a href="{{ site.dc_post_survey }}{{ site.github.project_title }}">Post-workshop Survey</a></p>
{% elsif page.carpentry == "lc" %}
<p>Pregúntele a su instructor acerca de los detalles de la encuesta antes y después del taller.</p>
{% endif %}


{% if page.carpentry == "swc" %}
  {% include sc/schedule.html %}
{% elsif page.carpentry == "dc" %}
  {% include dc/schedule.html %}
{% elsif page.carpentry == "lc" %}
  {% include lc/schedule.html %}
{% endif %}

{% comment %}
  Notas de colaboración

  Si quieres usar un Etherpad, ve a

      http://pad.software-carpentry.org/YYYY-MM-DD-site

  donde 'YYYY-MM-DD-site' es el identificador de su taller,
  e.g., '2015-06-10-esu'.
{% endcomment %}
{% if page.collaborative_notes %}
<p id="collaborative_notes">
 Utilizaremos este <a href="{{page.collaborative_notes}}"> documento colaborativo </a> para chatear, tomar notas y compartir URL y fragmentos de código.
</p>
{% endif %}

<hr/>

{% comment %}
  CURRICULA

  En inglés, syllabus. Muestra que tópicos van a ser cubiertos.

  1. Si tu taller es sobre R antes que Python, remueve el comentario
     alrededor de esa sección y pon un comentario alrededor de la sección Python.
  2. Algunos talleres van a remover SQL.
  3. Por favor asegúrate que la lista de tópicos está sincronizada con lo que
     pretendes enseñar.
  4. Podría ser que necesites mover los campos div con class="col-md-6" alrededor
     dentro de los div con class="row" para balancear el diseño multi-columnar.

  Este es uno de los lugares donde la gente frecuentemente comete errores, así que
  por favor observa la previsualización del sitio antes de comitear, y asegúrate
  de ejecutar también 'tools/check'.
{% endcomment %}

<h2 id="syllabus">Currícula</h2>

{% if page.carpentry == "swc" %}
  {% include sc/syllabus.html %}
{% elsif page.carpentry == "dc" %}
  {% include dc/syllabus.html %}
{% elsif page.carpentry == "lc" %}
  {% include lc/syllabus.html %}
{% endif %}

<hr/>

