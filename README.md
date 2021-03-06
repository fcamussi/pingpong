# Ping Pong

Juego de Ping Pong al estilo Atari™. Este programita lo hice hace muchos años para probar la técnica de double buffering para evitar el parpadeo cuando se dibujan objetos. Y ahora aproveché y le agregué la posibilidad de jugar contra la máquina ya que antes solo se podía jugar de a dos personas.

La técnica de double buffering es extremadamente sencilla, consiste en dibujar lo que se va a mostrar en pantalla en un buffer, y una vez dibujado por completo, se actualiza la pantalla copiando dicho buffer a la misma. También, al mantener la "última" pantalla en un buffer se puede redibujar la misma de forma inmediata, cuando por ejemplo, ésta es solapada por otra ventana y luego descubierta, sin tener que rehacer nuevamente los cálculos.

## Screenshots

![screenshot1](https://user-images.githubusercontent.com/75378876/178094319-9b7f31ef-7fe2-4ff7-8cf4-ed0a0ba9b61e.png)

![screenshot2](https://user-images.githubusercontent.com/75378876/178094318-58ad12de-1e54-45c4-b112-a3f35367377d.png)

## Requisitos

* gcc
* GTK+ 2

## Compilación

```
make
```

## Ejecución

```
./pingpong
```
