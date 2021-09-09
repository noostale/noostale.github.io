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

    // OROLOGIO

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

<center>
<button type="button" onclick='piu()'>+</button>
<div id="numero">0</div>
<button type="button" onclick='meno()'>-</button>


<div id="orologio">0</div>
<button type="button" onclick='interval()'>START</button>
<button type="button" onclick='stop()'>STOP</button>
<button type="button" onclick='reset()'>RESET</button>
</center>