# Arctus.com.br
Index.html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Arctus Imóveis — apartamentos novos e lançamentos imobiliários.">
  <title>Arctus Imóveis | Apartamentos Novos</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      color: #172033;
      background: #f6f7f9;
    }

    header {
      background: #0d1b2a;
      color: white;
      padding: 18px 6%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .logo {
      font-size: 27px;
      font-weight: bold;
      letter-spacing: 1px;
    }

    .logo span {
      color: #d4a84f;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
    }

    .hero {
      min-height: 520px;
      padding: 80px 6%;
      display: flex;
      align-items: center;
      color: white;
      background:
        linear-gradient(rgba(7,18,30,.72), rgba(7,18,30,.72)),
        url("https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=1800&q=80")
        center/cover;
    }

    .hero-content {
      max-width: 700px;
    }

    .hero h1 {
      font-size: clamp(40px, 7vw, 68px);
      line-height: 1.05;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 19px;
      margin-bottom: 30px;
      color: #e5e7eb;
    }

    .button {
      display: inline-block;
      background: #d4a84f;
      color: #111827;
      padding: 14px 24px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      border: none;
      cursor: pointer;
    }

    .search-box {
      width: 90%;
      max-width: 1100px;
      margin: -40px auto 60px;
      background: white;
      padding: 25px;
      border-radius: 14px;
      box-shadow: 0 10px 35px rgba(0,0,0,.12);
      position: relative;
    }

    .search-box h2 {
      margin-bottom: 18px;
    }

    .filters {
      display: grid;
      grid-template-columns: repeat(4, 1fr) auto;
      gap: 12px;
    }

    select,
    input {
      width: 100%;
      padding: 13px;
      border: 1px solid #d5d9df;
      border-radius: 7px;
      font-size: 15px;
      background: white;
    }

    .section {
      width: 90%;
      max-width: 1200px;
      margin: 0 auto 70px;
    }

    .section-title {
      margin-bottom: 25px;
    }

    .section-title h2 {
      font-size: 34px;
      margin-bottom: 5px;
    }

    .section-title p {
      color: #667085;
    }

    .properties {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .property {
      background: white;
      border-radius: 14px;
      overflow: hidden;
      box-shadow: 0 5px 20px rgba(0,0,0,.08);
    }

    .property img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }

    .property-info {
      padding: 20px;
    }

    .property-info h3 {
      margin-bottom: 8px;
      font-size: 21px;
    }

    .location {
      color: #667085;
      margin-bottom: 14px;
    }

    .details {
      display: flex;
      gap: 12px;
      color: #475467;
      font-size: 14px;
      margin-bottom: 18px;
      flex-wrap: wrap;
    }

    .price {
      font-size: 23px;
      font-weight: bold;
      margin-bottom: 15px;
    }

    .about {
      background: #0d1b2a;
      color: white;
      padding: 70px 6%;
    }

    .about-content {
      max-width: 1100px;
      margin: auto;
    }

    .about h2 {
      font-size: 38px;
      margin-bottom: 18px;
    }

    .about p {
      color: #d1d5db;
      font-size: 17px;
    }

    .contact {
      padding: 70px 6%;
      text-align: center;
      background: white;
    }

    .contact h2 {
      font-size: 36px;
      margin-bottom: 12px;
    }

    .contact p {
      color: #667085;
      margin-bottom: 25px;
    }

    footer {
      background: #07121e;
      color: #9ca3af;
      text-align: center;
      padding: 25px;
    }

    .whatsapp {
      position: fixed;
      right: 20px;
      bottom: 20px;
      width: 58px;
      height: 58px;
      border-radius: 50%;
      background: #25d366;
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      text-decoration: none;
      font-size: 25px;
      z-index: 20;
    }

    @media (max-width: 900px) {
      .filters {
        grid-template-columns: 1fr 1fr;
      }

      .properties {
        grid-template-columns: 1fr 1fr;
      }
    }

    @media (max-width: 600px) {
      nav {
        display: none;
      }

      .filters,
      .properties {
        grid-template-columns: 1fr;
      }

      .hero h1 {
        font-size: 43px;
      }
    }
  </style>
</head>

<body>

<header>
  <div class="logo">ARCTUS<span>.</span></div>

  <nav>
    <a href="#imoveis">Imóveis</a>
    <a href="#sobre">Sobre</a>
    <a href="#contato">Contato</a>
  </nav>
</header>

<section class="hero">
  <div class="hero-content">
    <h1>Seu novo apartamento começa aqui.</h1>

    <p>
      Encontre apartamentos novos e lançamentos selecionados pela Arctus Imóveis.
    </p>

    <a href="#imoveis" class="button">Ver apartamentos</a>
  </div>
</section>

<section class="search-box">
  <h2>Encontre seu imóvel</h2>

  <div class="filters">
    <select id="quartos">
      <option value="">Quartos</option>
      <option value="1">1 quarto</option>
      <option value="2">2 quartos</option>
      <option value="3">3 quartos</option>
      <option value="4">4+ quartos</option>
    </select>

    <input id="localizacao" type="text" placeholder="Cidade ou bairro">

    <select id="preco">
      <option value="">Faixa de preço</option>
      <option value="300000">Até R$ 300 mil</option>
      <option value="500000">Até R$ 500 mil</option>
      <option value="800000">Até R$ 800 mil</option>
      <option value="1000000">Até R$ 1 milhão</option>
    </select>

    <div></div>

    <button class="button" onclick="buscarImoveis()">Buscar</button>
  </div>
</section>

<section class="section" id="imoveis">

  <div class="section-title">
    <h2>Apartamentos em destaque</h2>
    <p>Confira nossos imóveis selecionados.</p>
  </div>

  <div class="properties">

    <article class="property" data-preco="450000" data-quartos="2">
      <img
        src="https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=900&q=80"
        alt="Apartamento moderno">
      <div class="property-info">
        <h3>Residencial Arctus Prime</h3>
        <p class="location">São Paulo • Vila Mariana</p>

        <div class="details">
          <span>🛏 2 quartos</span>
          <span>🚗 1 vaga</span>
          <span>📐 68 m²</span>
        </div>

        <div class="price">R$ 450.000</div>

        <a
          class="button"
          href="https://wa.me/5511961556644?text=Ol%C3%A1%2C%20tenho%20interesse%20no%20Residencial%20Arctus%20Prime."
          target="_blank">
          Tenho interesse
        </a>
      </div>
    </article>

    <article class="property" data-preco="680000" data-quartos="3">
      <img
        src="https://images.unsplash.com/photo-1600566753086-00f18fb6b3ea?auto=format&fit=crop&w=900&q=80"
        alt="Apartamento de alto padrão">

      <div class="property-info">
        <h3>Arctus Residence</h3>
        <p class="location">São Paulo • Moema</p>

        <div class="details">
          <span>🛏 3 quartos</span>
          <span>🚗 2 vagas</span>
          <span>📐 94 m²</span>
        </div>

        <div class="price">R$ 680.000</div>

        <a
          class="button"
          href="https://wa.me/5511961556644?text=Ol%C3%A1%2C%20tenho%20interesse%20no%20Arctus%20Residence."
          target="_blank">
          Tenho interesse
        </a>
      </div>
    </article>

    <article class="property" data-preco="295000" data-quartos="1">
      <img
        src="https://images.unsplash.com/photo-1600607688969-a5bfcd646154?auto=format&fit=crop&w=900&q=80"
        alt="Apartamento compacto">

      <div class="property-info">
        <h3>Arctus Studio</h3>
        <p class="location">São Paulo • Pinheiros</p>

        <div class="details">
          <span>🛏 1 quarto</span>
          <span>🚗 1 vaga</span>
          <span>📐 42 m²</span>
        </div>

        <div class="price">R$ 295.000</div>

        <a
          class="button"
          href="https://wa.me/5511961556644?text=Ol%C3%A1%2C%20tenho%20interesse%20no%20Arctus%20Studio."
          target="_blank">
          Tenho interesse
        </a>
      </div>
    </article>

  </div>
</section>

<section class="about" id="sobre">
  <div class="about-content">
    <h2>Arctus Imóveis</h2>

    <p>
      Encontre apartamentos novos e lançamentos imobiliários
      de acordo com seu perfil, localização e orçamento.
    </p>
  </div>
</section>

<section class="contact" id="contato">
  <h2>Encontre seu próximo imóvel</h2>

  <p>
    Fale com a Arctus e receba informações sobre os apartamentos disponíveis.
  </p>

  <a
    class="button"
    href="https://wa.me/5511961556644?text=Ol%C3%A1%2C%20quero%20conhecer%20os%20apartamentos%20da%20Arctus."
    target="_blank">
    Falar pelo WhatsApp
  </a>
</section>

<footer>
  © 2026 Arctus Imóveis — Todos os direitos reservados.
</footer>

<a
  class="whatsapp"
  href="https://wa.me/5511961556644?text=Ol%C3%A1%2C%20quero%20conhecer%20os%20apartamentos%20da%20Arctus."
  target="_blank"
  aria-label="WhatsApp">
  ☎
</a>

<script>
  function buscarImoveis() {
    const quartos = document.getElementById("quartos").value;
    const preco = document.getElementById("preco").value;
    const localizacao =
      document.getElementById("localizacao").value.toLowerCase();

    const imoveis = document.querySelectorAll(".property");

    imoveis.forEach(imovel => {
      const precoImovel = Number(imovel.dataset.preco);
      const quartosImovel = Number(imovel.dataset.quartos);
      const texto = imovel.innerText.toLowerCase();

      let mostrar = true;

      if (quartos && quartos !== "4" &&
          quartosImovel !== Number(quartos)) {
        mostrar = false;
      }

      if (quartos === "4" && quartosImovel < 4) {
        mostrar = false;
      }

      if (preco && precoImovel > Number(preco)) {
        mostrar = false;
      }

      if (localizacao && !texto.includes(localizacao)) {
        mostrar = false;
      }

      imovel.style.display = mostrar ? "block" : "none";
    });

    document.getElementById("imoveis").scrollIntoView({
      behavior: "smooth"
    });
  }
</script>

</body>
</html>
