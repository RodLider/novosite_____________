
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Solicite crédito para investimento com parcelas acessíveis. Rural, imóvel, veículos e mais!" />
  <meta name="theme-color" content="#28a745" />
  <title>Crédito para Investimentos</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
      font-family: 'Montserrat', sans-serif;
    }

    body {
      margin: 0;
      padding: 0;
      background: url('https://i.imgur.com/feeaOsL.jpeg') no-repeat center center fixed;
      background-size: cover;
      color: #000;
    }

    h1 {
      text-align: center;
      color: #28a745;
      font-size: 22px;
      margin-top: 40px;
      padding: 0 15px;
      text-transform: uppercase;
    }

    .container {
      background: rgba(255, 255, 255, 0.95);
      padding: 30px;
      border-radius: 12px;
      max-width: 480px;
      width: 90%;
      margin: 40px auto;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.2);
    }

    h2 {
      color: #28a745;
      font-weight: 600;
      margin-bottom: 20px;
      text-align: center;
      text-transform: uppercase;
    }

    label {
      font-size: 14px;
      font-weight: 600;
      text-align: left;
      display: block;
      margin-top: 15px;
    }

    input, select {
      width: 100%;
      padding: 12px;
      margin-top: 5px;
      border-radius: 6px;
      border: 1px solid #ccc;
      font-size: 15px;
    }

    button {
      margin-top: 25px;
      width: 100%;
      background-color: #28a745;
      color: white;
      padding: 15px;
      border: none;
      border-radius: 6px;
      font-size: 16px;
      font-weight: bold;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #218838;
      cursor: pointer;
    }

    .info-section {
      max-width: 800px;
      margin: 40px auto;
      padding: 0 20px;
      background-color: rgba(255,255,255,0.95);
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    .info-block {
      margin-bottom: 30px;
    }

    .info-block img {
      width: 100%;
      border-radius: 8px;
      margin-bottom: 15px;
    }

    .info-block h3 {
      color: #28a745;
      font-size: 20px;
      margin-bottom: 10px;
      text-transform: uppercase;
    }

    .info-block p {
      font-size: 15px;
      line-height: 1.6;
      color: #333;
      text-transform: none;
    }

    footer {
      background-color: #f0f0f0;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
      font-size: 14px;
      text-transform: uppercase;
      color: #333;
    }

    footer a {
      color: #28a745;
      text-decoration: none;
      margin: 0 10px;
    }

    @media (max-width: 480px) {
      h1, h2 {
        font-size: 18px;
      }
    }
  </style>
</head>
<body>

  <h1>Simule o crédito que precisa, com as melhores condições!</h1>

  <div class="container">
    <h2>Solicite seu crédito</h2>
    <form onsubmit="event.preventDefault(); enviarWhatsApp();">
      <label for="nome">Nome</label>
      <input type="text" id="nome" placeholder="Digite seu nome" required />

      <label for="telefone">Telefone (com DDD)</label>
      <input type="tel" id="telefone" placeholder="Ex: 98999999999" pattern="\\d{10,11}" required />

      <label for="cidade">Cidade</label>
      <input type="text" id="cidade" placeholder="Sua cidade" required />

      <label for="investimento">Área de Investimento</label>
      <select id="investimento" required>
        <option value="" disabled selected>Escolha uma opção</option>
        <option>Crédito Rural</option>
        <option>Crédito Veicular</option>
        <option>Crédito Imobiliário</option>
        <option>Crédito para Construção</option>
        <option>Crédito para Reforma</option>
        <option>Crédito Comercial</option>
        <option>Crédito para Máquinas</option>
        <option>Crédito Agropecuário</option>
      </select>

      <label for="valor">Valor do Investimento</label>
      <select id="valor" onchange="atualizarParcelas()" required>
        <option value="" disabled selected>Selecione o valor</option>
        <option value="100000">R$ 100.000</option>
        <option value="150000">R$ 150.000</option>
        <option value="200000">R$ 200.000</option>
        <option value="250000">R$ 250.000</option>
        <option value="350000">R$ 350.000</option>
        <option value="400000">R$ 400.000</option>
        <option value="500000">R$ 500.000</option>
        <option value="600000">R$ 600.000</option>
        <option value="750000">R$ 750.000</option>
        <option value="800000">R$ 800.000</option>
        <option value="1000000">R$ 1.000.000</option>
      </select>

      <label for="parcela">Parcela Aproximada</label>
      <select id="parcela" required>
        <option value="" disabled selected>Escolha o valor do investimento primeiro</option>
      </select>

      <button type="submit">Solicitar via WhatsApp</button>
    </form>
  </div>

  <div class="info-section">
    <div class="info-block">
      <img src="https://i.imgur.com/h8OLLPy.jpeg" alt="Crédito Agrícola" />
      <h3>Crédito para investimento agrícola</h3>
      <p>Você sabia que agora é mais fácil adquirir o seu crédito para investimento agro com as melhores condições do mercado? Taxas de juros quase zero, entrada reduzida e parcelas flexíveis, tudo para tornar a aquisição da sua máquina, terras, fazendas, uma realidade mais acessível.</p>
    </div>

    <div class="info-block">
      <img src="https://i.imgur.com/IeHB7yK.jpeg" alt="Crédito Imobiliário" />
      <h3>Crédito Imobiliário</h3>
      <p>Se você está em busca de condições incríveis para adquirir o seu imóvel, nós temos a solução perfeita para você! Com taxas de juros extremamente competitivas, praticamente a zero, garantimos que você pague menos, com parcelas que cabem no seu bolso.</p>
    </div>

    <div class="info-block">
      <img src="https://i.imgur.com/FkYEFVg.jpeg" alt="Crédito para Veículos" />
      <h3>Crédito para Veículos leves</h3>
      <p>Está pronto para conquistar o seu novo carro? Agora, você pode ter as melhores condições para conquistar o veículo dos seus sonhos, com taxas de juros quase zero, entrada reduzida e parcelas que cabem no seu orçamento, tudo com a flexibilidade que você precisa.</p>
    </div>
  </div>

  <footer>
    <a href="#">Políticas</a> |
    <a href="#">Privacidade</a> |
    <a href="#">LGPD</a><br>
    Copyright © 2025
  </footer>

  <script>
    function atualizarParcelas() {
      var valor = document.getElementById("valor").value;
      var parcela = document.getElementById("parcela");
      parcela.innerHTML = '<option disabled selected>Carregando...</option>';

      const opcoesParcelas = {
        "100000": [590, 690, 800, 900],
        "150000": [890, 950, 1200, 1500],
        "200000": [1100, 1300, 1500, 1800],
        "250000": [1500, 2000, 2500, 3000],
        "350000": [2000, 2500, 3000],
        "400000": [2200, 2700, 3200],
        "500000": [3000, 4000, 5000],
        "600000": [3500, 4500, 5500],
        "750000": [5000, 6000, 7000],
        "800000": [5500, 7000, 8500],
        "1000000": [7000, 10000, 15000]
      };

      parcela.innerHTML = '<option disabled selected>Escolha uma opção</option>';
      if (opcoesParcelas[valor]) {
        opcoesParcelas[valor].forEach(p => {
          const opt = document.createElement("option");
          opt.value = p;
          opt.textContent = `R$ ${p.toLocaleString()}`;
          parcela.appendChild(opt);
        });
      }
    }

    function enviarWhatsApp() {
      const nome = document.getElementById("nome").value.trim();
      const tel = document.getElementById("telefone").value.trim();
      const cidade = document.getElementById("cidade").value.trim();
      const investimento = document.getElementById("investimento").value;
      const valor = document.getElementById("valor").value;
      const parcela = document.getElementById("parcela").value;

      if (!nome || !tel || !cidade || !investimento || !valor || !parcela) {
        alert("Preencha todos os campos!");
        return;
      }

      const mensagem = `Oi, meu nome é *${nome}*.\nTenho interesse em crédito para investimento.\n\n📍 *Cidade:* ${cidade}\n📞 *Telefone:* ${tel}\n🏠 *Área:* ${investimento}\n💰 *Valor:* R$ ${parseInt(valor).toLocaleString()}\n💳 *Parcela:* R$ ${parseInt(parcela).toLocaleString()}`;
      const link = `https://wa.me/5598985315556?text=${encodeURIComponent(mensagem)}`;
      window.open(link, "_blank");
    }
  </script>

</body>
</html>
