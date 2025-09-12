#clase_7

# Contenido inicial

Falté, mis apuntes son con el material que adjuntó el profe.

Msj inicial: 
![[Pasted image 20250911224008.png]]

Material de la clase 
![[Pasted image 20250911224019.png]]
![[Pasted image 20250911224013.png]]

Mmm sospechoso el archivo descargado, pero parece que al final es un falso positivo.
![[Pasted image 20250911230604.png]]
https://www.virustotal.com/gui/file/090378304d593c20191a1741b2365d1e31f69f28baacbfb43d8f9f9c2e9217d1/detection

---
# Cifrado por desplazamiento
https://www.abcdatos.com/programa/practicas-criptografia-clasica.html
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
## Ejercicio 2:

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
https://www.abcdatos.com/programa/ataque-fortaleza-estandar-des.html
## Ejercicio 1: Ataque Monousuario
