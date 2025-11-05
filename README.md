<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Método Venda Inicial - Sua Primeira Venda Online em 2025</title>
    <style>
        /* Reset e configurações básicas */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary: #000000;
            --secondary: #D4AF37;
            --accent: #FFD700;
            --light: #F8F8F8;
            --dark: #1A1A1A;
            --gray: #333333;
            --text: #FFFFFF;
        }
        
        body {
            background-color: var(--primary);
            color: var(--text);
            line-height: 1.6;
            scroll-behavior: smooth;
            padding-top: 40px;
            -webkit-text-size-adjust: 100%;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Barra de contador regressivo */
        #countdown-bar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: linear-gradient(90deg, var(--primary), var(--dark));
            color: var(--secondary);
            padding: 8px 0;
            text-align: center;
            font-size: 0.9rem;
            font-weight: 700;
            z-index: 1000;
            border-bottom: 1px solid var(--secondary);
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
        }
        
        #countdown {
            font-size: 1rem;
            font-weight: 800;
            letter-spacing: 1px;
            background: rgba(212, 175, 55, 0.1);
            padding: 2px 8px;
            border-radius: 4px;
            margin: 0 5px;
        }
        
        /* Tipografia */
        h1, h2, h3, h4 {
            font-weight: 700;
            line-height: 1.2;
            margin-bottom: 20px;
        }
        
        h1 {
            font-size: 2.8rem;
        }
        
        h2 {
            font-size: 2.2rem;
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }
        
        h2:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: var(--secondary);
        }
        
        h3 {
            font-size: 1.8rem;
        }
        
        p {
            margin-bottom: 15px;
            font-size: 1.1rem;
        }
        
        /* Botões */
        .btn {
            display: inline-block;
            padding: 15px 30px;
            background: linear-gradient(135deg, var(--secondary), var(--accent));
            color: var(--primary);
            text-decoration: none;
            font-weight: 700;
            font-size: 1.2rem;
            border-radius: 5px;
            text-align: center;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.3);
            -webkit-appearance: none;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(212, 175, 55, 0.5);
        }
        
        .btn-large {
            padding: 20px 40px;
            font-size: 1.4rem;
            width: 100%;
            max-width: 400px;
        }
        
        /* Seções */
        section {
            padding: 80px 0;
        }
        
        .section-light {
            background-color: var(--light);
            color: var(--primary);
        }
        
        .section-dark {
            background-color: var(--dark);
        }
        
        /* Header */
        header {
            background: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.9));
            padding: 60px 0 100px;
            text-align: center;
        }
        
        .logo-container {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }
        
        .logo-image {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid var(--secondary);
            box-shadow: 0 0 20px rgba(212, 175, 55, 0.5);
        }
        
        .logo-text {
            font-size: 2.5rem;
            font-weight: 700;
            margin-left: 20px;
            color: var(--secondary);
        }
        
        .subtitle {
            font-size: 1.4rem;
            margin-bottom: 30px;
            color: var(--secondary);
        }
        
        .attention {
            background-color: var(--secondary);
            color: var(--primary);
            padding: 10px 20px;
            border-radius: 5px;
            display: inline-block;
            margin: 20px 0;
            font-weight: 700;
        }
        
        /* Problema/Solução */
        .problem-list {
            list-style: none;
            margin: 30px 0;
        }
        
        .problem-list li {
            margin-bottom: 15px;
            padding-left: 30px;
            position: relative;
        }
        
        .problem-list li:before {
            content: '✗';
            position: absolute;
            left: 0;
            color: #ff4d4d;
            font-weight: bold;
        }
        
        .solution-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .card {
            background: var(--dark);
            padding: 30px;
            border-radius: 10px;
            border-left: 5px solid var(--secondary);
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }
        
        .section-light .card {
            background: var(--light);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        /* Benefícios */
        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .benefit-item {
            background: var(--dark);
            padding: 25px;
            border-radius: 10px;
            border-top: 3px solid var(--secondary);
        }
        
        .section-light .benefit-item {
            background: var(--light);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .benefit-item h3 {
            color: var(--secondary);
            margin-bottom: 15px;
        }
        
        /* Depoimentos */
        .testimonials {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
            margin-top: 40px;
        }
        
        .testimonial {
            background: var(--dark);
            padding: 25px;
            border-radius: 10px;
            position: relative;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            transition: transform 0.3s ease;
        }
        
        .section-light .testimonial {
            background: var(--light);
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .testimonial:hover {
            transform: translateY(-5px);
        }
        
        .testimonial:before {
            content: '"';
            font-size: 4rem;
            color: var(--secondary);
            position: absolute;
            top: -10px;
            left: 10px;
            opacity: 0.3;
        }
        
        .testimonial-image {
            width: 100%;
            border-radius: 8px;
            margin: 20px 0;
            border: 2px solid var(--secondary);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .testimonial-author {
            font-weight: 700;
            margin-top: 15px;
            color: var(--secondary);
            display: flex;
            align-items: center;
        }
        
        .testimonial-author:before {
            content: "—";
            margin-right: 5px;
        }
        
        .testimonial-highlight {
            background: linear-gradient(135deg, var(--secondary), var(--accent));
            color: var(--primary);
            padding: 5px 10px;
            border-radius: 5px;
            font-weight: 700;
            display: inline-block;
            margin: 10px 0;
        }
        
        /* Garantia */
        .guarantee {
            text-align: center;
            padding: 50px;
            background: var(--dark);
            border-radius: 10px;
            margin-top: 40px;
            border: 2px solid var(--secondary);
        }
        
        .section-light .guarantee {
            background: var(--light);
        }
        
        .guarantee h3 {
            color: var(--secondary);
        }
        
        /* Preços */
        .pricing {
            text-align: center;
            padding: 50px 30px;
            background: var(--dark);
            border-radius: 10px;
            margin-top: 40px;
            border: 2px solid var(--secondary);
        }
        
        .section-light .pricing {
            background: var(--light);
        }
        
        .price-old {
            text-decoration: line-through;
            color: #999;
            font-size: 1.5rem;
        }
        
        .price-new {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--secondary);
            margin: 10px 0;
        }
        
        .price-installments {
            font-size: 2.2rem;
            font-weight: 800;
            color: var(--accent);
            margin: 15px 0;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
        }
        
        .installment-highlight {
            background: linear-gradient(135deg, var(--accent), var(--secondary));
            color: var(--primary);
            padding: 8px 16px;
            border-radius: 8px;
            display: inline-block;
            margin: 10px 0;
            box-shadow: 0 4px 12px rgba(212, 175, 55, 0.4);
        }
        
        .bonus {
            background: var(--secondary);
            color: var(--primary);
            padding: 10px;
            border-radius: 5px;
            margin: 20px 0;
            font-weight: 700;
        }
        
        /* Autor */
        .author-section {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 30px;
            margin: 40px 0;
            padding: 30px;
            background: var(--dark);
            border-radius: 10px;
        }
        
        .section-light .author-section {
            background: var(--light);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .author-image {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid var(--secondary);
        }
        
        .author-info {
            flex: 1;
        }
        
        .author-highlight {
            color: var(--secondary);
            font-weight: 700;
        }
        
        /* FAQ */
        .faq-item {
            margin-bottom: 20px;
            border-bottom: 1px solid var(--gray);
            padding-bottom: 20px;
        }
        
        .section-light .faq-item {
            border-bottom: 1px solid #ddd;
        }
        
        .faq-question {
            font-weight: 700;
            color: var(--secondary);
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .faq-answer {
            margin-top: 10px;
            display: none;
        }
        
        .faq-item.active .faq-answer {
            display: block;
        }
        
        /* Footer */
        footer {
            background: var(--dark);
            padding: 40px 0;
            text-align: center;
            border-top: 1px solid var(--gray);
        }
        
        .footer-logo {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .footer-logo-image {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid var(--secondary);
        }
        
        .legal {
            font-size: 0.9rem;
            color: #999;
            margin-top: 30px;
        }

        /* Classes para substituir estilos inline */
        .testimonials-intro {
            text-align: center;
            max-width: 800px;
            margin: 0 auto 40px;
        }
        
        .testimonials-cta {
            text-align: center;
            margin-top: 50px;
        }
        
        .payment-info {
            margin-top: 20px;
            font-size: 0.9rem;
        }
        
        .header-countdown {
            font-weight: bold;
            color: var(--secondary);
        }
        
        /* Responsividade - Mobile First */
        /* Telas pequenas (smartphones) */
        @media (max-width: 576px) {
            body {
                padding-top: 35px;
            }
            
            #countdown-bar {
                font-size: 0.7rem;
                padding: 6px 0;
            }
            
            #countdown {
                font-size: 0.8rem;
            }
            
            .container {
                padding: 0 15px;
            }
            
            h1 {
                font-size: 1.8rem;
            }
            
            h2 {
                font-size: 1.5rem;
                margin-bottom: 30px;
            }
            
            h3 {
                font-size: 1.3rem;
            }
            
            p {
                font-size: 1rem;
            }
            
            section {
                padding: 40px 0;
            }
            
            header {
                padding: 40px 0 60px;
            }
            
            .logo-container {
                flex-direction: column;
                text-align: center;
            }
            
            .logo-image {
                width: 100px;
                height: 100px;
            }
            
            .logo-text {
                font-size: 1.8rem;
                margin-left: 0;
                margin-top: 15px;
            }
            
            .subtitle {
                font-size: 1.1rem;
            }
            
            .btn {
                padding: 12px 25px;
                font-size: 1rem;
                width: 100%;
                max-width: 300px;
            }
            
            .btn-large {
                padding: 15px 30px;
                font-size: 1.2rem;
            }
            
            .solution-cards, .benefits-grid, .testimonials {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .card, .benefit-item, .testimonial {
                padding: 20px;
            }
            
            .author-section {
                flex-direction: column;
                text-align: center;
                gap: 20px;
                padding: 20px;
                margin: 30px 0;
            }
            
            .author-image {
                width: 120px;
                height: 120px;
            }
            
            .guarantee, .pricing {
                padding: 30px 15px;
                margin-top: 30px;
            }
            
            .price-new {
                font-size: 2rem;
            }
            
            .price-installments {
                font-size: 1.8rem;
            }
            
            .footer-logo-image {
                width: 60px;
                height: 60px;
            }
            
            .testimonials-intro {
                margin: 0 auto 30px;
            }
            
            .testimonials-cta {
                margin-top: 30px;
            }
        }
        
        /* Telas médias (tablets) */
        @media (min-width: 577px) and (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
            h2 {
                font-size: 1.8rem;
            }
            
            section {
                padding: 60px 0;
            }
            
            .solution-cards, .benefits-grid, .testimonials {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .logo-container {
                flex-direction: column;
                text-align: center;
            }
            
            .logo-text {
                margin-left: 0;
                margin-top: 15px;
            }
            
            .author-section {
                flex-direction: column;
                text-align: center;
            }
        }
        
        /* Ajustes específicos para orientação paisagem em mobile */
        @media (max-height: 500px) and (orientation: landscape) {
            header {
                padding: 30px 0 50px;
            }
            
            section {
                padding: 30px 0;
            }
        }
        
        /* Melhorias de toque para dispositivos móveis */
        .btn, .faq-question {
            -webkit-tap-highlight-color: transparent;
        }
        
        .btn:active {
            transform: scale(0.98);
        }
        
        /* Prevenir problemas de renderização no iOS */
        * {
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
    </style>
</head>
<body>
    <!-- Barra de contador regressivo -->
    <div id="countdown-bar">
        <div class="container">
            ⚠️ OFERTA EXPIRA EM: <span id="countdown">20:00</span> - NÃO DEIXE PARA DEPOIS!
        </div>
    </div>

    <!-- Header -->
    <header>
        <div class="container">
            <div class="logo-container">
                <img src="https://www.dropbox.com/scl/fi/h54044utwgq09a5zda3ca/ChatGPT-Image-3-de-nov.-de-2025-10_20_00.png?rlkey=74xlanyd943o82qc3kfwgiiz6&st=aea0dolb&dl=1" alt="Método Venda Inicial" class="logo-image">
                <div class="logo-text">MÉTODO VENDA INICIAL</div>
            </div>
            <h1>SEU MAPA PARA DOMINAR VENDAS ONLINE EM 2025</h1>
            <p class="subtitle">(Mesmo Que Você Não Tenha Experiência, Produto ou Audiência)</p>
            <p>Enquanto 95% dos iniciantes desperdiçam tempo com métodos ultrapassados, você vai seguir um sistema comprovado que já gerou R$ 2,3+ milhões em vendas digitais.</p>
            
            <div class="attention">
                ⚠️ ATENÇÃO: 72% dos acessos com condição especial já foram preenchidos.
            </div>
            <p>Essa é sua chance <strong>ÚNICA</strong> de garantir o Método Venda Inicial com 80%, oferta válida expira em: <span id="header-countdown" class="header-countdown">20:00</span></p>
            
            <a href="#oferta" class="btn btn-large">QUERO MINHA PRIMEIRA VENDA!</a>
        </div>
    </header>

    <!-- Seção Para Quem É -->
    <section class="section-light">
        <div class="container">
            <h2>PARA QUEM ISSO FOI CRIADO</h2>
            <div class="solution-cards">
                <div class="card">
                    <h3>Iniciantes Absolutos</h3>
                    <p>Para quem quer criar um produto digital do zero e nunca vendeu nada online.</p>
                </div>
                <div class="card">
                    <h3>Frustrados Digitais</h3>
                    <p>Para quem já tentou vender online mas não teve resultados consistentes.</p>
                </div>
                <div class="card">
                    <h3>Pessoas Ocupadas</h3>
                    <p>Para quem tem apenas 1-2 horas por dia para dedicar ao negócio online.</p>
                </div>
                <div class="card">
                    <h3>Céticos Informados</h3>
                    <p>Para quem cansou de cursos genéricos que não funcionam na prática.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção Problema -->
    <section>
        <div class="container">
            <h2>VOCÊ SE IDENTIFICA COM ISSO?</h2>
            <ul class="problem-list">
                <li>Tentou seguir "gurus" que prometem enriquecimento rápido?</li>
                <li>Investiu em cursos que só mostram a teoria, mas não funcionam na prática?</li>
                <li>Passou horas nas redes sociais sem conseguir vender nada?</li>
                <li>Acreditou que precisa de milhares de seguidores para vender online?</li>
                <li>Se sente sobrecarregado com tanta informação contraditória?</li>
            </ul>
            <p><strong>O problema não é você - é a falta de um método realista e passo a passo.</strong></p>
        </div>
    </section>

    <!-- Seção Autor -->
    <section class="section-light">
        <div class="container">
            <h2>QUEM VAI TE GUIAR NESTA JORNADA</h2>
            <div class="author-section">
                <img src="https://www.dropbox.com/scl/fi/h54044utwgq09a5zda3ca/ChatGPT-Image-3-de-nov.-de-2025-10_20_00.png?rlkey=74xlanyd943o82qc3kfwgiiz6&st=aea0dolb&dl=1" alt="Gustavo Figueredo" class="author-image">
                <div class="author-info">
                    <h3>Gustavo Figueredo</h3>
                    <p>Vim de uma família simples, onde o dinheiro era sempre uma preocupação. Comecei do absoluto zero, sem contatos, sem experiência e sem saber por onde começar no mundo digital.</p>
                    <p>Depois de muitas tentativas frustradas, desenvolvi um método próprio que me levou a <span class="author-highlight">faturar mais de R$ 100.000 trimestralmente</span> com vendas online.</p>
                    <p>Hoje, minha missão é compartilhar esse conhecimento com pessoas que, assim como eu, querem transformar suas vidas através do digital, mas não sabem por onde começar.</p>
                    <p>O Método Venda Inicial nasceu da minha vontade de criar um caminho claro e acessível para quem está começando, baseado no que realmente funcionou para mim.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção Solução -->
    <section>
        <div class="container">
            <h2>A SOLUÇÃO: MÉTODO VENDA INICIAL</h2>
            <p>Não é milagre. É método comprovado.</p>
            
            <div class="solution-cards">
                <div class="card">
                    <h3>PRODUTO VITORIOSO</h3>
                    <p>Como criar uma oferta que as pessoas realmente querem comprar, mesmo começando do zero.</p>
                </div>
                <div class="card">
                    <h3>MÁQUINA DE VENDAS</h3>
                    <p>Estrutura automatizada que trabalha 24h por dia para você, mesmo enquanto dorme.</p>
                </div>
                <div class="card">
                    <h3>TRÁFEGO INTELIGENTE</h3>
                    <p>Onde e como anunciar gastando pouco e vendendo muito, sem complicação.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção Conteúdo -->
    <section class="section-light">
        <div class="container">
            <h2>O QUE VOCÊ VAI APRENDER</h2>
            <p>Conteúdo 100% focado em vendas e resultados práticos</p>
            
            <div class="benefits-grid">
                <div class="benefit-item">
                    <h3>Módulo 1: Estratégia de Vendas Digital</h3>
                    <p>O mindset do vendedor de sucesso, identificação de oportunidades reais de mercado e estrutura de vendas que converte constantemente.</p>
                </div>
                <div class="benefit-item">
                    <h3>Módulo 2: Criação do Produto Vencedor</h3>
                    <p>Metodologia para desenvolver produtos que vendem, formulação de preços e estratégias de valor e diferenciação competitiva.</p>
                </div>
                <div class="benefit-item">
                    <h3>Módulo 3: Copywriting que Converte</h3>
                    <p>Técnicas comprovadas de persuasão escrita, estrutura de copy para anúncios e páginas de venda e gatilhos mentais aplicados ao digital.</p>
                </div>
                <div class="benefit-item">
                    <h3>Módulo 4: Anúncios que Vendem</h3>
                    <p>Estratégias de tráfego pago e orgânico, otimização de campanhas para máximo ROI e segmentação avançada para encontrar seu cliente ideal.</p>
                </div>
                <div class="benefit-item">
                    <h3>Módulo 5: Conversão e Vendas</h3>
                    <p>Técnicas de fechamento online, estratégias para aumentar ticket médio e como lidar com objeções para aumentar conversão.</p>
                </div>
                <div class="benefit-item">
                    <h3>Módulo 6: Escalando Resultados</h3>
                    <p>Análise de métricas e KPIs essenciais, estratégias para escalar vendas comprovadas e automatização inteligente do processo comercial.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção Depoimentos com Comprovantes -->
    <section>
        <div class="container">
            <h2>RESULTADOS REAIS DE QUEM SEGUIU O MÉTODO</h2>
            <p class="testimonials-intro">Não são apenas palavras. São comprovantes reais de pessoas comuns que aplicaram o Método Venda Inicial e transformaram suas vidas financeiras.</p>
            
            <div class="testimonials">
                <!-- Depoimento 1 -->
                <div class="testimonial">
                    <p>"Eu nunca imaginei que chegaria a essa marca. Em apenas 5 meses aplicando o Método Venda Inicial, alcancei <span class="testimonial-highlight">R$ 100.000 em vendas na Kiwify</span>. Antes disso, eu mal conseguia vender R$ 500 por mês."</p>
                    
                    <img src="https://www.dropbox.com/scl/fi/endlwznk7wet6khxrkldj/WhatsApp-Image-2025-11-03-at-10.21.09.jpeg?rlkey=6d2babowmqfttwjtxhhxrr3ja&st=82lbmwn6&dl=1" alt="Comprovante de R$ 100.000 em vendas na Kiwify" class="testimonial-image">
                    
                    <div class="testimonial-author">Camila Fernandes, 28 anos</div>
                    <p><em>Ex-assistente administrativa, hoje empreendedora digital em tempo integral</em></p>
                </div>
                
                <!-- Depoimento 2 -->
                <div class="testimonial">
                    <p>"O que mais me impressionou foi a <span class="testimonial-highlight">automação do processo</span>. Agora vejo as vendas chegando a qualquer momento, no celular e no computador. Em um único dia faturei R$ 3.847, algo que antes me levaria meses."</p>
                    
                    <img src="https://www.dropbox.com/scl/fi/fa5ncu8wjalrwxoexl6fg/WhatsApp-Image-2025-11-03-at-10.21.10-1.jpeg?rlkey=ypuanw1ydcd8ygr78li5weqx3&st=dqh8rscw&dl=1" alt="Notificações de vendas no celular e métricas no computador" class="testimonial-image">
                    
                    <div class="testimonial-author">Ricardo Almeida, 32 anos</div>
                    <p><em>Ex-uber, hoje tem múltiplas fontes de renda online</em></p>
                </div>
                
                <!-- Depoimento 3 -->
                <div class="testimonial">
                    <p>"São tantas notificações de vendas que <span class="testimonial-highlight">perdi as contas de quantos produtos vendi</span>. O método me mostrou como escalar e hoje tenho uma renda que nunca imaginei possível. Tudo isso trabalhando de casa, no meu ritmo."</p>
                    
                    <img src="https://www.dropbox.com/scl/fi/kn4n4uyavtf69qlvdh9ml/WhatsApp-Image-2025-11-03-at-10.21.10-2.jpeg?rlkey=4j4921c3rm7m5td673x4nzqqv&st=991w5y1q&dl=1" alt="Print de notificações de vendas" class="testimonial-image">
                    
                    <div class="testimonial-author">Patrícia Santos, 35 anos</div>
                    <p><em>Mãe e empreendedora digital, fatura 5 dígitos mensais</em></p>
                </div>
            </div>
            
            <div class="testimonials-cta">
                <h3>Esses resultados podem ser seus também</h3>
                <p>O Método Venda Inicial não é teoria. É um passo a passo comprovado que já ajudou centenas de pessoas comuns a conquistarem sua independência financeira.</p>
                <a href="#oferta" class="btn btn-large">QUERO MEU PRIMEIRO RESULTADO</a>
            </div>
        </div>
    </section>

    <!-- Seção Garantia -->
    <section class="section-light">
        <div class="container">
            <div class="guarantee">
                <h3>GARANTIA INCONDICIONAL DE 7 DIAS</h3>
                <p>Entre no método, assista todas as aulas, execute o passo a passo por <strong>7 dias</strong>.</p>
                <p>Se não sentir que está no caminho certo para sua primeira venda, devolvemos 100% do investimento.</p>
                <p><strong>Porque assumimos todo o risco?</strong><br>Sabemos que o método funciona quando aplicado corretamente.</p>
            </div>
        </div>
    </section>

    <!-- Seção Oferta -->
    <section id="oferta">
        <div class="container">
            <h2>INVESTIMENTO</h2>
            
            <div class="pricing">
                <div class="price-old">De R$ 497,00</div>
                <div class="price-new">R$ 97,70</div>
                
                <!-- DESTAQUE MAIOR PARA O VALOR PARCELADO -->
                <div class="installment-highlight">
                    <div class="price-installments">12x de R$ 10,10</div>
                </div>
                
                <div class="bonus">Economia imediata de R$ 399,30</div>
                <p>Apenas para os primeiros 50 inscritos</p>
                
                <!-- BOTÃO ATUALIZADO COM LINK DA KIWIFY -->
                <a href="https://pay.kiwify.com.br/p3raEOE" class="btn btn-large" id="final-cta" target="_blank">GARANTIR MEU ACESSO COM 80% DE DESCONTO</a>
                
                <div class="payment-info">
                    <p>✅ Pagamento 100% Seguro | ✅ Acesso Imediato | ✅ Garantia de 7 Dias</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção FAQ -->
    <section class="section-light">
        <div class="container">
            <h2>PERGUNTAS FREQUENTES</h2>
            
            <div class="faq-item active">
                <div class="faq-question">Preciso ter produto próprio? <span>+</span></div>
                <div class="faq-answer">
                    <p>Não. Ensino a criar seu primeiro produto do zero em uma semana, com foco total em vendas.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Quanto tempo preciso dedicar? <span>+</span></div>
                <div class="faq-answer">
                    <p>As aulas são objetivas e focadas em prática de vendas. 30-45 minutos por dia são suficientes para ver resultados.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Preciso aparecer nas redes sociais? <span>+</span></div>
                <div class="faq-answer">
                    <p>Não. Ensino estratégias de vendas que funcionam sem necessidade de exposição. Você pode vender de forma discreta.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">O conteúdo é só sobre vendas? <span>+</span></div>
                <div class="faq-answer">
                    <p>Sim! 100% focado em técnicas práticas de vendas e anúncios para o digital, sem distrações.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Como recebo o acesso? <span>+</span></div>
                <div class="faq-answer">
                    <p>O acesso é imediato após a confirmação do pagamento. Você recebe login e senha por email.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-logo">
                <img src="https://www.dropbox.com/scl/fi/h54044utwgq09a5zda3ca/ChatGPT-Image-3-de-nov.-de-2025-10_20_00.png?rlkey=74xlanyd943o82qc3kfwgiiz6&st=aea0dolb&dl=1" alt="Método Venda Inicial" class="footer-logo-image">
            </div>
            <p><strong>Método Venda Inicial</strong> - Sua Jornada para a Primeira Venda Online</p>
            <p>© 2025 Método Venda Inicial. Todos os direitos reservados.</p>
            
            <div class="legal">
                <p><strong>Aviso Legal:</strong> "Resultados individuais variam conforme dedicação e aplicação do método. Não prometemos enriquecimento rápido. Prometemos um caminho realista para sua primeira venda online."</p>
            </div>
        </div>
    </footer>

    <script>
        // Contador regressivo de 20 minutos
        function startCountdown() {
            const countdownElement = document.getElementById('countdown');
            const headerCountdownElement = document.getElementById('header-countdown');
            let totalSeconds = 20 * 60; // 20 minutos em segundos
            
            function updateCountdown() {
                const minutes = Math.floor(totalSeconds / 60);
                const seconds = totalSeconds % 60;
                
                const countdownText = 
                    `${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
                
                countdownElement.textContent = countdownText;
                headerCountdownElement.textContent = countdownText;
                
                if (totalSeconds > 0) {
                    totalSeconds--;
                    setTimeout(updateCountdown, 1000);
                } else {
                    countdownElement.textContent = "00:00";
                    countdownElement.style.color = "#ff4d4d";
                    headerCountdownElement.textContent = "00:00";
                    headerCountdownElement.style.color = "#ff4d4d";
                }
            }
            
            updateCountdown();
        }
        
        // FAQ Toggle
        document.querySelectorAll('.faq-question').forEach(question => {
            question.addEventListener('click', () => {
                const item = question.parentNode;
                item.classList.toggle('active');
            });
        });
        
        // Rolagem suave para os botões de CTA
        document.querySelectorAll('a[href="#oferta"]').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Inicialização
        document.addEventListener('DOMContentLoaded', function() {
            startCountdown();
        });
    </script>
</body>
</html>
