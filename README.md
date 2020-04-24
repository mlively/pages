<div id="randomNumber" style="text-align: center; font-weight: bold; font-size: 20em"></div>
 
<script>
    window.setInterval(function () {
        document.getElementById("randomNumber").innerHTML = Math.floor(Math.random() * 10) ;
    }, 10000);
</script>
