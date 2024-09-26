---
title: Presentation 1
layout: post
permalink: /presentation-1/
background: '#0a5'

slides:
 - title: "Actuadores Eléctricos"
   slide-data: "**Tipos:** Motores de corriente continua (DC), Motores de corriente alterna (AC), Servomotores, Motores paso a paso.<br><br>**Funcionamiento:** Convierten energía eléctrica en movimiento mecánico mediante señales eléctricas que controlan velocidad, posición y dirección.<br><br>**Características:** Alta precisión, rápida respuesta, fácil control y monitoreo, bajo mantenimiento.<br><br>**Modo de Comunicación:** Señales analógicas (voltaje o corriente), señales digitales (PWM), comunicación por buses industriales (CAN, Modbus, etc.)."

 - title: "Actuadores Mecánicos"
   slide-data: "**Tipos:** Actuadores lineales, actuadores rotativos, actuadores de leva.<br><br>**Funcionamiento:** Transforman el movimiento rotativo en movimiento lineal o viceversa, usando mecanismos como tornillos y engranajes.<br><br>**Características:** Alta fuerza de salida, buena precisión en movimientos lineales, requiere mantenimiento.<br><br>**Modo de Comunicación:** Control manual o mecánico mediante levas y engranajes, sistemas electrónicos avanzados."

 - title: "Actuadores Hidráulicos"
   slide-data: "**Tipos:** Cilindros hidráulicos, motores hidráulicos.<br><br>**Funcionamiento:** Utilizan fluidos a presión para generar movimiento, transformando la presión hidráulica en energía mecánica.<br><br>**Características:** Alta potencia y fuerza, movimientos suaves, requiere mantenimiento del fluido.<br><br>**Modo de Comunicación:** Válvulas de control manuales o sistemas electrónicos de control de válvulas."
  
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
  <h1>{{slide.title}}</h1>
  <p>{{ slide.slide-data | markdownify }}</p>
</section>
                    
{% endfor %}


