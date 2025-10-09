#clase_12 | Luciano Esteban | Seguridad Informática | ININF 2025 | UCEMA

# Respuesta a preguntas

**1) ¿Después de dar el “enter” una vez instalado la clave en el servidor, qué puede ver que**
**sucedió ahora?**
	Tras instalar la clave y volver a entrar: login sin password (se ve Accepted publickey en auth.log)

**2) ¿Cómo tenía que loguearse antes de instalar SSH?**
	Antes: usuario+password por SSH.

**3) En el cliente ejecutar el comando:  `ls - la`**
**¿Qué es lo que puede ver ahora?**
	ls -la en el cliente: veo ~/.ssh/ con id_rsa, id_rsa.pub, known_hosts, etc.

**4) En el cliente ejecute el siguiente comando: `mkdir Prueba`**
**Ahora vaya al servidor y ejecute el comando: `ls -la**`
**¿Qué puede ver que sucedió en el servidor?**
	mkdir Prueba en el cliente → en el servidor no cambia nada (FS distinto).

**5) En el cliente ejecute el siguiente comando: `rmdir Prueba`
Ahora vaya al servidor y ejecute el comando: `ls -la`
¿Qué puede ver que sucedió en el servidor?**
	rmdir Prueba en el cliente → en el servidor sigue igual.
	

**6) Compruebe que la conexión con el cliente está cerrada**
**Sino cierre la conexión desde el cliente.**
```
exit
```
**Debe verse que la conexión se detuvo.**
```
logout
connection to xxx.xxx.xxx.xxx closed
```
**Ahora desde el servidor intente conectarse al cliente.**
```
ssh (Nombre_Servidor)@xxx.xxx.xxx.xxx -p 443
```
**Dar enter**
**¿Pudo conectarse?**
**¿Las conexiones son bidireccionales?**
	Cierro con exit --> Connection closed.
	Desde el server a Kali por 443 no entra (Kali no tiene sshd en 443 por defecto).
	Conexión no bidireccional salvo que habilite openssh-server también en Kali.

---

# Procedimiento en el TP
- Pantalla clara: Servidor Debian
- Pantalla oscura: Cliente Kali

Datos alumno

![[Pasted image 20251009193313.png]]

![[Pasted image 20251009193348.png]]
changeme - password

---
ufw en 443
![[Pasted image 20251009193625.png]]

---

ip address debian:
![[Pasted image 20251009195319.png]]

---

ip address kali:
![[Pasted image 20251009195445.png]]

---

![[Pasted image 20251009195724.png]]

---

![[Pasted image 20251009200942.png]]



---


![[Pasted image 20251009201138.png]]

![[Pasted image 20251009201328.png]]

---

Generación de clave en cliente:

![[Pasted image 20251009201457.png]]

![[Pasted image 20251009201518.png]]


![[Pasted image 20251009201742.png]]

```
└─$ cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQC006nax1DIkZNebyAU3NHEBAddnGaWcQm+BjwLpDGE+aF98nSeb0IM6iuS1dA7wQN5V5CxaSPA9hT7sq4/IZG+Rkb4enZ/FSzeSly/fHVY3ixsnRxjYO6L+sXo6OqANIMdGdBzZophPfDPI+1E2eyfVKL5FS0N123iNYCGIvw9d8nAi4HMzUIDPJQiLSc+bPUXEAINT59TJpBBUasT39xFCeqU/GIwnvr37KybZ64YivVsFnQCiZuFtLkA6YwxeEMLr/fpgDVIz3x2aDu4sp/TDQaLC1bW+W5UFD1sVzFh1p8uu/N+K3XQo+X9ZQmF9ndloULEV896S0aYvT1gw0C/cvFJ3e2dDsQMBUMvZdEcSpiw6pLZXzI7fenaZNVIH6p/v8NXaS36nv95l2tWBCHhRGHcD4BX+lBPJQJzRJ6b2TYb28zxlua2p/0WDBJsNb88lao83gkSvVzAnGCSrt6YU2fxCAlDgvvZonyUstXTt838OUzAtvFzdk5a2URI2GDUnjPTzi0nw/ZxQksC8TGOzY+vuibZp5YDuwwRDCCDPNk+sKKDlqQkaU8xoer0hZHdZnyiMngC8LX17e93Gt6xiof/5fYUYdO9fudmtv8ALaxBC4+Uyj3YolFnSXacGEtzrfUkk018KdSlCS6worW+MpbNVWY5H0w6QgD9yp5s6w== alumno@kali
```

---

![[Pasted image 20251009201925.png]]
![[Pasted image 20251009202543.png]]

#### Desde Kali (Cliente)
Conexión sin clave:
![[Pasted image 20251009202620.png]]

