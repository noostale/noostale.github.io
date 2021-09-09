---
layout: default
title: Test
---


<script>
    var x = 0;
    function piu(){
        x = x + 1;
        document.getElementById("numero").innerHTML = x;
    }
    function meno(){
        x = x - 1;
        document.getElementById("numero").innerHTML = x;
    }
</script>

<button type="button" onclick='piu()'>+</button>
<button type="button" onclick='meno()'>-</button>
<p id="numero">0</p>
