# HTML Introduction

HTML es un leguanje de etiquetas, sus siglas significan Hyper-Text Markup Language o en español 
Lenguaje de marcado de hipertexto

HTML es en si la base de todo sitio web, ya que con este se define una pagina web, su estructura e importancia.

Basicamente son etiquetas que el navegador interpreta para mostrar la informacion y que el usuario entienda que es lo que esta viendo.

La estructura basica seria la siguiente

`<Etiqueta>` contenido `</Etiqueta>`

Cada etiqueta tiene un nombre que lo identifica, El nombre de la etiqueta va dentro de los <> e indica que empieza la etiqueta, mientras que para indicar que se cierra se pode dentro del </>

A estas se les llaman etiqueta de apertura y de cierre respectivamente, y entre ambas va el contenido de la etiqueta.

Estas a su vez pueden tener otras etiquetas dentro siguiendo este patron (Para practicidad usaremos la palabra tag para nombrar cualquier etiqueta en los ejemplos de aqui en adelante):
`<tag><tag>`...`</tag></tag>`

Ademas, no necesariamente tienen que estar uno dentro de otro, pueden estar 2 dentro de un mismo elemento pero uno al lado del otro:
`<tag><tag>`...`</tag><tag>`...`</tag></tag>`

En este ejemplo se puede ver que esta dentro de que, pero cuando hay muchos elementos es un poco dificil de saber cual esta dentro de cual, como aqui:
`<tag><tag>`...`</tag><tag><tag><tag>`...`</tag><tag>...</tag></tag></tag></tag>`

Para poder tener una mejor representacion visual se indentan las etiquetas, indentar significa que los elemtos que esten dentro de otro se mueven a la derecha con 4 espacios o con un tab de distancia por lo general, de esta forma
```
<tag>
    <tag>...</tag>
</tag>
```

aun asi depende de como te guste verlo.
Usemos el mismo ejemplo anterior pero indentado

```
<tag>
    <tag>...</tag>
    <tag>
        <tag>
            <tag>...</tag>
            <tag>...</tag>
        </tag>
    </tag>
</tag>
```

De esta manera con solo ver se puede saber cual elemento esta dentro de cual y si se dan cuenta, cuando un elemento anida a otro, la etiqueta de cierre se encuentra directamente debajo de la de apertura, de esta forma es mas facil identificar si hace falta una etiqueta de cierre (Pasa mas de lo que deberia)

Cada etqueta tiene propiedades que se pueden asignar de la siguiente forma

`<tag propiedad="lo que quieres poner">...</tag>`

Cada etiqueta tiene propiedades unicas que veremos mas adelante.

Hasta ahora solo hemos visto como funcionan las etiquetas, pero como se hace una pagina web?
Como ya se habia mencionado antes las etiquetas son las que le dan sentido y ordern al sitio, por ende cada etiqueta, es unica y tiene un proposito, para poder entender esto veamos la estructura de una pagina web
Principalmente se inicia con la etiqueta <!DOCTYPE html>, la cual en si no es una etiqueta, es mas un indicador del tipo de archivo que el navegador  va a recibir

Toda pagina web tiene como etiqueta exterior la etiqueta html

`<html>`

dentro de ella definimos nuestra pagina. una pagina tiene 2 componentes, un header y un body, los cuales son
`<head>` y `<body>`

ya con estos 4 elementos podremos estructurar nuestra pagina, quedando de esta manera
```
<!DOCTYPE html>
<html>
    <head></head>
    <body></body>
</html>
```
Abre sample_1.html en este mismo documento, veras que tiene la misma estructura pero en el navegador no se ve nada, luego llenaremos esto

Vamos a sample_2.html, veras que tiene dentro de head otras etiquetas las cuales son `<meta>` y `<title>`
`<meta>` es una etiqeuta que sirve para dar informacion al navegador de como comportarse
y `<title>`, como su nombre indica, le da el titulo a la pagina
