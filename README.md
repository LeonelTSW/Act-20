# Act-20
# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Leonel Zapata Angulo
---

**DOCUMENTACIÓN DE OPERACIONES MATRICIALES APLICADAS A IMÁGENES EN Google Sheets**

##  Archivo trabajado:

`Matrices.xlsx`

---

##  **1. Objetivo**

El objetivo de este documento es explicar paso a paso el proceso de programación y aplicación de fórmulas en Microsoft Excel para manipular imágenes representadas como matrices numéricas de **30×30 píxeles**, aplicando conceptos básicos del álgebra matricial:

* Trasposición de matrices
* Multiplicación escalar
* Suma de matrices
* Resta de matrices
* Composición 

---

##  **2. Estructura del Archivo**

El archivo contiene **14 hojas**, divididas en:

* **5 hojas base:** imágenes originales en forma de matriz
* **5 hojas derivadas:** transpuestas de cada imagen
* **4 hojas de operaciones:** suma, resta, multiplicación escalar y composición 

La estructura general es la siguiente:


imagen 1

<img width="598" height="512" alt="image" src="https://github.com/user-attachments/assets/ba86c45e-10c3-4bf8-9252-ff1449fdf93d" />

Transpuesta 1

<img width="694" height="590" alt="image" src="https://github.com/user-attachments/assets/ddf83f4d-4343-4402-9c0a-1395d0c6e4a3" />

imagen 2

<img width="597" height="473" alt="image" src="https://github.com/user-attachments/assets/0e057997-7619-40a8-8150-a9d5d5ffd725" />

Transpuesta 2

<img width="653" height="587" alt="image" src="https://github.com/user-attachments/assets/44251e5d-9610-44bb-8f0f-469d29a56695" />

Imagen 3

<img width="597" height="605" alt="image" src="https://github.com/user-attachments/assets/b648a939-93d8-4d20-8292-a7331a522bfd" />

Transpuesta 3

<img width="654" height="565" alt="image" src="https://github.com/user-attachments/assets/2724bf4c-1bf3-45fb-a510-12724f659298" />

imagen 4

<img width="598" height="567" alt="image" src="https://github.com/user-attachments/assets/bec00d63-386f-4978-804c-04a70e6d649a" />

Transpuesta 4

<img width="635" height="560" alt="image" src="https://github.com/user-attachments/assets/9f91e259-9d41-4b7f-803f-6be92a516339" />

imagen 5

<img width="599" height="549" alt="image" src="https://github.com/user-attachments/assets/f409d426-45fc-4bd3-be70-e7f950cb1f68" />

Transpuesta 5

<img width="732" height="570" alt="image" src="https://github.com/user-attachments/assets/f1676772-1fab-4cf8-9c31-0860062174a0" />

Suma

<img width="599" height="588" alt="image" src="https://github.com/user-attachments/assets/d838deb3-f7f2-4f18-9b3a-7c3c12e73cdf" />

Resta

<img width="597" height="587" alt="image" src="https://github.com/user-attachments/assets/5815cb7c-0534-4602-b44e-277889e1bdd5" />

Multiplicacion Escalar

<img width="596" height="587" alt="image" src="https://github.com/user-attachments/assets/7b0cecef-7353-4549-9e25-508b5573113a" />

Composicion 

<img width="598" height="589" alt="image" src="https://github.com/user-attachments/assets/f35bf22d-caa1-4a44-a2e5-7e83265d992f" />

---

##  **3. Documentación de las Hojas Base**

## ##  **3.1 Imágenes Originales**

Cada una contiene una **matriz 30×30** correspondiente a una imagen pixelada.
Cada celda contiene un valor (0, 1 o 2) que representa un color o intensidad.
Estas matrices servirán como base para todas las operaciones posteriores.

---

##  **4. Documentación de Matrices Transpuestas**

## ##  **4.1 Definición Matemática**

La traspuesta de una matriz ( A ) se define como:

Intercambia filas por columnas.

## ##  **4.2 Fórmula usada en Google Sheets**

```
=TRANSPONER('imagen X'!A1:AD30)
```

**Instrucciones:**

1. Seleccionar un rango 30×30 vacío.
2. Escribir la fórmula.
3. Confirmar con Ctrl
4. Excel generará automáticamente la matriz traspuesta.

---

##  **5. Operaciones Matriciales**

Estas operaciones se encuentran en las siguientes hojas, aqui es donde realizamos las operaciones con dos imagenes que creamos:

* `Suma`
* `Resta`
* `Multiplicacion Escalar`
* `Composicion` 

La fórmula se arrastra hasta cubrir la matriz completa.

---

##  **5.2 Suma de Matrices**

### Fórmula en Google Sheets

Ejemplo sumando `imagen 1` + `imagen 2`:

```
='imagen 1'!A1 + 'imagen 2'!A1
```

Se arrastra sobre 30×30 celdas.

---

##  **5.3 Resta de Matrices**

###  Fórmula en Google Sheets

Ejemplo restando `imagen 1` - `imagen 2`:

```
='imagen 1'!A1 - 'imagen 2'!A1
```

También se arrastra sobre la matriz completa.

---

---

##  **5.1 Multiplicación Escalar**

### Fórmula en Google Sheets

Si el escalar ( k ) está en la celda `B1` y la matriz base es `imagen 1`, entonces en `A1` colocamos:

```
='imagen 1'!A1 * $B$1
```


 ## **5.4 Composición Lineal**
 
###  Fórmula en Google Sheets

```
=IF('Imagen2'!A1<>"";'Imagen2'!A1;'Imagen1'!A1)

```

Arrastrar la fórmula hasta completar 30 filas × 30 columnas.

---
