<!-- Encabezado con banner -->
<div align="center">

# 🛰️ **Proyecto de Simulación de Red — Lesand Corp**  

🔐 **Ciberseguridad | Redes | Infraestructura IT | Simulación Cisco Packet Tracer**

---

</div>

<p align="center">
  <img src="https://img.shields.io/badge/Cisco%20Packet%20Tracer-8.2.0-blue?style=for-the-badge&logo=cisco" />
  <img src="https://img.shields.io/badge/Networking-CCNA%20Level-blueviolet?style=for-the-badge&logo=linuxfoundation" />
  <img src="https://img.shields.io/badge/Linux-Intermediate-orange?style=for-the-badge&logo=linux" />
  <img src="https://img.shields.io/badge/Cybersecurity-In%20Progress-success?style=for-the-badge&logo=datadog" />
</p>

---

## 🏢 Escenario del proyecto  

**Lesand Corp** es una organización dedicada a las **tecnologías de la información (TI)**.  
Inicialmente contaba con una única sede conectada a Internet, pero debido a su crecimiento decidió **migrar parte de sus usuarios a una nueva ubicación** y ampliar su infraestructura tecnológica.  

El nuevo diseño debía:  
- Mantener la conectividad segura con la sede original (usuarios directivos).  
- Incorporar un **nuevo campus corporativo** con áreas especializadas (*Desarrollo, Testing, Producción, TI, Ciberseguridad*).  
- Establecer una conexión con un **SOC externo** mediante un **enlace MPLS**, para centralizar la supervisión y gestión de eventos de seguridad.  

El objetivo fue **garantizar la disponibilidad, escalabilidad y seguridad de la red**, aplicando buenas prácticas de diseño y segmentación.

---

## 🎯 Objetivos principales  

✅ Diseñar y desplegar una infraestructura de red escalable.  
✅ Integrar la red original con un nuevo campus mediante enlace MPLS.  
✅ Configurar VLANs, DHCP, DNS, NAT y servicios de red esenciales.  
✅ Implementar redundancia (HSRP), enrutamiento dinámico (OSPF, BGP, RIP).  
✅ Establecer túneles VPN y monitoreo con SNMP, NTP y NetFlow.  

---

## 🧩 Etapas del proyecto  

### 🔹 [Etapa 1 — Infraestructura y SOC](./Etapa1_Infraestructura_y_SOC/)
- Instalación y conexión de routers y switches (Cisco 2811, 2960, 3560).  
- Asignación de direccionamiento IPv4 y configuración básica de dispositivos.  
- Habilitación de servicios HTTP, FTP, DHCP, DNS y correo electrónico.  
- Implementación de acceso remoto (Telnet) y gestión del SOC.
📂 [Packet Tracer](./Etapa1_Infraestructura_y_SOC/packet_tracer_file/Etapa1_LesandCorp.7z) | 📑 [Informe PDF](./Etapa1_Infraestructura_y_SOC/reporte/Etapa1_Informe_LesandCorp.pdf)

### 🔹 [Etapa 2 — Segmentación y Red de Campus](./Etapa2_VLANs_y_Campus/)
- Creación de VLANs por departamentos (Desarrollo, Testing, Producción, TI, Ciberseguridad, Invitados).  
- Configuración de enlaces troncales y gateways (SVI).  
- Activación de DHCP en switches de distribución.  
- Implementación de PortChannel y LLDP en SOC.
📂 [Packet Tracer](./Etapa2_VLANs_y_Campus/packet_tracer_file/Etapa2_LesandCorp_VLANs.zip) | 📑 [Informe PDF](./Etapa2_VLANs_y_Campus/reporte/Etapa2_LesandCorp_VLANs.pdf)

### 🔹 [Etapa 3 — Enrutamiento IPv6 y Alta Disponibilidad](./Etapa3_IPv6_y_HSRP/)
- Configuración de IPv6 y direcciones *link-local*.  
- Implementación de HSRP para redundancia en la red de Gerencia.  
- Configuración de STP y *tracking* de interfaces.  
- Integración dual-stack (IPv4 e IPv6).
📂 [Packet Tracer](./Etapa3_IPv6_y_HSRP/packet_tracer_file/Etapa3_HSRP_DualStack.zip) | 📑 [Informe PDF](./Etapa3_IPv6_y_HSRP/reporte/Etapa3_HSRP_DualStack.pdf)

### 🔹 [Etapa 4 — Protocolos de Enrutamiento Dinámico](./Etapa4_OSPF_BGP_RIP/)
- Configuración de OSPF (áreas 0 y 51) en IPv4 e IPv6.  
- Sumarización y redistribución de rutas por defecto.  
- Implementación de BGP entre el ISP y la red de Gerencia.  
- Configuración de RIPv2 en redes internas.
📂 [Packet Tracer](./Etapa4_OSPF_BGP_RIP/packet_tracer_file/Etapa4_Enrutamiento_Dinamico.7z) | 📑 [Documentación PDF](./Etapa4_OSPF_BGP_RIP/reporte/Etapa4_Routing_Documentation.pdf)

### 🔹 [Etapa 5 — Servicios Avanzados y VPN](./Etapa5_VPN_y_Servicios/)
- Configuración de NAT dinámico y SNAT.  
- Implementación de SNMP, NTP y NetFlow para monitoreo.  
- Creación de túneles GRE entre sedes (RT-INET, RT-G1, RT-G2).  
- Restricción de acceso remoto por VLAN (Telnet solo para IT).

---

## 🧠 Tecnologías y herramientas utilizadas  

| Categoría | Tecnologías |
|:----------:|:------------|
| **Simulación** | Cisco Packet Tracer 8.1.1 – 8.2.0 |
| **Sistemas** | Cisco IOS, Linux |
| **Protocolos** | VLAN, DHCP, DNS, FTP, HTTP, SMTP, LLDP, STP, OSPF, BGP, RIPv2, HSRP, IPv6, NAT, SNMP, NTP, NetFlow, GRE |
| **Servicios** | Web, Correo, DHCP, DNS, VPN, SOC |

---

## 💡 Aprendizajes clave  

- Diseño y documentación de redes empresariales.  
- Configuración de dispositivos Cisco y servicios de red.  
- Implementación de enrutamiento y alta disponibilidad.  
- Integración y monitoreo de múltiples sedes.  
- Aplicación de buenas prácticas en seguridad de infraestructura.  

---

## 🚀 Extensiones futuras  

- 🔐 Implementar IDS/IPS (Snort o Suricata).  
- 🧩 Integrar autenticación AAA (TACACS+ / RADIUS).  
- 🕵️ Simular ataques controlados y respuesta ante incidentes.  
- ☁️ Crear escenarios híbridos con AWS / Azure.  
- 🧠 Automatizar configuraciones con Python y Ansible.  





---

⭐ _Este proyecto replica un entorno corporativo real, aplicando principios de diseño, segmentación y seguridad de red fundamentales para el desarrollo profesional en ciberseguridad._  

</div>
