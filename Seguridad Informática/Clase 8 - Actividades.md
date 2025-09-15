#clase_8

# Algoritmos simétricos de encriptado (DES) ATAQUE
https://www.abcdatos.com/programa/ataque-fortaleza-estandar-des.html

![[Pasted image 20250912001151.png]]
![[Pasted image 20250912001201.png]]
https://www.reddit.com/r/antivirus/comments/1fuwx2z/trojanmalware300983susgen_its_bad/?tl=es-419
## Ejercicio 1: Ataque Monousuario

---

12.9.25

![[Pasted image 20250912181731.png]]

![[3_ CIF_SIM_DES_ATAQUE (2).pdf]]


---

Descargar
- kali debian
- Cliente servidor , certificados ssh
	- conexión segura
- kali -> Ruptura de clave

Ir instalando Kali para tenerlo en la prox clase



![[Pasted image 20250912182914.png]]

---

# Teoría

![[Pasted image 20250912183005.png]]


Ejemplo

![[Pasted image 20250912183504.png]]

![[Pasted image 20250912183511.png]]
![[Pasted image 20250912183647.png]]

![[Pasted image 20250912184707.png]]

![[Pasted image 20250912184848.png]]
- En el parcial no se toma la cantidad de campos de un certificado. Osea, esto.


![[Pasted image 20250912185727.png]]

![[Pasted image 20250912190143.png]]

![[Pasted image 20250912190237.png]]

![[Pasted image 20250912190503.png]]

![[Pasted image 20250912191826.png]]

![[Pasted image 20250912192853.png]]

![[Pasted image 20250912193020.png]]

![[Pasted image 20250912193123.png]]

![[Pasted image 20250912193716.png]]

![[Pasted image 20250912194024.png]]

![[Pasted image 20250912194143.png]]

![[Pasted image 20250912194437.png]]

![[Pasted image 20250912194647.png]]

![[Pasted image 20250912194735.png]]

![[Pasted image 20250912195058.png]]

![[Pasted image 20250912195840.png]]

![[Pasted image 20250912200106.png]]

![[Pasted image 20250912203156.png]]

![[Pasted image 20250912203213.png]]

![[Pasted image 20250912203313.png]]

![[Pasted image 20250912203341.png]]

![[Pasted image 20250912203444.png]]

![[Pasted image 20250912203802.png]]

![[Pasted image 20250912204152.png]]

![[Pasted image 20250912204218.png]]

![[Pasted image 20250912204323.png]]

![[Pasted image 20250912204455.png]]


---


![[Pasted image 20250912205551.png]]

**1. Metodología de investigación**

- **Identificación:** Confirmar el tipo de ataque (DoS), registrar fechas, horas, sistemas afectados y patrones de repetición.
    
- **Contención:** Aislar el tráfico malicioso, implementar filtros en firewall y balanceadores.
    
- **Erradicación:** Localizar y eliminar el programa dejado por el intruso, limpiar sistemas comprometidos.
    
- **Recuperación:** Restaurar operación normal, verificar estabilidad de la red y monitoreo activo.
    
- **Lecciones aprendidas:** Documentar vectores de ataque, brechas y mejoras necesarias.
    

---

**2. Resultados obtenidos**

- Identificado que el intruso dejó un script que bloqueaba el sistema de ventas.
    
- Detectadas ventanas de ataque (entre 23 y 30 de diciembre, 4-5 ataques diarios).
    
- Restablecida la operación en las sucursales y proveedores.
    
- Aplicadas medidas de mitigación para evitar recurrencia (actualización de seguridad, monitoreo reforzado).
    
- Evidencia recolectada para rastreo forense y posible acción legal.
![[Caso de estudio 2.pdf]]

## 📝 Metodología de investigación
- **Contención inmediata:** Aislar sucursales afectadas y detener propagación.
- **Recolección de evidencia:** Logs de red, servidores, endpoints y proveedores.
- **Análisis forense:** Identificar código malicioso, hora de ejecución, IPs de origen.
- **Erradicación:** Eliminar malware, limpiar sistemas, reinstalar servicios críticos.
- **Recuperación:** Restaurar operaciones (backup, redundancia, alta disponibilidad).
- **Seguimiento:** Monitoreo post-incidente, hardening de sistemas, capacitación.
## 🔍 Información obtenida
- Ataques **recurrentes** (23–30 de diciembre, cada 2 días, varios por día).
- Afectó hasta **90% de usuarios** y proveedores.
- **Malware programado** para ejecutarse viernes 19:00hs → Denegación de servicio.
## 📌 Identificación del ataque
- **Lugar:** Red corporativa de la empresa y proveedores.
- **Hora:** Ataques planificados en horario crítico (viernes tarde).
- **Precedencia:** Acceso previo → intrusión → instalación de programa.
## 🧾 Clasificación del ataque
- **Tipo:** Denegación de Servicio (DoS) / Posible ataque distribuido (DDoS).
- **Impacto:** Disponibilidad (afecta continuidad del negocio).
## 🛠 Vulnerabilidades aprovechadas
- Falta de **control de accesos** o monitoreo de integridad.
- Ausencia de **segmentación de red** (afectó 120 sucursales).
- Posible **falla en parches** o credenciales expuestas.
## 🧪 Técnicas empleadas
- Instalación de **script/programa automatizado** (cron o servicio).
- **Persistencia** en la red (ataques recurrentes).
- Probable uso de **movimiento lateral** para escalar a proveedores.
## 🌍 Origen probable
- **Remoto**, desde Internet o VPN comprometida.
- Necesitó acceso previo → credenciales robadas o explotación de vulnerabilidad.
## 🛡 Medidas preventivas
- SIEM y **monitoreo en tiempo real**.
- **Parcheo y hardening** de servidores y POS.
- Control de **acceso remoto** y MFA.
- **Segmentación de red** y listas blancas de comunicación.
- **Planes de continuidad** y backups verificados.
- Capacitación en **conciencia de seguridad** al personal.
## 👤 Identificación del atacante
- Sin datos personales aún; requiere correlación de logs, análisis de tráfico y colaboración con **CERT/autoridades**.
# 🗺 Pendiente: Diagrama



Quienes quedamos a lo último con la consigna en manos:
![[Pasted image 20250912213145.png]]