---
layout: workshop      # NO CAMBIAR ESTO 
carpentry: "swc"    # qué tipo de Carpentry (ya sea "lc", "dc" o "swc")
venue: "LatinR - Carpentries teaching practices for R users"        # nombre breve del espacio donde se lleva adelante el taller, sin dirección (por ejemplo, "Universidad de Buenos Aires")
address: "University of Palermo"      # dirección completa del espacio donde se realizará el taller (por ejemplo, "Aula 3, Av. Córdoba 1234, Buenos Aires, Argentina")
country: "Argentina"      # código ISO del país, dos letras en minúscula como por ejemplo "fr" (ver https://en.wikipedia.org/wiki/ISO_3166-1)
language: "es"     # código ISO del idioma, dos letras en minúscula como por ejemplo "fr" (ver https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "-34.597238, -58.415996"       # latitud y longitud del espacio en formato decimal (por ejemplo, "41.7901128,-87.6007318" - usar http://www.latlong.net/)
humandate: "Sep 5, 2018"    # fechas del taller en formato legible (por ejemplo, "Feb 17-18, 2020")
humantime: "09:00 - 13:00"    # hora del taller en formato legible (por ejemplo, "9:00 am - 4:30 pm")
startdate: 2018-09-05      # fecha de inicio del taller en formato YYYY-MM-DD (por ejemplo, 2015-01-01)
enddate: 2018-09-05        # fecha de finalización del taller en formato YYYY-MM-DD, por ejemplo 2015-01-02
instructor: ["Florencia D'Andrea", "Rayna Harris"] # lista de nombres de las instructoras separados por comas y entre corchetes, como ["Florencia D'Andrea", "Rayna Harris"]
email: ["rayna.harris@gmail.com"]    # lista de direcciones de correo electrónico de contacto con la **host** ó **lead instructor**, separadas por comas y entre corchetes, como ["ada.lovelace@ejemplo.org", "carrie.fisher@ejemplo.org", "hedy.lamarr@example.org"]
collaborative_notes: https://docs.google.com/document/d/1b_9CkoRPvhzwQnZU7AAzSzD1T5MMqsiXAJAWo6xjo_c/edit?usp=sharing            # optional: URL de las notas colaborativas del taller, por ejemplo un Etherpad o documento de Google Docs 
eventbrite:           # optional: clave alfanumérica de registro en Eventbrite, por ejemplo "1234567890AB" (si se está utilizando Eventbrite)
---



<h2 id="general">General Information</h2>

{% comment %}
  INTRODUCCIÓN 

  Edita el párrafo introductorio general debajo si quieres modificar la presentación.
  
{% endcomment %}

Researchers have discovered an enormous amount about how people learn and how best to teach them. Unfortunately, much of that knowledge has not yet been translated into common classroom practice at the university level. 

In addition to teaching foundational coding and data science skills to researchers worldwide, The Carpentries organizations lead an instructor training program focuses on evidence-based best-practices of teaching.

This LatinR workshop will focus on the highlights of the two-day Carpentry instructor training program. Attendees will learn how to create a positive environment for learners at workshops, have opportunities to practice and build your teaching skills,  become integrated into the Carpentry community, and prepare you to use these teaching skills in teaching Carpentry workshops.


<h2 id="schedule">Schedule</h2>

{% if page.carpentry == "swc" %}
  {% include sc/schedule.html %}
{% elsif page.carpentry == "dc" %}
  {% include dc/schedule.html %}
{% elsif page.carpentry == "lc" %}
  {% include lc/schedule.html %}
{% endif %}

