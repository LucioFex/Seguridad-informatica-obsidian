#clase_7 **Alumno**: Luciano Esteban

# Contenido
```table-of-contents
```

---
# Cifrado por desplazamiento
https://www.abcdatos.com/programa/practicas-criptografia-clasica.html

**Revisión del archivo descargable** (parece que es un falso positivo)
![[Pasted image 20250911230604.png]]
https://www.virustotal.com/gui/file/090378304d593c20191a1741b2365d1e31f69f28baacbfb43d8f9f9c2e9217d1/detection
## Ejercicio 1
1. Seleccionar “Opciones > Español Z27
2. Seleccionar “Criptosistemas > Desplazados Puros”.
![[Pasted image 20250911230732.png]]

3. Haga clic sobre el icono “Clave” y seleccione una Constante de desplazamiento igual a 3
(“Cifrado del César”)

![[Pasted image 20250911232334.png]]

4. En el cuadro “Entrada” escriba la siguiente frase: CURSO DE SEGURIDAD
![[Pasted image 20250911232409.png]]

5. Haga clic en “Cifrar”. Haga Click SI en “Quiere ver el informe”. Analice el informe.
![[Pasted image 20250911232508.png]]

6. Haga click en “Criptoanalizar”. Analice las frecuencias del alfabeto.
7. Copie la cadena de salida obtenida en el casillero correspondiente a “Entrada”.
8. Haga clic en “Descifrar”.
9. Haga Click Si en “Quiere ver el informe”. Analice el informe.
10. Como resultado del descifrado, usted podrá notar algunas diferencias respecto del texto
original, ¿Cuáles son?

FXUVRGHVHJXULGDG
![[Pasted image 20250911232917.png]]

10. Como resultado del descifrado, usted podrá notar algunas diferencias respecto del texto
original, ¿Cuáles son?

**A:** CURSO DE SEGURIDAD
**B:** CURSODESEGURIDAD

El texto es igual, pero sin espacios.
## Ejercicio 2
1. Haga clic sobre el icono “Clave” y seleccione una Constante de desplazamiento igual a 3 (“Cifrado del César”).
![[Pasted image 20250911233424.png]]

2. Redacte un texto breve utilizando el bloc de notas de Windows, grábelo como “prueba.txt”. (recuerde la ubicación del mismo)

Texto de prueba: **test_ej2.txt**
```md
And in the face of ignorance and resistance
I wrote financial systems into existence
And when my prayers to God were met with indifference
I picked up a pen, I wrote my own deliverance
```

3. Repita el ejercicio anterior seleccionando el ícono “Fichero entrada” y cague el archivo “prueba.txt”

![[Pasted image 20250911233959.png]]

4. Seleccione el ícono “Cifrar”. Haga Click Si en “Quiere ver el informe”. Analice el informe.
![[Pasted image 20250911234124.png]]

5. Copie el texto cifrado y guárdelo en un archivo de texto como “prueba.cif”.

**Prueba.cif.txt**
```md
DPGLPWKHIDFHRILJPRUDPFHDPGUHVLVWDPFHLZURWHILPDPFLDÑVBVWHOVLPWRHALVWHPFHDPGZKHPOBSUDBHUVWRJRGZHUHOHWZLWKLPGLIIHUHPFHLSLFNHGXSDSHPLZURWHOBRZPGHÑLYHUDPFH
```
6. Cierre el cuadro de dialogo
7. Seleccionar “Criptosistemas > Desplazados Puros”.
8. Haga clic sobre el icono “Clave” y seleccione una Constante de desplazamiento igual a 3
(“Cifrado del César”).
9. Haga clic sobre “Descifrar”.
10. Repita el ejercicio anterior seleccionando el ícono “Fichero entrada” y cague el archivo
“prueba.cif”
11. Analice el resultado.

![[Pasted image 20250911234339.png]]

El texto resultante es el mismo, pero sin espacios y todo en mayúsculas. Además, se eliminaron los saltos de línea.
```md
ANDINTHEFACEOFIGNORANCEANDRESISTANCEIWROTEFINANCIALSYSTEMSINTOEXISTENCEANDWHENMYPRAYERSTOGODWEREMETWITHINDIFFERENCEIPICKEDUPAPENIWROTEMYOWNDELIVERANCE
```

El texto separado semánticamente es el siguiente:
```md
and in the face of ignorance and resistance i wrote financial systems into existence and when my prayers to god were met with indifference i picked up a pen i wrote my own deliverance
```

---
## Cifrado por Vigenere

## Ejercicio 1
1. Seleccionar “Opciones > Español Z27
2. Seleccionar “Criptosistemas > Vigenere”.
![[Pasted image 20250911235623.png]]
3. Haga clic sobre el icono “Clave” y escriba una clave deseada
![[Pasted image 20250911235741.png]]
4. En el cuadro “Entrada” escriba la siguiente frase: CURSO DE SEGURIDAD
![[Pasted image 20250911235802.png]]
5. 5. Haga clic en “Cifrar”. Haga Click SI en “Quiere ver el informe”. Analice el informe.
6. Haga click en “Criptoanalizar”. ¿Qué mensaje aparece?
![[Pasted image 20250911235846.png]]

![[Pasted image 20250911235903.png]]
7. Copie la cadena de salida obtenida en el casillero correspondiente a “Entrada”.
8. Haga clic en “Descifrar”.
9. Haga Click Si en “Quiere ver el informe”.
10. Analice el informe.

ÑJEVDPKHPUHUWPGR --> CURSODESEGURIDAD

![[Pasted image 20250912000053.png]]

---
# Algoritmos simétricos de encriptado (DES) ATAQUE
## Revisión de archivos y programas

https://www.abcdatos.com/programa/ataque-fortaleza-estandar-des.html
![[Pasted image 20250912001151.png]]
![[Pasted image 20250912001201.png]]
https://www.reddit.com/r/antivirus/comments/1fuwx2z/trojanmalware300983susgen_its_bad/?tl=es-419

**Prueba para DES.txt**
![[Pasted image 20250921194933.png]]
**Prueba Cifrado.cif**
![[Pasted image 20250921194947.png]]

## Ejercicio 1: Ataque Monousuario
1. Descargue del campus los siguientes archivos: “Prueba para DES.txt” y “Prueba Cifrado.cif”
![[Pasted image 20250921195323.png]]
2. Ejecute la aplicación.
3. A continuación, seleccione “DES > Ataque > Monousuario” 
![[Pasted image 20250921195355.png]]
4. En la ventana “archivo” _ “Fichero Sin Cifrar” Ingrese el archivo “Prueba para DES.txt”
![[Pasted image 20250921195505.png]]
5. En la ventana “archivo” _ “Fichero Cifrado” Ingrese el archivo “Prueba Cifrado.cif”
![[Pasted image 20250921195511.png]]
6. Seleccione la solapa “Opciones > Búsqueda delimitada de claves”, seleccione “Hexadecimal”
![[Pasted image 20250921195624.png]]
7. En “Clave inicial” ingrese el siguiente valor “B4E0167A2467FAB1”, en “Clave Final” ingrese el
siguiente valor “F4E0167A2467FAB1”. (Debe aparecer en el casillero “Número de claves Distintas ”18014398509481985”)
![[Pasted image 20250921195702.png]]
8. En el casillero “Atacar” tilde la casilla “Archivos”
![[Pasted image 20250921195741.png]]
9. Inicie el proceso seleccionando “Operaciones” y luego “Comenzar”.
![[Pasted image 20250921195811.png]]
10. En la solapa “Resultado Ficheros” se podrá observar las claves válidas. (Copie y guarde el
resultado”)
![[Pasted image 20250921200902.png]]
![[Pasted image 20250921201553.png]]
Como podemos comprobar en la captura adjunta más arriba, el proceso es claramente tardado (como dirían en Telecom: "Tarda más que socializar una herramienta nueva") y no cuento con la disponibilidad horaria para completarlo en su totalidad.

En su lugar, adjuntaré el detalle teórico detrás de este ejercicio.
### Explicación teórica
El ataque monousuario en DES consiste en una búsqueda exhaustiva de claves (fuerza bruta) dentro de un rango específico. En el ejercicio se configuran la clave inicial y final en hexa, generando una búsqueda de 18.014.398.509.481.985 claves posibles.

El programa prueba cada clave una por una hasta encontrar la correcta. Esto es computacionalmente muy costoso porque:
- DES usa claves de 56 bits, eso significa que puede haber hasta 2^56 combinaciones posibles.  
	- Eso equivale a aproximadamente 72 cuatrillones de claves (7.2 × 10^16). Digamoslo así, probarlas todas llevaría muchísimo tiempo en una computadora común.
- Si la computadora prueba, por ejemplo, 1 millón de claves por segundo, el proceso podría tardar días o semanas en completarse.

# Ejercicio 2: Ataque simultaneo

Detalle de la CPU con la que realizaré el ejercicio:
![[Pasted image 20250921204910.png | 300]]

1. A continuación, seleccione “DES > Ataque > Red > Simulación” 
![[Pasted image 20250921201734.png]]
2. Repita todos los pasos de la operación anterior hasta el punto 8.
3. En el casillero “Nro de procesos atacando simultáneamente” coloque inicialmente “4”.(Repita el
proceso nuevamente asignando 6, 8 y 10)
![[Pasted image 20250921201843.png]]
4. Inicie el proceso seleccionando “Operaciones” y luego “Comenzar".
5. En la solapa “Resultado Ficheros” se podrá observar las claves válidas. (Copie y guarde el resultado”)


Con un número de procesos de ataque simultáneos en 4, tuvo un avance del 25% aproximadamente en 13 minutos.
![[Pasted image 20250921203242.png]]
![[Pasted image 20250921203321.png]]

Lo detuve por cuestiones de tiempo (el motivo es iden. Al mencionado en el ejercicio de Monousuario).

Prueba con 6 procesos:
![[Pasted image 20250921203722.png]]
Entre las claves válidas, se encuentran:
```bash
D4E0167A2466FAB0
D4E0167A2466FAB1
D4E0167A2466FBB0
D4E0167A2466FBB1
D4E0167A2467FAB0
D4E0167A2467FAB1
D4E0167A2467FBB0
D4E0167A2467FBB1
D4E0167A2566FAB0
D4E0167A2566FAB1
D4E0167A2566FBB0
D4E0167A2566FBB1
D4E0167A2567FAB0
D4E0167A2567FAB1
D4E0167A2567FBB0
D4E0167A2567FBB1
D4E0167B2466FAB0
D4E0167B2466FAB1
D4E0167B2466FBB0
D4E0167B2466FBB1
...
```

Prueba con 8 procesos:
![[Pasted image 20250921203826.png]]
Tiempos de carga muy extensos como vimos previamente.

Prueba con 10 procesos:
![[Pasted image 20250921203907.png]]
Tarda incluso menos que la muestra con 4 procesos.

Muestra de algunos outputs:
```bash
D4E0167A2466FAB0
D4E0167A2466FAB1
D4E0167A2466FBB0
D4E0167A2466FBB1
D4E0167A2467FAB0
D4E0167A2467FAB1
D4E0167A2467FBB0
```