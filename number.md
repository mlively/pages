<div id="randomNumber" style="text-align: center; font-weight: bold; font-size: 20em; line-height: 1em"></div>
 
<script>
    var randomNumberTo = function (maxNum) {
        return Math.ceil(Math.random() * maxNum);
    };
    document.getElementById("randomNumber").innerHTML = randomNumberTo(9);
    window.setInterval(function () {
        document.getElementById("randomNumber").innerHTML = randomNumberTo(9);
    }, 10000);
</script>
