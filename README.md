# Consola
***

## Descripción
***

Este proyecto se basa en la creación de una consola, usando unicamente los lenguajes de HTML, CSS y JavaScript. Para este diseño se ha elegido una GameBoyColor,
con un diseño clásico.


## Código
***

### HTML

La parte del HTML se ha estructurado de forma en la que el cuerpo de la consola es el <div> principal y desde el sale el resto de composición de la consola como
se puede ver en el siguiente código:

...

<div class="cuerpo">
        <div class="detalleCuerpo"></div>
        <div class="letras">
            <span>GAME BOY</span>
            
        </div>
        <div class="letras2"><span style="color: palevioletred;">C</span><span></span><span style="color: blue;">O</span><span style="color: greenyellow;">L</span><span style="color: yellow;">O</span><span style="color:aquamarine;">R</span></div> 
        <div class="pantallaNegro">
            <div id="luz"></div>
            <div class="power">POWER</div>
        </div>
        <div text="" onclick="ChangeText" class="pantallaMain"></div>
        <button class="joistickT"></button>
        <button class="joistickL"></button>
        <button class="joistickR"></button>
        <button class="joistickB"></button>
        <div class="joistickM"></div>
        <button class="joistickI"></button>
        <input type="button"id="botonB"></input>
        <div class="b">B</div>
        <button class="botonA"></button>
        <div class="a">A</div>
        <button class="botonSelect" ></button>

        <button type="button"class="botonStart"></button>
        
        <div class="nintendo">NINTENDO</div>
        <div class="elipseN"></div>
        <div class="select">SELECT</div>
        <div class="start">START</div>
        
    </div>

...

En cuato a las letras principales de la consola:  GAMEBOY COLOR, se ha decidido hacer en el própio código HTML, para poder tener en una única línea el color,
que varía en cada letra, quitando peso al código CSS.

###CSS

El código CSS se ha estructurado igual que el de HTML, estando en el mismo órden cada apartado(Primero el cuerpo, segundo la pantalla...)para establecer un orden
a la hora de encontrar donde está cada parte de la consola siendo la estructura princpial el cuerpo de esta.

...

/*cuerpo de la consola*/
.cuerpo{
    position: absolute;
    display: flex;
    margin: 20px auto;
    margin-left: 4em;
    /*altura del cuerpo*/
    padding-bottom: 25em;
    /*redondeo de los bordes */
    border-bottom-left-radius: 3em;
    border-bottom-right-radius: 3em;
    border-top-left-radius: 1em;
    border-top-right-radius: 1em;
    z-index: 1;
    /*tamaño del cuerpo*/
    width: 25rem;
    weight: 50rem;
    padding-bottom: 43em;
    /*color principal*/
    background:rgb(27, 126, 109);   
    box-shadow: 10px 11px 0px -3px rgba(9,54,9,0.58),63px 26px 34px -3px rgba(0,0,0,0.58);
}

...


