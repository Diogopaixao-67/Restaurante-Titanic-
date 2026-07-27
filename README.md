
<html lang="pt">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">

<title>Restaurante TITANIC</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">

<style>


.whatsapp{
    position:fixed;
    right:20px;
    bottom:20px;
    background:#25D366;
    color:#fff;
    width:60px;
    height:60px;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:30px;
    text-decoration:none;
}
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:#f5f5f5;
color:#333;
}

.menu{
background:#8B0000;
color:#fff;
display:flex;
justify-content:space-between;
align-items:center;
padding:15px 20px;
position:sticky;
top:0;
z-index:999;
box-shadow:0 3px 10px rgba(0,0,0,.2);
}

.logo{
font-size:22px;
font-weight:700;
}

.menu ul{
list-style:none;
display:flex;
gap:20px;
}

.menu a{
color:#fff;
text-decoration:none;
font-weight:600;
transition:.3s;
}

.menu a:hover{
color:#FFD700;
}

.header{
background:linear-gradient(135deg,#8B0000,#C62828);
color:#fff;
padding:50px 20px;
text-align:center;
}

.header h1{
font-size:34px;
margin-bottom:10px;
}

.header p{
font-size:18px;
}

.slider{
background:#fff3cd;
padding:15px;
overflow:hidden;
}

.slides{
position:relative;
height:55px;
}

.slide{
display:none;
text-align:center;
font-size:20px;
font-weight:700;
color:#c0392b;
animation:fade .8s;
}

.slide.ativo{
display:block;
}

@keyframes fade{
from{
opacity:0;
transform:translateY(20px);
}
to{
opacity:1;
transform:translateY(0);
}
}

.bemvindo{
padding:30px 20px;
text-align:center;
}

.bemvindo h2{
margin-bottom:10px;
color:#8B0000;
}

.produto{
display:flex;
justify-content:center;
padding:20px;
}

.card{
background:#fff;
max-width:420px;
width:100%;
border-radius:18px;
overflow:hidden;
box-shadow:0 8px 20px rgba(0,0,0,.15);
}

.card h2{
padding:20px;
text-align:center;
color:#8B0000;
}

.card img{
width:100%;
height:250px;
object-fit:cover;
}

.card p{
padding:20px;
line-height:1.7;
text-align:center;
}

.precos{
display:flex;
justify-content:center;
align-items:center;
gap:20px;
margin-bottom:20px;
}

.antigo{
text-decoration:line-through;
color:#888;
font-size:18px;
}

.novo{
font-size:30px;
font-weight:bold;
color:#e53935;
}

.btn{
display:block;
margin:0 20px 25px;
padding:16px;
background:#25D366;
color:#fff;
text-decoration:none;
text-align:center;
font-size:18px;
font-weight:bold;
border-radius:12px;
transition:.3s;
}

.btn:hover{
background:#128C7E;
}

.promocao{
padding:40px 20px;
}

.promocao h2{
text-align:center;
color:#8B0000;
margin-bottom:25px;
}

.promocoes{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:20px;
}

.promo{
background:#fff;
border-radius:15px;
overflow:hidden;
box-shadow:0 5px 15px rgba(0,0,0,.15);
transition:.3s;
}

.promo:hover{
transform:translateY(-8px);
}

.promo img{
width:100%;
height:180px;
object-fit:cover;
}

.promo h3{
padding:15px;
text-align:center;
color:#d32f2f;
font-size:28px;
}

footer{
background:#8B0000;
color:#fff;
text-align:center;
padding:20px;
margin-top:30px;
}

.modal{
display:none;
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:rgba(0,0,0,.6);
justify-content:center;
align-items:center;
padding:20px;
z-index:9999;
}

.modal-box{
background:#fff;
max-width:500px;
width:100%;
padding:30px;
border-radius:18px;
position:relative;
animation:fade .4s;
}

.modal-box h2{
color:#8B0000;
margin-bottom:15px;
}

.modal-box p{
margin-bottom:15px;
line-height:1.7;
}

.fechar{
position:absolute;
top:15px;
right:18px;
font-size:30px;
cursor:pointer;
font-weight:bold;
}

.fecharBtn{
background:#8B0000;
color:#fff;
border:none;
padding:12px 25px;
border-radius:8px;
cursor:pointer;
font-size:16px;
}

.fecharBtn:hover{
background:#B71C1C;
}

@media(max-width:768px){

.menu{
flex-direction:column;
gap:12px;
}

.menu ul{
flex-direction:column;
text-align:center;
}

.header h1{
font-size:28px;
}

.slide{
font-size:17px;
}

.card img{
height:220px;
}

.novo{
font-size:26px;
}

.btn{
font-size:17px;
}
}
</style>

</head>

<body>

<!-- MENU -->

<nav class="menu">

<div class="logo">
<i class="fas fa-utensils"></i>
Restaurante TITANIC
</div>

<ul>

<li><a href="#">Início</a></li>

<li>
<a href="#" id="sobreBtn">
Sobre Nós
</a>
</li>

</ul>

</nav>

<!-- HEADER -->

<header class="header">

<h1>Restaurante TITANIC</h1>

<p>
Oferecendo uma Experiência Gastronómica Única.
</p>

</header>

<!-- SLIDER -->

<section class="slider">

<div class="slides">

<div class="slide ativo">

<h2>
🔥 Restam poucas refeições disponíveis!
</h2>

</div>

<div class="slide">

<h2>
⚠ Promoção válida apenas hoje!
</h2>

</div>

<div class="slide">

<h2>
🍛 Faça já a sua encomenda!
</h2>

</div>

</div>

</section>

<!-- BOAS VINDAS -->

<section class="bemvindo">

<h2>
Bem-vindo ao portal de encomenda do Restaurante TITANIC
</h2>

<p>
Escolha o seu prato favorito e receba rapidamente.
</p>

</section>

<!-- CARD -->

<section class="produto">

<div class="card">

<h2>Arroz com Feijão</h2>

<img
src="https://github.com/Diogopaixao-67/Restaurante-Titanic-/Arroz com feijão.webp">

<p>

Delicioso arroz branco acompanhado de feijão preparado com ingredientes frescos.

</p>

<div class="precos">

<span class="antigo">
1.500 Kz
</span>

<span class="novo">
900 Kz
</span>

</div>

<a
href="https://wa.me/244941530467?text=Olá,%20quero%20encomendar%20Arroz%20com%20Feijão."
class="btn">

<i class="fab fa-whatsapp"></i>

Fazer Pedido

</a>

</div>

</section>

<!-- PROMOÇÕES -->

<section class="promocao">

<h2>

🔥 Promoção de 24 Horas

</h2>

<div class="promocoes">

<div class="promo">

<img
src="HTML/descarregar (3).webp">

<h3>500 Kz</h3>

</div>

<div class="promo">

<img
src="HTML/OIP (9).webp">

<h3>500 Kz</h3>

</div>

<div class="promo">

<img
src="HTML/descarregar (5).webp">

<h3>500 Kz</h3>

</div>

</div>

</section>

<!-- MODAL -->

<div class="modal" id="modal">

<div class="modal-box">

<span class="fechar">

&times;

</span>

<h2>

Sobre o Restaurante TITANIC

</h2>

<p>

O Restaurante TITANIC dedica-se à preparação de refeições de alta qualidade, utilizando ingredientes frescos e um atendimento rápido.

</p>

<p>

Nossa missão é oferecer comida saborosa, higiene, qualidade e entrega eficiente para todos os clientes.

</p>

<button class="fecharBtn">

Fechar

</button>

</div>

</div>
<a class="whatsapp"
href="https://wa.me/244941530467"
target="_blank">
💬
</a>
<footer>

© Restaurante TITANIC

</footer>

<script>
// ===============================
// SLIDER AUTOMÁTICO
// ===============================

const slides = document.querySelectorAll(".slide");
let indice = 0;

function trocarSlide() {

    slides.forEach(slide => {
        slide.classList.remove("ativo");
    });

    indice++;

    if (indice >= slides.length) {
        indice = 0;
    }

    slides[indice].classList.add("ativo");

}

setInterval(trocarSlide, 3000);


// ===============================
// MODAL SOBRE NÓS
// ===============================

const modal = document.getElementById("modal");
const abrir = document.getElementById("sobreBtn");
const fechar = document.querySelector(".fechar");
const fecharBtn = document.querySelector(".fecharBtn");

abrir.addEventListener("click", function(e){

    e.preventDefault();

    modal.style.display = "flex";

});

fechar.addEventListener("click", function(){

    modal.style.display = "none";

});

fecharBtn.addEventListener("click", function(){

    modal.style.display = "none";

});

window.addEventListener("click", function(e){

    if(e.target === modal){

        modal.style.display = "none";

    }

});


// ===============================
// ANIMAÇÃO DO BOTÃO
// ===============================

const botao = document.querySelector(".btn");

setInterval(function(){

    botao.style.transform = "scale(1.08)";

    setTimeout(function(){

        botao.style.transform = "scale(1)";

    },400);

},1800);


// ===============================
// MENSAGEM DE ESCASSEZ
// ===============================

const mensagens = [

"🔥 Restam poucas refeições disponíveis!",

"⚠ Mais de 20 pessoas encomendaram hoje.",

"🍛 Garanta já o seu prato antes que termine.",

"⏳ Promoção válida apenas por tempo limitado."

];

const slideTexto = document.querySelectorAll(".slide h2");

let msg = 0;

setInterval(function(){

    slideTexto[msg].innerHTML = mensagens[msg];

    msg++;

    if(msg >= mensagens.length){

        msg = 0;

    }

},3000);


// ===============================
// EFEITO NOS CARDS DAS PROMOÇÕES
// ===============================

const cards = document.querySelectorAll(".promo");

cards.forEach(function(card){

    card.addEventListener("mouseenter",function(){

        card.style.transform="scale(1.05)";

    });

    card.addEventListener("mouseleave",function(){

        card.style.transform="scale(1)";

    });

});


// ===============================
// ANO AUTOMÁTICO NO RODAPÉ
// ===============================

const footer = document.querySelector("footer");

footer.innerHTML =
"© " + new Date().getFullYear() + " Restaurante TITANIC - Todos os direitos reservados.";

</script>

</body>
</html>
