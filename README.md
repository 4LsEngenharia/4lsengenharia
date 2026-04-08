
<!--
**4LsEngenharia/4lsengenharia** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>4LS Engenharia | Engenharia e Empreendimentos Elétricos</title>

  <meta name="description" content="4LS Engenharia - Engenharia e Empreendimentos Elétricos. Serviços técnicos e operacionais com qualidade, compromisso e parceria." />

  <style>
    :root{
      --bg:#070708;
      --bg2:#0f0f12;
      --gold:#d4af37;
      --gold2:#f2d675;
      --text:#f2f2f2;
      --muted:#c5c5c5;
      --card:#141417;
      --border:rgba(212,175,55,.25);
      --shadow: 0 20px 60px rgba(0,0,0,.55);
    }

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family: Arial, Helvetica, sans-serif;
      scroll-behavior:smooth;
    }

    body{
      background: linear-gradient(180deg, var(--bg), #040405);
      color:var(--text);
      overflow-x:hidden;
    }

    a{
      text-decoration:none;
      color:inherit;
    }

    header{
      position:fixed;
      top:0;
      left:0;
      width:100%;
      z-index:999;
      background: rgba(10,10,12,.88);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(212,175,55,.18);
    }

    .container{
      width:100%;
      max-width:1180px;
      margin:0 auto;
      padding:0 18px;
    }

    .nav{
      display:flex;
      align-items:center;
      justify-content:space-between;
      padding:14px 0;
      gap:10px;
    }

    .logo-area{
      display:flex;
      align-items:center;
      gap:12px;
    }

    .logo-img{
      width:55px;
      height:55px;
      border-radius:14px;
      object-fit:cover;
      border:1px solid rgba(212,175,55,.25);
      box-shadow: 0 0 25px rgba(212,175,55,.12);
    }

    .logo-text{
      display:flex;
      flex-direction:column;
      line-height:1.1;
    }

    .logo-text strong{
      font-size:18px;
      letter-spacing:1px;
      color:var(--gold2);
    }

    .logo-text span{
      font-size:12px;
      color:var(--muted);
      letter-spacing:.8px;
    }

    nav ul{
      list-style:none;
      display:flex;
      gap:18px;
      align-items:center;
    }

    nav ul li a{
      font-size:14px;
      color:var(--text);
      opacity:.85;
      transition:.2s;
    }

    nav ul li a:hover{
      opacity:1;
      color:var(--gold2);
    }

    .btn{
      padding:10px 16px;
      border-radius:12px;
      background: linear-gradient(135deg, var(--gold), var(--gold2));
      color:#111;
      font-weight:bold;
      font-size:14px;
      box-shadow: 0 10px 25px rgba(212,175,55,.18);
      transition:.25s;
      display:inline-block;
      border:none;
      cursor:pointer;
    }

    .btn:hover{
      transform: translateY(-2px);
      filter:brightness(1.05);
    }

    .btn-outline{
      padding:10px 16px;
      border-radius:12px;
      border:1px solid rgba(212,175,55,.45);
      color:var(--gold2);
      font-weight:bold;
      transition:.25s;
      display:inline-block;
    }

    .btn-outline:hover{
      background: rgba(212,175,55,.10);
      transform: translateY(-2px);
    }

    .hero{
      padding-top:120px;
      padding-bottom:80px;
      position:relative;
      overflow:hidden;
      background:
        linear-gradient(180deg, rgba(0,0,0,.85), rgba(0,0,0,.95)),
        url("https://images.unsplash.com/photo-1581092919535-7146f72f6dbe?auto=format&fit=crop&w=1400&q=80");
      background-size:cover;
      background-position:center;
    }

    .hero-grid{
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap:30px;
      align-items:center;
    }

    .hero h1{
      font-size:44px;
      line-height:1.15;
      margin-bottom:14px;
      color:#fff;
    }

    .hero h1 span{
      color:var(--gold2);
    }

    .hero p{
      color:rgba(255,255,255,.78);
      font-size:16px;
      line-height:1.7;
      margin-bottom:22px;
      max-width:650px;
    }

    .hero-actions{
      display:flex;
      gap:12px;
      flex-wrap:wrap;
      margin-bottom:16px;
    }

    .hero-card{
      background: linear-gradient(180deg, rgba(18,18,20,.92), rgba(10,10,12,.92));
      border:1px solid var(--border);
      border-radius:22px;
      padding:22px;
      box-shadow: var(--shadow);
    }

    .hero-card h3{
      font-size:16px;
      margin-bottom:12px;
      color:var(--gold2);
      letter-spacing:.5px;
    }

    .hero-card ul{
      list-style:none;
      display:flex;
      flex-direction:column;
      gap:10px;
    }

    .hero-card li{
      display:flex;
      align-items:flex-start;
      gap:10px;
      font-size:14px;
      color:var(--text);
      opacity:.9;
      line-height:1.5;
    }

    .dot{
      width:10px;
      height:10px;
      margin-top:5px;
      border-radius:50%;
      background: var(--gold2);
      box-shadow: 0 0 20px rgba(212,175,55,.55);
      flex-shrink:0;
    }

    section{
      padding:70px 0;
    }

    .title{
      font-size:28px;
      margin-bottom:10px;
      color:#fff;
    }

    .subtitle{
      color:var(--muted);
      max-width:760px;
      line-height:1.7;
      font-size:15px;
      margin-bottom:28px;
    }

    .cards{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:18px;
    }

    .card{
      background: linear-gradient(180deg, rgba(18,18,20,.92), rgba(10,10,12,.92));
      border:1px solid rgba(212,175,55,.18);
      border-radius:20px;
      padding:22px;
      transition:.25s;
    }

    .card:hover{
      transform: translateY(-4px);
      border:1px solid rgba(212,175,55,.35);
    }

    .card h4{
      font-size:16px;
      color:var(--gold2);
      margin-bottom:10px;
    }

    .card p{
      color:var(--muted);
      font-size:14px;
      line-height:1.7;
    }

    .about-grid{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:22px;
      align-items:center;
    }

    .about-box{
      background: linear-gradient(180deg, rgba(18,18,20,.92), rgba(10,10,12,.92));
      border:1px solid rgba(212,175,55,.20);
      border-radius:22px;
      padding:26px;
      box-shadow: var(--shadow);
    }

    .about-box h3{
      color:var(--gold2);
      font-size:18px;
      margin-bottom:10px;
    }

    .about-box p{
      color:var(--muted);
      font-size:14px;
      line-height:1.8;
      margin-bottom:12px;
    }

    .badge-row{
      display:flex;
      flex-wrap:wrap;
      gap:10px;
      margin-top:12px;
    }

    .badge{
      border:1px solid rgba(212,175,55,.35);
      padding:8px 12px;
      border-radius:999px;
      font-size:12px;
      color:var(--gold2);
      background: rgba(212,175,55,.06);
    }

    .contact-grid{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:20px;
    }

    .contact-box{
      background: linear-gradient(180deg, rgba(18,18,20,.92), rgba(10,10,12,.92));
      border:1px solid rgba(212,175,55,.18);
      border-radius:22px;
      padding:26px;
    }

    .contact-box h3{
      color:var(--gold2);
      margin-bottom:10px;
    }

    .contact-box p{
      color:var(--muted);
      line-height:1.7;
      font-size:14px;
      margin-bottom:10px;
    }

    .contact-info{
      margin-top:10px;
      display:flex;
      flex-direction:column;
      gap:10px;
      font-size:14px;
    }

    .contact-info span{
      color:var(--text);
      opacity:.9;
    }

    form{
      display:flex;
      flex-direction:column;
      gap:12px;
      margin-top:10px;
    }

    input, textarea{
      width:100%;
      padding:12px 14px;
      border-radius:14px;
      border:1px solid rgba(212,175,55,.20);
      background: rgba(5,5,6,.7);
      color:#fff;
      outline:none;
      font-size:14px;
    }

    textarea{
      min-height:120px;
      resize:none;
    }

    footer{
      padding:30px 0;
      border-top:1px solid rgba(212,175,55,.12);
      background: rgba(0,0,0,.35);
    }

    footer p{
      font-size:13px;
      color:var(--muted);
      line-height:1.7;
      text-align:center;
    }

    .whatsapp-float{
      position:fixed;
      bottom:20px;
      right:20px;
      background: linear-gradient(135deg, var(--gold), var(--gold2));
      color:#111;
      padding:12px 16px;
      border-radius:999px;
      font-weight:bold;
      box-shadow: 0 18px 40px rgba(0,0,0,.55);
      z-index:9999;
      display:flex;
      gap:10px;
      align-items:center;
      transition:.2s;
    }

    .whatsapp-float:hover{
      transform: translateY(-3px);
      filter:brightness(1.05);
    }

    .menu-btn{
      display:none;
      border:1px solid rgba(212,175,55,.25);
      padding:8px 12px;
      border-radius:12px;
      color:var(--gold2);
      font-size:14px;
      background: transparent;
      cursor:pointer;
    }

    @media (max-width: 900px){
      .hero-grid{
        grid-template-columns:1fr;
      }

      .cards{
        grid-template-columns:1fr;
      }

      .about-grid{
        grid-template-columns:1fr;
      }

      .contact-grid{
        grid-template-columns:1fr;
      }

      nav ul{
        display:none;
        position:absolute;
        top:70px;
        right:18px;
        flex-direction:column;
        background: rgba(10,10,12,.95);
        border:1px solid rgba(212,175,55,.18);
        padding:16px;
        border-radius:18px;
        width:220px;
        box-shadow: var(--shadow);
      }

      nav ul.active{
        display:flex;
      }

      .menu-btn{
        display:block;
      }

      .hero h1{
        font-size:34px;
      }
    }
  </style>
</head>

<body>

  <!-- HEADER -->
  <header>
    <div class="container">
      <div class="nav">

        <div class="logo-area">
          <img src="logo.png" class="logo-img" alt="Logo 4LS Engenharia">
          <div class="logo-text">
            <strong>4LS ENGENHARIA</strong>
            <span>Engenharia e Empreendimentos Elétricos</span>
          </div>
        </div>

        <nav>
          <button class="menu-btn" onclick="toggleMenu()">Menu</button>
          <ul id="menu">
            <li><a href="#inicio">Início</a></li>
            <li><a href="#servicos">Serviços</a></li>
            <li><a href="#sobre">Sobre</a></li>
            <li><a href="#parcerias">Parcerias</a></li>
            <li><a href="#contato">Contato</a></li>
          </ul>
        </nav>

        <a class="btn" href="#contato">Solicitar Orçamento</a>

      </div>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero" id="inicio">
    <div class="container">
      <div class="hero-grid">

        <div>
          <h1>
            Soluções em <span>Engenharia</span> com Qualidade e Compromisso
          </h1>

          <p>
            A <strong>4LS Engenharia</strong> atua com excelência em serviços de engenharia e atividades operacionais,
            oferecendo suporte completo, agilidade e compromisso com prazos e qualidade.
          </p>

          <div class="hero-actions">
            <a class="btn" target="_blank" href="https://wa.me/5577999158488">WhatsApp</a>
            <a class="btn-outline" href="tel:+5577999158488">Ligar</a>
            <a class="btn-outline" href="mailto:4lsengenharia@gmail.com">E-mail</a>
            <a class="btn-outline" target="_blank" href="https://www.instagram.com/4lsengenharia/">Instagram</a>
          </div>

          <p style="font-size:13px; color:rgba(255,255,255,.6);">
            Atendimento profissional • Responsabilidade • Segurança • Resultados
          </p>
        </div>

        <div class="hero-card">
          <h3>Diferenciais da 4LS</h3>
          <ul>
            <li><span class="dot"></span> Atendimento rápido e personalizado</li>
            <li><span class="dot"></span> Compromisso com qualidade e segurança</li>
            <li><span class="dot"></span> Profissionais qualificados</li>
            <li><span class="dot"></span> Soluções para demandas industriais e operacionais</li>
            <li><span class="dot"></span> Parcerias para locação de máquinas, caminhões e ferramentas</li>
          </ul>
        </div>

      </div>
    </div>
  </section>

  <!-- SERVIÇOS -->
  <section id="servicos">
    <div class="container">
      <h2 class="title">Nossos Serviços</h2>
      <p class="subtitle">
        Prestamos serviços completos para empresas e indústrias, oferecendo soluções eficientes, técnicas e operacionais.
      </p>

      <div class="cards">
        <div class="card">
          <h4>Engenharia e Serviços Técnicos</h4>
          <p>Atuação com planejamento, suporte e execução de atividades de engenharia em diversos setores.</p>
        </div>

        <div class="card">
          <h4>Empreendimentos Elétricos</h4>
          <p>Atividades e soluções voltadas para área elétrica, manutenção e suporte técnico especializado.</p>
        </div>

        <div class="card">
          <h4>Manutenção Industrial</h4>
          <p>Suporte em atividades industriais, manutenção preventiva e corretiva conforme necessidade do cliente.</p>
        </div>

        <div class="card">
          <h4>Serviços Operacionais</h4>
          <p>Atuação em campo e suporte operacional com foco em produtividade e segurança.</p>
        </div>

        <div class="card">
          <h4>Terceirização de Equipes</h4>
          <p>Fornecimento de mão de obra qualificada para demandas temporárias ou contínuas.</p>
        </div>

        <div class="card">
          <h4>Consultoria e Apoio Técnico</h4>
          <p>Consultoria e suporte para organização de serviços, execução e melhorias técnicas.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- SOBRE -->
  <section id="sobre">
    <div class="container">
      <h2 class="title">Sobre a 4LS Engenharia</h2>
      <p class="subtitle">
        Uma empresa comprometida em entregar soluções com excelência, segurança e confiança para seus clientes.
      </p>

      <div class="about-grid">
        <div class="about-box">
          <h3>Quem Somos</h3>
          <p>
            A <strong>4LS Engenharia</strong> oferece soluções em engenharia e empreendimentos elétricos,
            atendendo demandas técnicas e operacionais com responsabilidade e qualidade.
          </p>
          <p>
            Trabalhamos com foco em resultados e na satisfação do cliente, mantendo compromisso com prazos e segurança.
          </p>

          <div class="badge-row">
            <div class="badge">Compromisso</div>
            <div class="badge">Segurança</div>
            <div class="badge">Qualidade</div>
            <div class="badge">Parceria</div>
          </div>
        </div>

        <div class="about-box">
          <h3>Missão, Visão e Valores</h3>
          <p><strong style="color:var(--gold2);">Missão:</strong> entregar soluções eficientes e seguras em engenharia.</p>
          <p><strong style="color:var(--gold2);">Visão:</strong> ser referência em serviços técnicos e operacionais.</p>
          <p><strong style="color:var(--gold2);">Valores:</strong> ética, qualidade, confiança e profissionalismo.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- PARCERIAS -->
  <section id="parcerias">
    <div class="container">
      <h2 class="title">Parcerias e Relacionamento</h2>
      <p class="subtitle">
        Temos um excelente relacionamento com empresas parceiras de locação de máquinas, caminhões e ferramentas,
        garantindo suporte completo para atender nossos clientes com agilidade e estrutura.
      </p>

      <div class="cards">
        <div class="card">
          <h4>Locação de Máquinas</h4>
          <p>Parcerias com empresas qualificadas para locação de máquinas e equipamentos.</p>
        </div>

        <div class="card">
          <h4>Locação de Caminhões</h4>
          <p>Suporte logístico com caminhões para operações e transporte de materiais.</p>
        </div>

        <div class="card">
          <h4>Locação de Ferramentas</h4>
          <p>Ferramentas e equipamentos para execução de serviços técnicos e industriais.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CONTATO -->
  <section id="contato">
    <div class="container">
      <h2 class="title">Contato</h2>
      <p class="subtitle">
        Solicite seu orçamento agora mesmo. Atendimento rápido e profissional.
      </p>

      <div class="contact-grid">

        <div class="contact-box">
          <h3>Informações</h3>
          <p>Entre em contato conosco pelos canais abaixo:</p>

          <div class="contact-info">
            <span><strong style="color:var(--gold2);">WhatsApp:</strong> (77) 99915-8488</span>
            <span><strong style="color:var(--gold2);">E-mail:</strong> 4lsengenharia@gmail.com</span>
            <span><strong style="color:var(--gold2);">Endereço:</strong> Rua Olegário Augusto Viana, Nº 458</span>
            <span><strong style="color:var(--gold2);">Instagram:</strong> @4lsengenharia</span>
            <span><strong style="color:var(--gold2);">CNPJ:</strong> 60.943.647/0001-89</span>
          </div>

          <br>

          <a class="btn" target="_blank" href="https://wa.me/5577999158488">Falar no WhatsApp</a>
        </div>

        <div class="contact-box">
          <h3>Solicitar Orçamento</h3>

          <form onsubmit="enviarWhats(event)">
            <input type="text" id="nome" placeholder="Seu nome" required />
            <input type="text" id="empresa" placeholder="Empresa (opcional)" />
            <input type="text" id="telefone" placeholder="Seu WhatsApp" required />
            <textarea id="mensagem" placeholder="Descreva o serviço que precisa..." required></textarea>

            <button class="btn" type="submit">Enviar no WhatsApp</button>
          </form>
        </div>

      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="container">
      <p>
        © 2026 - 4LS Engenharia. Todos os direitos reservados.<br>
        CNPJ: 60.943.647/0001-89 | Rua Olegário Augusto Viana, Nº 458<br>
        Instagram: @4lsengenharia | E-mail: 4lsengenharia@gmail.com
      </p>
    </div>
  </footer>

  <!-- BOTÃO WHATSAPP -->
  <a class="whatsapp-float" target="_blank" href="https://wa.me/5577999158488">
    💬 WhatsApp
  </a>

  <script>
    function toggleMenu(){
      const menu = document.getElementById("menu");
      menu.classList.toggle("active");
    }

    function enviarWhats(event){
      event.preventDefault();

      const nome = document.getElementById("nome").value;
      const empresa = document.getElementById("empresa").value;
      const telefone = document.getElementById("telefone").value;
      const mensagem = document.getElementById("mensagem").value;

      const texto = `Olá! Me chamo ${nome}.
Empresa: ${empresa}
Telefone: ${telefone}

Gostaria de solicitar orçamento:
${mensagem}`;

      const numeroWhats = "5577999158488";
      const link = `https://wa.me/${numeroWhats}?text=${encodeURIComponent(texto)}`;

      window.open(link, "_blank");
    }
  </script>

</body>
</html>
