# Laboratorio de EtherChannel (PAgP – LACP – Redundancia)

## 🧪 Descripción

Este laboratorio muestra la configuración de enlaces troncales y canales EtherChannel utilizando los protocolos *PAgP* y *LACP, además de un **EtherChannel redundante* entre switches.  
El objetivo fue optimizar el ancho de banda y asegurar la disponibilidad de la red ante fallas en uno de los enlaces físicos.

## 🧭 Topología

- 3 Switches Cisco 2960
- Enlaces troncales entre los switches
- Configuración de EtherChannel con:
  - PAgP
  - LACP
  - Un canal redundante
- Verificación de enlaces trunk y configuración manual donde no estaban activados.

## ⚙ Configuración realizada

- Verificación de estado de interfaces con:
show interfaces | include Ethernet
show interface summary
show interfaces trunk
- Configuración de trunk en interfaces que no lo tenían:
  switchport mode trunk
  - Configuración de EtherChannel:
- PAgP en modo *desirable* y *auto*
- LACP en modo *active* y *passive*
- EtherChannel redundante como respaldo.

## ✅ Resultado esperado

- Todos los enlaces operativos como *trunk*.  
- Canales EtherChannel activos y funcionando correctamente.  
- Redundancia asegurada en caso de caída de un enlace físico.

## 📝 Archivo

- 6.2.4-packet-tracer---configure-etherchannel_es-XL.pkt → Archivo de Packet Tracer con toda la topología configurada.

## 🧠 Aprendizajes

- Diferencias entre PAgP y LACP.
- Importancia de configurar correctamente los enlaces troncales antes de crear el canal.
- Verificación del estado de los canales y su redundancia.
- Buenas prácticas de escalabilidad en redes LAN.

---

✍ Autor/a: [Stefania]  
📅 Fecha: Octubre 2025
