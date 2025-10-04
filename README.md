<!doctype html>
.side{
max-width:300px; display:none; flex-direction:column; gap:12px; align-items:stretch;
}
.promo{background:linear-gradient(180deg,#071125 30%, rgba(255,255,255,0.01)); border-radius:12px; padding:16px; border:1px solid rgba(255,255,255,0.02)}
.promo h3{margin:0 0 6px 0}
.promo p{margin:0;color:var(--muted);font-size:13px}


/* RESPONSIVO */
@media (min-width:980px){
.wrap{align-items:flex-start}
.side{display:flex}
}


/* Prefer dark/light theme adjustments */
@media (prefers-color-scheme: light){
:root{--bg:#f7fafc; --card:#ffffff; --text:#0b1220; --muted:#475569; --accent:#60a5fa; --accent-2:#7dd3fc}
body{background:linear-gradient(180deg,var(--bg),#e6eef6 60%)}
}


/* Acessibilidade: aumentos de contraste */
@media (prefers-contrast: more){
:root{--card:#0b1220; --text:#ffffff}
.link-btn{border-color:rgba(255,255,255,0.07)}
}


/* Pequenas otimizações: imagens responsivas, fontes do sistema */
img{max-width:100%;height:auto;display:block}
</style>
</head>
<body>
<main class="wrap" aria-labelledby="page-title">


<section class="card" role="region" aria-label="Perfil e links">
<header>
<div class="avatar" aria-hidden="true">SM</div>
<div class="profile">
<h1 id="page-title">Seu Nome ou Marca</h1>
<p>Descrição curta — Especialista em X • Entregas rápidas</p>
</div>
</header>


<nav class="links" aria-label="Links afiliados">
<!-- Exemplo de item de link. Substitua href pelo seu link de afiliado. -->


<a class="link-btn" href="https://exemplo.com/afiliado1" target="_blank" rel="noopener noreferrer nofollow" aria-label="Abrir oferta X">
<span class="link-icon" aria-hidden="true">1</span>
<span class="link-text">
Oferta Imperdível
<span class="link-sub">Cupom: RIEK10 • Válido até 2026</span>
</span>
</a>


<a class="link-btn" href="https://exemplo.com/afiliado2" target="_blank" rel="noopener noreferrer nofollow" aria-label="Abrir curso Y">
<span class="link-icon" aria-hidden="true">🎓</span>
<span class="link-text">Curso Completo de Marketing
<span class="link-sub">Parcelamento em até 12x</span>
</span>
</a>


<a class="link-btn" href="https://exemplo.com/afiliado3" target="_blank" rel="noopener noreferrer nofollow" aria-label="Abrir produto Z">
<span class="link-icon" aria-hidden="true">🛒</span>
<span class="link-text">Kit Ferramentas Pro
<span class="link-sub">Frete grátis — Entrega 3-7 dias</span>
</span>
</a>


<!-- Dica: mantenha no máximo 6-9 links principais para não poluir a UX -->
</nav>


<p class="small">Links com * são links de afiliado. Ao comprar, você ajuda a manter o conteúdo. Obrigado!</p>
</section>


<aside class="side" aria-label="Promoções e informações">
<div class="promo" role="note">
<h3>Promoção do mês</h3>
<p>Use o cupom <strong>RIEK10</strong> para desconto em ofertas selecionadas.</p>
</div>


<div class="promo" role="note">
<h3>Integrações</h3>
<p>Adicione Google Analytics, pixel de afiliado ou UTM nas URLs para rastrear conversões.</p>
</div>
</aside>
</main>
