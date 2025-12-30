<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fátima Cocadas e Doces Caseiros</title>
    <link href="fonts.googleapis.com" rel="stylesheet">
    <style>
        :root {
            --cor-primaria: #4e342e; /* Marrom Chocolate */
            --cor-secundaria: #fffbf2; /* Creme suave */
            --cor-destaque: #8d6e63; /* Marrom elegante */
            --cor-texto: #2d2d2d;
            --whatsapp: #25d366;
        }

        body { 
            font-family: 'Lora', serif; 
            margin: 0; 
            background-color: var(--cor-secundaria); 
            color: var(--cor-texto);
            line-height: 1.8;
        }

        .container { max-width: 900px; margin: auto; padding: 0 20px; }
        section { padding: 80px 0; }

        /* HEADER */
        header { 
            background-color: var(--cor-primaria);
            color: #f5f5f5; 
            padding: 100px 0 50px 0; 
            text-align: center;
            border-bottom: 8px solid var(--cor-destaque);
        }

        header h1 { 
            font-family: 'Playfair Display', serif;
            font-size: 4.5em; 
            margin: 0;
            letter-spacing: 2px;
        }

        header p { font-style: italic; font-size: 1.3em; opacity: 0.9; margin-top: 10px; }

        /* MENU FIXO NO TOPO */
        .menu {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: var(--cor-primaria);
            padding: 10px 0;
            z-index: 999;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }

        .menu ul {
            list-style: none;
            display: flex;
            gap: 40px;
            margin: 0;
            padding: 0;
            justify-content: center;
        }

        .menu ul li a {
            text-decoration: none;
            color: #fff;
            font-weight: bold;
            font-size: 1.1em;
            transition: color 0.3s, transform 0.3s;
        }

        .menu ul li a:hover {
            color: var(--cor-destaque);
            transform: scale(1.1);
        }

        /* HERO / NOSSAS ESPECIALIDADES */
        .hero { 
            background: white; 
            text-align: center; 
            border-bottom: 1px solid #e0e0e0;
            padding-top: 120px; /* espaço para menu fixo */
        }

        .hero h2 { 
            font-family: 'Playfair Display', serif;
            color: var(--cor-primaria); 
            font-size: 2.8em; 
            margin-bottom: 20px; 
        }

        .hero p { 
            font-size: 1.2em; 
            max-width: 700px;
            margin: 0 auto;
            color: #444;
        }

        /* Layout da Lista de Sabores */
        .cardapio { 
            display: flex; 
            flex-direction: column; 
            gap: 40px; 
            margin-top: 20px;
        }

        .item-doce { 
            background: white; 
            padding: 40px;
            border-radius: 4px; 
            border-left: 5px solid var(--cor-primaria);
            box-shadow: 0 4px 15px rgba(0,0,0,0.03);
        }
        
        .item-doce h3 { 
            font-family: 'Playfair Display', serif;
            color: var(--cor-primaria); 
            font-size: 2.2em;
            margin: 0 0 15px 0; 
            border-bottom: 1px solid #eee;
            padding-bottom: 10px;
        }

        .item-doce p { 
            font-size: 1.1em; 
            color: #444; 
            text-align: justify;
        }

        /* CTA */
        .cta { background: var(--cor-destaque); color: white; text-align: center; }
        .cta h3 { font-family: 'Playfair Display', serif; font-size: 2.2em; margin-bottom: 10px; }

        /* BOTÃO WHATSAPP */
        .whatsapp-btn {
          display: inline-flex;
          align-items: center;
          gap: 10px;
          background: var(--whatsapp);
          color: white;
          font-weight: bold;
          padding: 12px 20px;
          border-radius: 50px;
          text-decoration: none;
          font-family: Arial, sans-serif;
          box-shadow: 0 0 10px var(--whatsapp), 0 0 20px var(--whatsapp), 0 0 30px var(--whatsapp);
          transition: all 0.3s ease-in-out;
          animation: glow 1.5s infinite alternate;
        }

        .whatsapp-btn img { width: 24px; height: 24px; }

        .whatsapp-btn:hover {
          transform: scale(1.1);
          box-shadow: 0 0 20px var(--whatsapp), 0 0 30px var(--whatsapp), 0 0 40px var(--whatsapp);
        }

        @keyframes glow {
          from { box-shadow: 0 0 10px var(--whatsapp), 0 0 20px var(--whatsapp), 0 0 30px var(--whatsapp); }
          to { box-shadow: 0 0 20px var(--whatsapp), 0 0 30px var(--whatsapp), 0 0 40px var(--whatsapp); }
        }

        /* BOTÃO FLUTUANTE WHATSAPP */
        .wpp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: var(--whatsapp);
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            text-align: center;
            line-height: 60px;
            box-shadow: 2px 5px 15px rgba(0,0,0,0.3);
            z-index: 100;
            text-decoration: none;
            font-weight: bold;
        }

        footer { text-align: center; padding: 60px 20px; background: #2d2d2d; color: #bbb; }
        footer a { color: #fff; text-decoration: none; border-bottom: 1px solid #555; }
    </style>
</head>
<body>

    <!-- MENU FIXO NO TOPO -->
    <nav class="menu">
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#sobre-nos">Sobre Nós</a></li>
        <li><a href="#produtos">Nossos Produtos</a></li>
        <li><a href="#contato">Fale Conosco</a></li>
      </ul>
    </nav>

    <header>
        <div class="container">
            <h1>Fátima Cocadas</h1>
            <p>Tradição Artesanal e Sabor Inigualável</p>
        </div>
    </header>

    <!-- SEÇÃO HERO / NOSSAS ESPECIALIDADES -->
    <section class="hero" id="home">
        <div class="container">
            <h2>Nossas Especialidades</h2>
            <p>Descubra a autenticidade das nossas cocadas artesanais: sabores elaborados com coco fresco, frutas naturais e todo carinho artesanal que garante um doce **cremoso, saboroso e inesquecível** em cada mordida. Uma verdadeira experiência de tradição e qualidade para os paladares mais exigentes.</p>
        </div>
    </section>

    <!-- SEÇÃO SOBRE NÓS -->
    <section class="container" id="sobre-nos">
        <h2>Sobre Nós</h2>
        <p>Há anos trazendo doces artesanais com tradição e qualidade. Cada receita é feita com amor e cuidado, mantendo o sabor autêntico que nossos clientes adoram.</p>
    </section>

    <!-- SEÇÃO PRODUTOS -->
    <section class="container" id="produtos">
        <div class="cardapio">
            
            <!-- Cocadas -->
            <div class="item-doce">
                <h3>Cocada Natural</h3>
                <p>Desfrute da autenticidade do coco fresco em cada mordida. Nossa cocada natural é cuidadosamente preparada com ingredientes selecionados, sem conservantes ou aditivos artificiais, garantindo sabor puro e textura irresistível. Uma opção deliciosa e tradicional para quem valoriza qualidade e naturalidade.</p>
            </div>

            <div class="item-doce">
                <h3>Cocada Queimada</h3>
                <p>Um clássico irresistível! Nossa cocada queimada é feita com coco fresco e açúcar caramelizado, resultando em uma textura crocante por fora e macia por dentro, com aquele sabor intenso e levemente tostado que conquista qualquer paladar. Feita artesanalmente, sem conservantes, é a escolha perfeita para quem busca tradição e sabor marcante.</p>
            </div>

            <div class="item-doce">
                <h3>Cocada de Maracujá</h3>
                <p>Delicie-se com a combinação perfeita de coco fresco e maracujá natural, resultando em uma cocada cremosa, leve e com um toque cítrico irresistível. Feita artesanalmente, sem conservantes, é a escolha ideal para quem busca sabor autêntico e sofisticado.</p>
            </div>

            <div class="item-doce">
                <h3>Cocada de Abacaxi</h3>
                <p>Uma combinação tropical que encanta! Nossa cocada de abacaxi é feita com coco fresco e abacaxi natural, resultando em uma textura cremosa e sabor equilibrado entre doce e levemente ácido. Produzida artesanalmente e sem conservantes, oferece um sabor fresco e autêntico em cada mordida.</p>
            </div>

            <div class="item-doce">
                <h3>Cocada de Limão</h3>
                <p>Refrescante e irresistível! Nossa cocada de limão combina coco fresco e limão natural, resultando em uma textura cremosa com sabor cítrico delicado e marcante. Feita artesanalmente e sem conservantes, é a escolha ideal para quem busca sabor autêntico e equilibrado.</p>
            </div>

        </div>
    </section>

    <!-- SEÇÃO CTA / WHATSAPP -->
    <section class="cta" id="contato">
        <div class="container">
            <h3>Faça seu Pedido</h3>
            <p>Levamos o melhor do doce artesanal até você ou seu estabelecimento.</p>
            
            <a href="https://wa.me/5548991317838" target="_blank" class="whatsapp-btn">
              <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" />
              Fale conosco
            </a>
        </div>
    </section>

    <!-- BOTÃO FLUTUANTE WHATSAPP -->
    <a href="https://wa.me/5548991317838" class="wpp-float" target="_blank">WPP</a>

    <footer>
        <div class="container">
            <p>
                <a href="https://www.google.com" target="_blank">
                    📍 Rua Miguel Teixeira 140, Morro da Fumaça - SC
                </a>
            </p>
            <p>&copy; 2025 Fátima Cocadas e Doces Caseiros. Desde sempre, o sabor da tradição.</p>
        </div>
    </footer>

</body>
</html>
