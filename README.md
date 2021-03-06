# ***Analizar y documenta los siguientes scripts de Powershell***

Practica Powershell. Sistemas informáticos  

## **Script 1**

Para comprender el funcionamiento del siguiente script vamos a añadir varios puntos de interupcion como se muestra a continuación: 

![Ejercicio 1.1](imagenes/ej11.png)

*(Los puntos rojos son los puntos de interrupción.)*

Conforme vayamos ejecutando el script, a una variable `$number` se le asigna el valor 1; luego se escribe en la pantalla mediante el cmdlet `Write-Host`. Luego, a la variable `$number` se le asigna el siguiente número en la secuencia y se muestra en la pantalla nuevamente, y esto se repite varias veces. 

A continuación se muesttra la ejecución del script:

![Ejercicio 1.2](imagenes/ej12.gif)

---

## **Script 2**

Añadimos los siguientes puntos de interrupción para ver el funcionamiento del siguiente script:

![Ejercicio 2.1](imagenes/ej21.png)

Y observamos la ejecucion del script: 

![Ejercicio 2.2](imagenes/ej22.gif)

---

## **Script 3**

El Script 3 tiene unos cuantos errores: 

```powershell
if ("HELLO" -match "H") {

    string "HELLO"
}

if ("HELLO" -notmatch "A") {
    string "HELLO"
}
```

`String` no se reconoce como nombre de la cmdlet. Dejando el código de la siguiente forma se podrá solucionar: 

```powershell
if ("HELLO" -match "H") {
    #H exists in the 
     "HELLO"
}
   
# -notmatch	Results in true when a string doesn't match a regex pattern.	
if ("HELLO" -notmatch "A") {
    #A does not match in the 
     "HELLO"
}
```

Así la ejecución del programa quedará de la siguiente forma: 

![Ejercicio 3](imagenes/ej3.gif)