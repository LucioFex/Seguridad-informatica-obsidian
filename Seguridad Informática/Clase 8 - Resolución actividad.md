#clase_8 


![[Caso de estudio 2 1.pdf]]


![[Pasted image 20250915000240.png]]

![[Pasted image 20250915000216.png]]

## “¿De dónde viene?” — Rutas de atribución (incluye **qué poner** como listas en cajas de Event 7)

**Hipótesis A — Origen interno (más alineada con “dejó un programa a las 19:00”):**

- _Indicadores a colocar:_ top talkers = IPs de LAN sucursales; timestamps = exacto 19:00; **Windows Event 4698/4699** (creación/eliminación de tarea), `C:\Windows\Tasks\*.job`, `HKLM\Software\Microsoft\Windows\CurrentVersion\Run`, servicios nuevos.
    
- _Conclusión en caja:_ “DoS **desde equipos internos** por tareas programadas desplegadas previamente”.
    

**Hipótesis B — Pivot vía **Proveedores** (abuso de RMM/VPN):**

- _Indicadores:_ logs de RMM con “job push” a múltiples hosts; autenticaciones exitosas desde IP del proveedor; cambios en horario laboral del proveedor cerca de 19:00; scripts idénticos firmados por cuenta de soporte.
    
- _Conclusión:_ “Intrusión a proveedor → despliegue masivo → DoS interno coordinado”.
    

**Hipótesis C — Botnet externa coordinada + “stager” interno mínimo:**

- _Indicadores:_ fuentes **miles de IPs públicas**/múltiples ASNs; proveedores ven ataques **entrantes** a su borde; en LAN hay un **triggger** ligero que ordena oleadas externas.
    
- _Conclusión:_ “Ataque mixto (externo botnet) con coordinación desde host comprometido”.
    

> **Regla práctica para tu diagrama (añade como nota):**
> 
> - Si ≥80% del tráfico ofensivo proviene de **rangos internos/VPN** → A o B.
>     
> - Si la mayoría es **IP pública diversa** y volumétrica → C.
>     
> - Si hay **jobs RMM/VPN** justo antes de 19:00 → B prima sobre A.
>