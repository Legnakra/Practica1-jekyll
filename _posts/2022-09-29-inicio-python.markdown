---
layout: post
title:  "Introducción a la programación Python"
date:   2022-09-29 17:45:16 +0200
categories: python
---

## Ejercicio 1
Diseñar el algoritmo correspondiente a un programa que lea el valor correspondiente a una distancia en millas marinas y las escriba expresadas en metros.

### Análisis:
Problema: Tenemos que leer una cantidad de millas marinas y calcular su valor en metros.
Entrada: millas(entero).
Salida: metros (entero).
### Diseño:
    1. Leer distancia_millas (distancia_millas).
    2. Convertir millas marinas a metros (distancia_millas*1852).
    3. Mostrar el resultado.

~~~
1. Leer distancia_millas (distancia_millas).
distancia_millas = float(input("Distancia en millas marinas: "))

2. Convertir millas marinas a metros (distancia_millas*1852).
metros= distancia_millas*1852

3. Mostrar el resultado en metros.
print("La distancia en metros es de: ",metros, "metros")
~~~

## Ejercicio 2
Escribir un programa que pida al usuario su peso (en kg) y estatura (en metros), calcule el índice de masa corporal y lo almacene en una variable, e imprima por pantalla la frase “Tu índice de masa corporal es…” y el resultado.

### Análisis:
Problema: Tenemos que calcular el IMC (índice de masa corporal) dados el peso (kg) y la estatura (m).
Entrada: peso (entero), estatura (entero).
Salida: imc (entero).

### Diseño:
1.Leer peso (peso) y estatura (estatura).
2.Calcular el IMC (imc = peso/(estatura**2,2).
3.Mostrar el resultado.

~~~
1.Leer peso (peso) y estatura (estatura).

peso = input("¿Cuál es tu peso?(kg): ")
estatura = input("¿Cuál es tu estatura (metros): ")

2.Calcular el IMC (imc = peso/(estatura**2,2).
imc = round(float(peso)/float(estatura)**2,2)

3.Mostrar el resultado.
print("Tu índice de masa corporal es " + str(imc))
~~~

## Ejercicio 3
Una juguetería tiene mucho éxito en dos de sus productos: payasos y muñecas. Suele hacer venta por correo y la empresa de logística les cobra por peso de cada paquete así que deben calcular el peso de los payasos y muñecas que saldrán en cada paquete a demanda. Cada payaso pesa 112 g y cada muñeca 75 g. Escribir un programa que lea el número de payasos y muñecas vendidos en el último pedido y calcule el peso total del paquete que será enviado. Además se nos pide el precio que se cobra por gramo, , y se nos mostrará el total de dinero que necesitamos para realizar el envío.

### Análisis
Problema: Tenemos que calcular el peso del último pedido de payasos y muñecas, y el precio por gramo
al realizar el envío.
Entrada: payasos (real), muñecas (real), peso_payaso (real), peso_muñeca (real).
Salida:peso_total (real), precio_envío (entero).

### Diseño:
1.Leer cantidad de payasos (payasos)
2.Leer cantidad de muñecas (muñecas)
3.Calcular el peso del pedido (peso_total = peso_payaso*payaso + peso_muñeca*muñeca)
4.Leer el precio del envío por gramo.
5.Calcular precio del envío.
6.Mostrar el resultado.

~~~

peso_payaso = 112
peso_muñeca = 75

1.Leer cantidad de payasos (payasos)
payasos = int(input("Introduce el número de payasos a enviar: "))

2.Leer cantidad de muñecas (muñecas)
muñecas = int(input("Introduce el número de muñecas a enviar: "))

3.Calcular el peso del pedido (peso_total = peso_payaso*payaso + peso_muñeca*muñeca)
peso_total = peso_payaso * payasos + peso_muñeca * muñecas

4.Leer el precio del envío por gramo.
precio = float(input("El precio por gramo del envío es de: "))

5.Calcular precio del envío.
precio_envio = peso_total * precio

6.Mostrar el resultado.
print("El precio total del envío es de: ",precio_envio,"€." )
~~~

## Ejercicio 4
Diseñar el algoritmo correspondiente a un programa que pida el total de kilómetros recorridos, el precio de la gasolina (por litro), el consumo del coche (litros/100 km) y nos muestre la siguiente información:
*  El total de litros de gasolina que ha gastado en el trayecto.
* ¿Cuánto dinero te ha costado la gasolina?

### Análisis
Problema:Tenemos que calcular el consumo de un coche, el consumo en un recorrido con determinados kilómetros y el coste del trayecto.
Entrada:kilometros_recorridos (entero), precio_gasolina (entero), consumo_coche (entero).
Salida: total_litros (entero), consumo_gasolina (entero), gasto_gasolina (entero).

### Diseño
1.Leer kilómetros totales recorridos.
2.Leer precio gasolina.
3.Leer consumo del coche.
4.Calcular litros consumidos en el recorrido.
5.Calcular coste de gasolina en el recorrido.
6.Mostrar resultado.

~~~
1.Leer kilómetros totales recorridos.
kilometros_recorridos = float(input("Los kilómetros recorridos son: "))

2.Leer precio gasolina.
precio_gasolina = float(input("El precio de la gasolina (por litro) es: "))

3.Leer consumo del coche.
consumo_coche= float(input("El coche consume (litros/100km): "))

4.Calcular litros consumidos en el recorrido.
consumo_gasolina =consumo_coche / 100 * kilometros_recorridos
print("El coche ha gastado en ",kilometros_recorridos," un total de",consumo_gasolina,"litros de gasolina.")

5.Calcular coste de gasolina en el recorrido.
gasto_gasolina = consumo_gasolina*precio_gasolina

6.Mostrar resultado.
print("El gasto total de gasolina es de: ",gasto_gasolina,"€.")
~~~

# Ejercicio 5
Suponiendo que una paella se puede cocinar exclusivamente con arroz y gambas, y que para cada cuatro personas se utiliza medio kilo de arroz y un cuarto de kilo de gambas, escribir un programa que pida por pantalla el número de comensales para la paella, el precio por kilo de los ingredientes y muestre las cantidades de los ingredientes necesarios y el coste de la misma.

### Análisis
Problema:Te pide el número de comensales para calcular el precio por kilo de los ingredientes para una paella, muestre las cantidades y el coste de la misma.
Entrada: comensales (real), cantidad_arroz (entero), cantidad_gambas (entero), precio_gamba(entero),precio_arroz(entero).
Salida:coste_paella (entero).

### Diseño
1.Leer el número de comensales.
2.Calcular ingredientes necesarios para la paella.
3.Leer precios del arroz y las gambas.
4.Calcular el coste total de la paella.
5.Mostrar resultado.

~~~
1.Leer el número de comensales.
comensales = float(input("El número total de comensales es: "))

2.Calcular ingredientes necesarios para la paella.
cantidad_arroz= comensales* 0.5/4
cantidad_gambas=comensales* 0.25/4
print("Vamos a necesitar ",cantidad_arroz, "gramos de arroz.")
print("Vamos a necesitar ",cantidad_gambas, "gramos de gambas.")

3.Leer precios del arroz y las gambas.
precio_arroz= float(input("El precio del arroz(kg) es de: "))
precio_gamba= float(input("El precio de las gambas(kg) es de: "))

4.Calcular el coste total de la paella.
coste_paella= (cantidad_arroz*precio_arroz)+(cantidad_gambas*precio_gamba)

5.Mostrar resultado.
print("La paella cuesta: ",coste_paella, "€.")
~~~
