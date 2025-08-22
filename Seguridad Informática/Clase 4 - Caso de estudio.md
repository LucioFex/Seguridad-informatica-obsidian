#clase_4


![[Pasted image 20250821213457.png]]
![[Pasted image 20250821213459.png]]

---

Metodología de investigación
- Este es un incidente, se realizará una investigación forense digital estructura por fases

**Fase 1: Análisis inicial y contención**
- Información del caso: Delito de extorsión.
- Corroboración: Entrevista a los gerentes afectados + Reserva de evidencia (ej: mails)
- Contención: Identificación data leaks.
**Fase 2: Análisis forense de la evidencia**
- Clasificación del ataque: Doxing y extorsión.
- Análisis de vulnerabilidad y ténicas
	- Hard skills: Un servidor mal configurado, software desactualizado, credenciales débiles o la falta de autenticación de dos factores (MFA).
	- Soft skils: Un empleado que fue víctima de **phishing** (cediendo sus credenciales) o un **actor interno** (empleado o ex-empleado con acceso previo a la información).
- Análisis de artefactos digitales
	- Análisis de cabeceras de correo
	- Análisis de metadatos de archivos
	- Análisis de logs
**Resultados esperados**
- Identificación de la vulnerabilidad
- Origen del ataque
- Identificación del atacante
**Medidas Preventivas**
- Técnicas
- Organizativas


---



### 1. Metodología de Investigación

Para abordar este incidente, se propone una metodología de investigación forense digital estructurada en las siguientes fases, respondiendo a las preguntas guía.

#### **Fase 1: Análisis Inicial y Contención**

- **Información del caso:** Se trata de un delito de **extorsión**. Un atacante anónimo obtuvo información confidencial y exige un pago a los gerentes de la empresa para no divulgarla. La comunicación y el envío de pruebas (archivos `.docx` y `.xlsx`) se realizan por correo electrónico.
- **Corroboración:** Se debe entrevistar a los gerentes afectados y asegurar de inmediato la evidencia digital: los correos electrónicos originales (en formato `.eml` para preservar las cabeceras) y los documentos adjuntos. Esto corrobora la denuncia y da inicio a la investigación técnica.
- **Contención:** Es crucial identificar la fuente de la fuga de datos y aislar los sistemas afectados para prevenir una mayor exfiltración de información.

---
#### **Fase 2: Análisis Forense de la Evidencia**

- **Clasificación del ataque:** El incidente es un **ataque dirigido de extorsión (doxing)**, que implica la amenaza de publicar información privada. No es ransomware, ya que no se cifran los datos, sino que se amenaza con su divulgación.
- **Análisis de vulnerabilidades y técnicas:** El atacante probablemente explotó una o varias de las siguientes vulnerabilidades:
    - **Técnicas:** Un servidor mal configurado, software desactualizado, credenciales débiles o la falta de autenticación de dos factores (MFA).
    - **Humanas:** Un empleado que fue víctima de **phishing** (cediendo sus credenciales) o un **actor interno** (empleado o ex-empleado con acceso previo a la información).
- **Análisis de artefactos digitales:**
    
    1. **Análisis de cabeceras de correo:** Se examinarán las cabeceras de los correos recibidos para trazar la ruta de envío e intentar identificar la dirección IP de origen. Sin embargo, es muy probable que el atacante haya utilizado servicios de anonimización como VPNs o la red Tor.
        
    2. **Análisis de metadatos de archivos:** Se analizarán los metadatos de los documentos `.docx` y `.xlsx` en busca de información como nombres de usuario, nombres de equipo, versiones de software o rutas de red que pudieran delatar al autor.
        
    3. **Análisis de logs:** Se revisarán los registros (logs) de los servidores de la empresa, firewalls y sistemas de autenticación en busca de accesos no autorizados o patrones de descarga de datos anómalos que coincidan con la fecha del incidente.
        

---

### 2. Resultados Esperados

La investigación probablemente arrojará los siguientes resultados:

- **Identificación de la vulnerabilidad:** Se logrará determinar con alta probabilidad el fallo de seguridad que permitió al atacante acceder a la información (ej. una cuenta de correo comprometida por phishing, una vulnerabilidad en un servidor web, etc.).
    
- **Origen del ataque:** Es poco probable identificar la ubicación física exacta del atacante si utilizó herramientas de anonimato. Sin embargo, el análisis de la información robada y los logs de acceso podría revelar si el origen es **interno o externo**. Un exempleado, por ejemplo, conocería exactamente qué información es más valiosa para la extorsión.
    
- **Identificación del atacante:** La identificación completa (nombre y apellido) es compleja y a menudo no se logra sin que el atacante cometa un error operativo (ej. reutilizar un seudónimo, dejar metadatos en un archivo, usar una cuenta bancaria poco segura para la transferencia). La solicitud de un giro postal o transferencia bancaria es un punto débil, ya que deja un rastro que puede ser investigado por las autoridades.
    

---

### 3. Medidas Preventivas

Para evitar futuros incidentes, se deben adoptar las siguientes medidas:

- **Técnicas:**
    
    - Implementar la **autenticación de múltiples factores (MFA)** en todos los accesos a correos y sistemas críticos.
        
    - Realizar **auditorías de seguridad** y pentesting periódicos.
        
    - Mantener todo el software y sistemas operativos **actualizados y parcheados**.
        
    - Utilizar un sistema de **filtrado de correo electrónico** avanzado para detectar phishing.
        
- **Organizativas:**
    
    - Desarrollar un **plan de respuesta a incidentes** claro y practicarlo.
        
    - Implementar el **principio de mínimo privilegio**, asegurando que los empleados solo tengan acceso a la información estrictamente necesaria para su función.
        
    - Ofrecer **formación continua en ciberseguridad** a todo el personal, enfocada en la detección de phishing e ingeniería social.