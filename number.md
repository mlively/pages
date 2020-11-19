<div id="randomNumber" style="text-align: center; font-weight: bold; font-size: 20em; line-height: 1em"></div>
  
<script>
    var colors = {
        'white': 1,
        'red': 1,
        'orange': 1,
        'yellow': 1,
        'green': 0,
        'blue': 0,
        'mediumpurple': 1,
        'saddlebrown': 0, 
    };
    var randomNumberTo = function (maxNum) {
        return Math.ceil(Math.random() * maxNum);
    };

    var randomColor = function () {
        var colorNames = Object.keys(colors);
        var color = colorNames[Math.floor(Math.random() * colorNames.length)];
        return [ color, colors[color] ? 'black' : 'white' ];
    };

    var update = function () {
        document.getElementById("randomNumber").innerHTML = randomNumberTo(9);
        var colorPair = randomColor();
        document.body.style.backgroundColor = colorPair[0];
        document.body.style.color = colorPair[1];
    };

    update();

    window.setInterval(function () {
        update();
    }, 2000);

</script>
