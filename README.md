

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nacionalidade</title>
</head>
<body>
    <h1>Nacionalidade</h1>
    País: <input type="text" name="txtvel" id="txtvel">
    <input type="button" value="Verificar" onclick="nasc()">
    <div id="res">

    </div>
    <script>
    function nasc() {
        var txtv = window.document.querySelector('input#txtvel')
        var res = window.document.querySelector('div#res')
        var pais = txtv.value
        res.innerHTML = `<p>Seu país é <strong>${pais}</strong></p>`
        if (pais == 'Brasil') {
            res.innerHTML += '<strong>Brasileiro!</strong>'
        } else {
            res.innerHTML += '<strong>Estrangeiro!</strong>'
        }
    }
</script>
</body>
</html>
