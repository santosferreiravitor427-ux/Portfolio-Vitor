

<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="style.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

</head>

<body>

<nav style="align-items: center;">
<a href="#sobre">Sobre</a>
<a href="#skills">Skills</a>
<a href="#projetos">Projetos</a>
<a href="#contato">Contato</a>
</nav>

<div class="hero">

<img src="vitor.jpeg">

<h1>Olá, eu sou <span>Vitor Santos</span></h1>

<a href="#projetos" class="btn">Ver Projetos</a>

</div>

<section id="sobre" class="hidden">
<h2>Sobre mim</h2>

<p class="sobre">
Sou estudante de Análise e Desenvolvimento de Sistemas, atualmente no <strong>3º semestre</strong>, com foco em desenvolvimento web.

Tenho como objetivo conquistar minha primeira oportunidade de estágio na área de tecnologia, onde eu possa aplicar meus conhecimentos, evoluir tecnicamente e contribuir com soluções eficientes.

Sou dedicado, tenho facilidade em aprender novas tecnologias e gosto de resolver problemas através da programação.
</p>

</section>

<section id="skills" class="hidden">
<h2>Skills</h2>

<div class="skills">
<div class="skill">HTML</div>
<div class="skill">CSS</div>
<div class="skill">JavaScript</div>
<div class="skill">Git</div>
<div class="skill">GitHub</div>
<div class="skill">Redes</div>
</div>

</section>

<section id="projetos" class="hidden">
<h2>Projetos</h2>

<div class="projetos">

<div class="card">

<h3>Calculadora Web</h3>

<p>Aplicação desenvolvida com JavaScript para prática de lógica de programação.</p>

<a class="btn" href="https://santosferreiravitor427-ux.github.io/calculadora-js/" target="_blank">
Ver Projeto
</a>
</div>

<div class="card">

<h3>Portfólio Profissional</h3>

<p>Site desenvolvido para apresentar minhas habilidades e projetos.</p>

<a class="btn" href="#">
Ver Projeto
</a>
</div>

</div>
</section>

<section id="contato" class="hidden">
<h2>Contato</h2>

<div class="contato">

<a href="mailto:santosvitos259@gmail.com">
<i class="fa-solid fa-envelope"></i> Email
</a>

<a href="https://www.linkedin.com/" target="_blank">
<i class="fa-brands fa-linkedin"></i> LinkedIn
</a>

<a href="https://github.com/" target="_blank">
<i class="fa-brands fa-github"></i> GitHub
</a>

<a href="https://wa.me/qr/K4EWE4LUH5UIE1" target="_blank">
<i class="fa-brands fa-whatsapp"></i> WhatsApp
</a>

</div>

<footer>
<p>©️ 2026 - Vitor Santos</p>
</footer>

</section>

<script>

const text = "Desenvolvedor em formação | Buscando estágio na área de TI";
let i = 0;

function typing(){
if(i < text.length){
document.getElementById("typing").innerHTML += text.charAt(i);
i++;
setTimeout(typing, 50);
}
}
typing();

const elements = document.querySelectorAll('.hidden');

const observer = new IntersectionObserver(entries => {
entries.forEach(entry => {
if(entry.isIntersecting){
entry.target.classList.add('show');
}
});
});

elements.forEach(el => observer.observe(el));

</script>

</body>
</html>
