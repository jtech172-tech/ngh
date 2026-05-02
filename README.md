<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Loja Avon</title>
<style>
body {
    font-family: Arial;
    background: #f5f5f5;
    text-align: center;
}
.produto {
    background: white;
    padding: 15px;
    margin: 15px;
    border-radius: 10px;
}
button {
    background: #25D366;
    color: white;
    border: none;
    padding: 10px;
    border-radius: 5px;
}
img {
    width: 150px;
}
</style>
</head>
<body>

<h1>Maria Cosmetico</h1>

<div class="produto">
    <img src="https://via.placeholder.com/150">
    <h2>Perfume Avon</h2>
    <p>R$ 79,90</p>
    <button onclick="comprar('Perfume Avon - R$79,90')">Comprar</button>
</div>

<div class="produto">
    <img src="https://via.placeholder.com/150">
    <h2>Batom Avon</h2>
    <p>R$ 19,90</p>
    <button onclick="comprar('Batom Avon - R$19,90')">Comprar</button>
</div>

<script>
function comprar(produto) {
    let numero = "38 99194-5141"; // coloque seu WhatsApp
    let mensagem = `Olá! Quero comprar: ${produto}`;
    let url = `https://wa.me/${numero}?text=${encodeURIComponent(mensagem)}`;
    window.open(url, "_blank");
}
</script>

</body>
</html>

