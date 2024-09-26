---
title: Unidad 1
layout: post
permalink: /presentation-2/

slides:
 - title: "Sensores Ópticos"
   slide-data: "**Tipos:** Sensores de luz, fotodiodos, fototransistores.<br><br>**Funcionamiento:** Detectan la luz mediante la conversión de energía luminosa en señales eléctricas.<br><br>**Características:** Alta sensibilidad, respuesta rápida, rango de operación amplio.<br><br>**Modo de Comunicación:** Señales analógicas, digitales o mediante protocolos de comunicación como I2C o SPI."
   background: "#e74c3c"

 - title: "Sensores de Temperatura"
   slide-data: "**Tipos:** Termistores, termopares, sensores de infrarrojos.<br><br>**Funcionamiento:** Miden la temperatura mediante la variación de resistencia eléctrica o generación de voltaje.<br><br>**Características:** Precisión, rango de temperatura, tiempo de respuesta.<br><br>**Modo de Comunicación:** Salida analógica, digital o mediante protocolos como 1-Wire."
   background: '#f1c40f'

 - title: "Sensores de Presión"
   slide-data: "**Tipos:** Sensores piezoeléctricos, sensores de presión absoluta, manómetros.<br><br>**Funcionamiento:** Miden la presión mediante la deformación de un elemento sensible bajo carga.<br><br>**Características:** Precisión, rango de presión, sensibilidad.<br><br>**Modo de Comunicación:** Salida analógica o digital, protocolos como CAN o Modbus."
   background: '#9b59b6'

 - title: "Sensores de Proximidad"
   slide-data: "**Tipos:** Sensores inductivos, capacitivos, ultrasónicos.<br><br>**Funcionamiento:** Detectan la presencia de un objeto sin contacto, utilizando campos eléctricos o ultrasónicos.<br><br>**Características:** Rango de detección, sensibilidad, respuesta rápida.<br><br>**Modo de Comunicación:** Salida digital o analógica, protocolos como I2C o RS-232."
   background: '#3498db'

---

{% for slide in page.slides %}
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
  <h1>{{slide.title}}</h1>
  <p>{{ slide.slide-data | markdownify }}</p>
</section>
{% endfor %}
