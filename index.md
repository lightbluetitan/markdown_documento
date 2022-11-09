---
title: "Sintaxis Básica Markdown"
subtitle: "Markdown - RMarkdown - Quarto"
author: "Renzo Cáceres Rossi"
date: "2022/11/09"
output:
  html_document:
    code_download: TRUE
    css: "style_001.css"
---

<!-- Añadir comentarios a nuestro documento Markdown - HTML tags -->


## Encabezados - Títulos

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5

Título 1
---------

Título 2
=========


## Negrita - Cursiva - Tachado - Subrayado


**Texto formateado como Negrita**

*Texto formateado como Cursiva*

***Texto formateado como Negrita y Cursiva***

~~Texto tachado~~


<u>Texto subrayado</u> <!-- HTML tags -->


## Enlaces - Añadir links a nuestro documento Markdown


<https://www.facebook.com/iise.utec/>{target=_blank}

[IISE - UTEC](https://www.facebook.com/iise.utec/){target=_blank}

[IISE - UTEC](https://www.facebook.com/iise.utec/ "Ingresa al IISE UTEC"){target=_blank}


## Imágenes - Añadir imágenes a nuestro documento Markdown

<center>

![](logo_r.png)

![](logo_quarto.png)

</center>

## Código - Añadir código de distintos lenguajes de programación


    summary(mtcars)
    
La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.


```R
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)


```

```Python

import matplotlib.pyplot as plt
 

eje_x = ['Python', 'R', 'Node.js', 'PHP']
 

eje_y = [50,20,35,47]
 

plt.bar(eje_x, eje_y)
 

plt.ylabel('Cantidad de usuarios')
 

plt.xlabel('Lenguajes de programación')
 

plt.title('Usuarios de lenguajes de programación')
 

plt.show()


```

    SELECT id_usuario,usuario_nombre,usuario_apellidos FROM usuarios;


```sql

USE Northwind;

SELECT * FROM Products;


```

