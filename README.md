<head>
    <meta charset="UTF-8">
    <title>Formas</title>
    <link href="css/stils.css" rel="stylesheet" type="text/css">
</head>
<body>
    <h1>Formas un ievadlauku piemērs</h1>
    <form>
        <p>Šodienas datums <input name="datums"></p>
        <p>Ja gribi uzzināt šodienas datumu, spied pogu DATUMS 
            <input onclick="datums.value=new Date();" name="poga" value="DATUMS" type="button">
        </p>
        <p>Ja gribi izdzēst datuma lodziņa saturu, spied pogu RESET
            <input value="RESET" type="reset">
        </p>
    </form>
    <form>
        <p> Ievadi skaitli un uzzināsi kāds būs datums pēc tik dienām. </p>
        <div>skaitlis<input type="number" name="sk0"> </div>
        <div>
            <input value="spied šeit" name="poga" onclick="rez.value=sk0.value+datums.value=new Date();" type="button">
        </div>
        <div>Datums<input name="datums"> </div>
    </form>
    <form>
        <div>1.skaitlis<input type="number" name="sk1"> </div>
        <div>
            <input value="X" name="reiz" onclick="rez.value=sk1.value*sk2.value" type="button">
        </div>
        <div>
            <input value="+" name="plus" onclick="rez.value=sk1.value+sk2.value" type="button">
        </div>
        <div>
            <input value="-" name="mīnus" onclick="rez.value=sk1.value-sk2.value" type="button">
        </div>
        <div>
            <input value="/" name="dalīt" onclick="rez.value=sk1.value/sk2.value" type="button">
        </div>
        <div>2.skaitlis<input type="number" name="sk2"> </div>
        <hr>
        <div>Rezultāts<input name="rez"> </div>
        <p>Ja gribi izdzēst lodziņu saturu, spied pogu RESET
            <input value="RESET" type="reset">
        </p>
    </form>
</body>

<head>
    <meta charset="UTF-8">
    <script>
    function krasot(){
        var kr=document.getElementById("krasa").value;
        document.getElementById("fons").style="background-color:"+kr;
        document.getElementById("fons").innerText = "Krāsa nomainīta!";
    }
    </script>
</head>
<body>
     <form>
  <div id="fons" style="background-color:lightgrey">Izvēlies krāsu!</div>
  <input type="color" id="krasa" value="#00ff00" onclick="krasot();">
</form>
</body>
