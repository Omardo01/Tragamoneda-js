# El juego de TRAGAMONEDA
El clasico juego de tragamoneda programado en html, css y js.
Que consiste en juego de azar, y probar tu suerte de manera divertida.

*Si deseas conocer mas del juego [visita aqui](https://es.wikipedia.org/wiki/M%C3%A1quinas_tragamonedas)*

# Vista general
El juego consiste en presionar el boton y esperara a tener la suerte de hacer coincidir las 3 imagenes.

![Captura de Pantalla 2022-02-23 a la(s) 10 02 48](https://user-images.githubusercontent.com/59854953/155357955-bef42bc5-dc9f-4ab6-a3d5-3842eb682687.png)

## Sobre el codigo
El juego esta programado con html, css y javascript. Los estilos son heredados del framework [Bootstrap](https://getbootstrap.com/).
Al momento de accionar el boton, la logica del programa crea 3 numeros aleatorios entre el 1 y el 3, mostrando en pantalla una imagen correspondiente a cada numero.
```
const aleatorio = (inferior, superior) => {
        let numPosibilidades = superior - inferior;
        let aleatorio = Math.random() * (numPosibilidades + 1);
        aleatorio = Math.floor(aleatorio);
        return inferior + aleatorio;
    };

let aleatorio1 = aleatorio(1,3);
```
![Captura de Pantalla 2022-02-23 a la(s) 10 08 08](https://user-images.githubusercontent.com/59854953/155358955-172cac5d-cae4-4137-9f09-a87a155e0a2f.png)

Existen 3 imagenes diferentes y el juego consiste en esperar a que tu suerte te permita tener la fortuna de coincidir las 3 imagenes.

## Ganando
Al momento de que coincides los 3 numeros o imagenes, se te muestra y el numero de intentos en los que ganaste el juego.
![Captura de Pantalla 2022-02-23 a la(s) 10 08 39](https://user-images.githubusercontent.com/59854953/155359108-509358a4-6c98-4564-8f5d-ff616e1b158d.png)

