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

    function stop() {
        clearInterval(Interval);
    }

    function reset() {
        clearInterval(Interval);
        tempo = 0;
    }

    var interval;

    function interval() {
        interval = setInterval(start, 1000);
    }

</script>

<button type="button" onclick='piu()'>+</button>
<p id="numero">0</p>
<button type="button" onclick='meno()'>-</button>


<p id="orologio">00</p>
<button type="button" onclick='interval()'>START</button>
<button type="button" onclick='piu()'>STOP</button>
<button type="button" onclick='piu()'>RESET</button>

