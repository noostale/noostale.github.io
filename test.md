---
layout: default
title: Test
---


<script>
    var x = 0;
    function func(){
        document.getElementById("numero").innerHTML = x ;
        x = x + 1;
    }
    
</script>

<button type="button" onclick='func()'>+</button>
<button type="button" onclick='func()'>-</button>
<p id="numero"></p>
