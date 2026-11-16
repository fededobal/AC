# Arquitectura de Computadoras

Prácticas resueltas y repasos de parcial de Arquitectura de Computadoras (cursada 2024). Las prácticas 1 a 3 usan el simulador VonSim (`.asm`), y las 4 y 5, WinMIPS64 (`.s`). Más detalles en el [README de 2024](2024/README.md).

## Prácticas

### [Práctica 1](2024/Práctica%201/): E/S con interrupciones por software y subrutinas

- [Consigna](2024/Práctica%201/Practica%201%20-%20Subrutinas%20y%20Pila%20-%20Arquitectura%20de%20Computadoras.pdf)
- [P2Ej4PuntosABC.asm](2024/Práctica%201/P2Ej4PuntosABC.asm): imprime las letras de la A a la Z con `INT 7`.
- [P4Ej2PuntosABC.asm](2024/Práctica%201/P4Ej2PuntosABC.asm): subrutina que calcula A+B−C con pasaje de parámetros por registro.
- [repaso.asm](2024/Práctica%201/repaso.asm): ejercicios de repaso (contar apariciones de una letra en un mensaje, etc.).

### [Práctica 2](2024/Práctica%202/): E/S por consulta de estado (PIO y Handshake)

- [Consigna](2024/Práctica%202/Practica%202%20-%20ES%20e%20Interrupciones%20por%20Software%20-%20Arquitectura%20de%20Computadoras.docx.pdf)
- [Ej4b.asm](2024/Práctica%202/Ej4b.asm): imprime un mensaje en la impresora a través del PIO.
- [IMP_CADENA_HADSHAKE.asm](2024/Práctica%202/IMP_CADENA_HADSHAKE.asm): imprime un mensaje a través del Handshake por consulta de estado.
- [IMP_LECTURA_HS.asm](2024/Práctica%202/IMP_LECTURA_HS.asm): lee caracteres del teclado y los imprime por Handshake.
- [Ej5a.asm](2024/Práctica%202/Ej5a.asm): impresión por Handshake con subrutinas de polling e impresión de caracteres.

### [Práctica 3](2024/Práctica%203/): interrupciones por hardware (PIC, TIMER, F10, Handshake)

- [Consigna](2024/Práctica%203/Practica%203%20-%20Interrupciones%20por%20Hardware.pdf)
- [Parte2_5b.asm](2024/Práctica%203/Parte2_5b.asm) y [Parte2_5d.asm](2024/Práctica%203/Parte2_5d.asm): uso del TIMER para mostrar mensajes periódicamente.
- [Parte2_6a.asm](2024/Práctica%203/Parte2_6a.asm): cuenta regresiva desde un dígito ingresado, que arranca al presionar F10 y avanza con el TIMER.
- [Parte2_7a.asm](2024/Práctica%203/Parte2_7a.asm): impresión por Handshake mediante interrupciones.
- [Parte3_2](2024/Práctica%203/Parte3_2): cada F10 invierte el estado de las luces del PIO.

### [Práctica 4](2024/Práctica%204/): introducción a WinMIPS64, instrucciones y E/S

- [Consigna](2024/Práctica%204/Practica%204%20-%20Instrucciones%20y%20E_S.pdf)
- [Parte 1](2024/Práctica%204/Parte%201/): ejercicios de instrucciones (aritmética, recorrido de vectores, conteo en cadenas) y un [ejemplo integrador](2024/Práctica%204/Parte%201/ejemploIntegrador.s) con subrutina que pasa una cadena a mayúsculas.
- [Parte 2](2024/Práctica%204/Parte%202/): E/S con `CONTROL`/`DATA`: imprimir texto, números y vectores, sumas de enteros y flotantes, ingreso de clave ([2a](2024/Práctica%204/Parte%202/2a.s), [2b](2024/Práctica%204/Parte%202/2b.s), [2c](2024/Práctica%204/Parte%202/2c.s)) y pintado de píxeles y líneas en la pantalla gráfica.

### [Práctica 5](2024/Práctica%205/): convención de registros, pila y subrutinas (WinMIPS64)

- [Consigna](2024/Práctica%205/Practica%205%20-%20Convención,%20pila%20y%20subrutinas.pdf)
- [1f.s](2024/Práctica%205/1f.s): lee un exponente y suma 2ⁿ + 3ⁿ con una subrutina de potencia.
- [factorialRecursivo.s](2024/Práctica%205/factorialRecursivo.s): factorial con subrutina recursiva.
- [contarPalindromos.s](2024/Práctica%205/contarPalindromos.s): cuenta las palabras palíndromo de un texto.
- [ejercicioTipoParcial1.s](2024/Práctica%205/ejercicioTipoParcial1.s): ingreso validado de números y conteo de impares.
- [ejercicioTipoParcial2.s](2024/Práctica%205/ejercicioTipoParcial2.s): dibuja un patrón alternando rojo y azul en la pantalla gráfica.
- [listaFlotante.txt](2024/Práctica%205/listaFlotante.txt): apunte de las instrucciones de punto flotante.

## [Repasos de parcial](2024/Repasos/)

**VonSim (`.asm`)**

- `Punto3Parcial1` a `Punto3Parcial4` y `Punto3ParcialRecu`: subrutinas con pasaje por pila, PIO y E/S (p. ej. [Punto3Parcial2.asm](2024/Repasos/Punto3Parcial2.asm) cuenta pares e impares de un vector).
- [Punto4Parcial1.asm](2024/Repasos/Punto4Parcial1.asm): envía un mensaje a la impresora por PIO y termina con F10.
- [Punto4Parcial2.asm](2024/Repasos/Punto4Parcial2.asm) y [Punto4Parcial3.asm](2024/Repasos/Punto4Parcial3.asm): muestran valores en luces del PIO durante tiempos controlados por el TIMER.
- [Ejercicio8.asm](2024/Repasos/Ejercicio8.asm): imprime un mensaje carácter a carácter con el TIMER.

**WinMIPS64 (`.s`)**

- [parcial1.s](2024/Repasos/parcial1.s): grafica puntos en el promedio de cada par de valores.
- [parcial2.s](2024/Repasos/parcial2.s): grafica puntos en la diferencia de cada par de valores.
- [parcial3.s](2024/Repasos/parcial3.s): grafica los pares de coordenadas que están en rango.
- [parcial4.s](2024/Repasos/parcial4.s): grafica números con distinto color según sean pares o impares.
