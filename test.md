---
layout: default
title: Test
---


<script>
    var x = 0;
    function piu(){
        document.getElementById("numero").innerHTML = x;
        x = x + 1;
    }
    function meno(){
        document.getElementById("numero").innerHTML = x;
        x = x - 1;
    }
</script>

<button type="button" onclick='piu()'>+</button>
<button type="button" onclick='meno()'>-</button>
<p id="numero">0</p>
