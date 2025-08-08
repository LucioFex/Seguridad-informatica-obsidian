#clase_2 

# Contenido
```table-of-contents
```
---
# Descripción del incidente

![[Pasted image 20250807212850.png]]
# Cuestionario guía
![[Pasted image 20250807212839.png]]

---
# Texto remarcado
## Descripción del incidente:

En el <mark style="background: #FFF3A3A6;">2024</mark> se intentó atacar a una <mark style="background: #FFF3A3A6;">empresa de servicios financieros</mark> enviando <mark style="background: #ADCCFFA6;">correos electrónicos</mark> de <mark style="background: #ADCCFFA6;">phishing</mark> a varios <mark style="background: #FFF3A3A6;">empleados</mark>.  

Los <mark style="background: #ADCCFFA6;">correos parecían provenir del director financiero</mark> de la compañía y <mark style="background: #FFF3A3A6;">solicitaban a los empleados</mark> que <mark style="background: #BBFABBA6;">ingresaran sus credenciales en un sitio web</mark>, la que imitaba a la <mark style="background: #BBFABBA6;">página de inicio de sesión de la empresa</mark>.  

Además, una <mark style="background: #ADCCFFA6;">persona se hizo pasar por un proveedor habitual de la empresa de manufactur</mark><mark style="background: #ADCCFFA6;">a</mark> y <mark style="background: #ADCCFFA6;">envió un correo electrónico al departamento de cuentas</mark>, <mark style="background: #FFF3A3A6;">solicitando un cambio en la cuenta bancaria</mark> donde <mark style="background: #FFF3A3A6;">se realizaban los pagos.</mark>  

En un <mark style="background: #ADCCFFA6;">intento de infiltración</mark>, <mark style="background: #BBFABBA6;">también pudieron identificar y </mark><mark style="background: #BBFABBA6;">contactar a través de sus redes sociales a un</mark> <mark style="background: #FFF3A3A6;">empleado de la empresa tecnológica que trabajaba en dicha empresa</mark>. Luego, <mark style="background: #ADCCFFA6;">utilizaron la información publicada por el empleado para</mark> <mark style="background: #BBFABBA6;">crear un perfil falso y hacerse pasar por él</mark>.

# Flujo de acción

#### Técnicas utilizadas:
- Phishing - **Envío de correos electrónicos a empleados del banco.**
- Ingeniería Social
	- **Persona que se hizo pasar por un proveedor habitual.**
	- **Solicitud de cambio de cuenta bancaria.**
- Defacement del sitio web - **Página para las credenciales.**
- Usurpación de identidad - **Uso de la información en redes de un empleado para la creación de un perfil falso.**
#### Origen del ataque:
- No hay información directa que se puede obtener del origen físico, pero podría averiguarse mediante la trazabilidad de logs de direcciones de IP accedidas, los chats con el falso director financiero, entre otros.
	- Solo se menciona la infraestructura o tácticas de acceso a la información privilegiada, pero no a datos duros / particulares del incidente.
#### Vulnerabilidades
- Principalmente capa 8: El factor humano, mediante ingeniería social.
	- Esto se puede relacionar a la falta de capacitación de los empleados y de un exceso de confianza de los medios por los que reciben / envían información
- Hubo una falla grave en los protocolos al momento de realizar el cambio de cuenta bancaria  con el falso miembro del proveedor habitual de la empresa de manufactura (*departamento de cuentas*).
#### Descubrimiento
- Muy probablemente se descubrió el incidente en el momento en el que el proveedor original no recibió su pago, lo da un delta de tiempo desde que se realizó el cambio de cuenta hasta que se realizó el mismo.
	- Este delta de tiempo es un apertura que incluso pudo haber sido aprovechada más a fondo.
#### Medidas preventivas
- Es necesaria más capacitación de los miembros de los empleados sobre phishing e ingeniería social.
- Es necesario utilizar métodos de autentificación de doble factor en caso que no los haya.
- Uso de herramientas de monitoreo de base de datos (ej: Guardium) para enviar alertas en tiempo real de acciones y acceso anómalos.
- Redes sociales.
-