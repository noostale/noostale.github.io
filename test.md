---
layout: default
title: Test
---

<script>

    // CONTATORE
    
    var x = 0;
    
    function piu(){
        x = x + 1;
        document.getElementById("numero").innerHTML = x;
    }
    function meno(){
        x = x - 1;
        document.getElementById("numero").innerHTML = x;
    }

    // OROLOGIO pull

    var tempo = 0;

    function start() {
        tempo = tempo + 1;
        document.getElementById("orologio").innerHTML = tempo;
    }

    var interval;

    function stop() {
        clearInterval(interval);
    }

    function reset() {
        clearInterval(interval);
        tempo = 0;
        document.getElementById("orologio").innerHTML = tempo;
    }

    function interval() {
        clearInterval(interval);
        interval = setInterval(start, 1000);
    }

</script>


<button type="button" onclick='piu()'>+</button>
<p id="numero" style="font-size:25px">0</p>
<button type="button" onclick='meno()'>-</button>
<br>
<br>
<p id="orologio" style="font-size:25px">0</p>
<button type="button" onclick='interval()' >START</button>
<button type="button" onclick='stop()'>STOP</button>
<button type="button" onclick='reset()'>RESET</button>

<canvas id="canvas"></canvas>

<script>
const canvas = document.getElementById('canvas');
const ctx = canvas.getContext('2d');

ctx.fillStyle = 'green';
ctx.fillRect(10, 10, 150, 100);
</script>