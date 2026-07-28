<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cidade Vida Real HMO - Portal Oficial</title>
    <style>
        /* Reset e Estilos Globais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #121613;
            color: #e0e6ed;
            line-height: 1.6;
        }

        /* Cabeçalho */
        header {
            background: linear-gradient(180deg, #1b241e 0%, #0d120f 100%);
            border-bottom: 3px solid #4b6b42;
            padding: 2rem 1rem;
            text-align: center;
        }

        header h1 {
            font-size: 2.8rem;
            color: #6b8e23;
            text-transform: uppercase;
            letter-spacing: 3px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.8);
        }

        header p {
            font-size: 1.1rem;
            color: #a3b899;
            margin-top: 5px;
            font-weight: 600;
        }

        /* Menu Principal de Categorias */
        .menu-categorias {
            background-color: #161d18;
            display: flex;
            justify-content: center;
            gap: 12px;
            padding: 15px;
            flex-wrap: wrap;
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 2px solid #2e3d30;
        }

        .btn-categoria {
            background-color: #1f2921;
            color: #d1d8ce;
            border: 1px solid #4b6b42;
            font-weight: bold;
            padding: 10px 20px;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-transform: uppercase;
            font-size: 0.95rem;
        }

        .btn-categoria:hover, .btn-categoria.ativo {
            background-color: #4b6b42;
            color: #ffffff;
            box-shadow: 0 0 10px rgba(107, 142, 35, 0.5);
        }

        .btn-categoria.att-btn:hover, .btn-categoria.att-btn.ativo {
            background-color: #005580;
            border-color: #33bbff;
            box-shadow: 0 0 12px rgba(51, 187, 255, 0.6);
        }

        /* Container de Conteúdo */
        .container {
            max-width: 1050px;
            margin: 30px auto;
            padding: 0 15px;
        }

        /* Seções Principais */
        .conteudo-secao {
            display: none;
            background-color: #1a221c;
            border-left: 4px solid #4b6b42;
            padding: 25px;
            border-radius: 0 8px 8px 0;
            box-shadow: 0 4px 10px rgba(0,0,0,0.5);
        }

        .conteudo-secao.ativo {
            display: block;
            animation: fadeIn 0.4s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h2 {
            color: #8fae7c;
            margin-bottom: 20px;
            text-transform: uppercase;
            font-size: 1.6rem;
            border-bottom: 1px solid #2e3d30;
            padding-bottom: 8px;
        }

        /* Sub-Navegação interna de Profissões e Cargos */
        .sub-menu-profissoes {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-bottom: 25px;
            flex-wrap: wrap;
            background: #121813;
            padding: 12px;
            border-radius: 6px;
            border: 1px solid #2e3d30;
        }

        .btn-sub-prof {
            background-color: #18221a;
            color: #b0c0b0;
            border: 1px solid #2e3d30;
            padding: 8px 16px;
            border-radius: 4px;
            font-weight: bold;
            font-size: 0.9rem;
            cursor: pointer;
            transition: all 0.2s;
            text-transform: uppercase;
        }

        .btn-sub-prof:hover, .btn-sub-prof.ativo {
            background-color: #3b5434;
            color: #ffffff;
            border-color: #6b8e23;
        }

        .btn-sub-prof.sub-mafia:hover, .btn-sub-prof.sub-mafia.ativo {
            background-color: #8b0000;
            color: #ffffff;
            border-color: #ff3333;
            box-shadow: 0 0 10px rgba(255, 0, 0, 0.4);
        }

        /* Conteúdos Internos das Sub-Abas */
        .sub-conteudo {
            display: none;
        }

        .sub-conteudo.ativo {
            display: block;
            animation: fadeIn 0.3s ease-in-out;
        }

        /* ---------------------------------------------------- */
        /* ESTILOS EXCLUSIVOS DA SEÇÃO DE MÁFIA (TEMA CRIMINOSO) */
        /* ---------------------------------------------------- */
        .mafia-box {
            background: linear-gradient(135deg, rgba(20, 10, 10, 0.95), rgba(35, 12, 12, 0.95)),
                        url('https://images.unsplash.com/photo-1518709268805-4e9042af9f23?q=80&w=1000&auto=format&fit=crop') center/cover;
            border: 1px solid #ff2a2a;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 0 15px rgba(255, 0, 0, 0.2);
        }

        .mafia-box h3.titulo-mafia {
            color: #ff4d4d;
            border-bottom: 1px solid #5a1818;
            padding-bottom: 8px;
            margin-bottom: 15px;
            font-size: 1.4rem;
            text-transform: uppercase;
        }

        /* Sub-navegação dos Cargos da Máfia */
        .mafia-cargos-nav {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 25px;
            background: rgba(10, 0, 0, 0.6);
            padding: 12px;
            border-radius: 6px;
            border: 1px solid #441111;
        }

        .btn-cargo-mafia {
            background: #200808;
            color: #ffb3b3;
            border: 1px solid #661111;
            padding: 6px 12px;
            font-size: 0.85rem;
            font-weight: bold;
            border-radius: 4px;
            cursor: pointer;
            transition: all 0.2s;
        }

        .btn-cargo-mafia:hover, .btn-cargo-mafia.ativo {
            background: #990000;
            color: #ffffff;
            border-color: #ff4d4d;
            box-shadow: 0 0 8px rgba(255, 0, 0, 0.5);
        }

        /* Card do Cargo Exibido */
        .cargo-detalhe {
            display: none;
            background-color: rgba(15, 5, 5, 0.9);
            border: 1px solid #551111;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 25px;
            box-shadow: inset 0 0 15px rgba(0,0,0,0.8);
        }

        .cargo-detalhe.ativo {
            display: block;
            animation: fadeIn 0.3s ease-in-out;
        }

        .cargo-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            border-bottom: 1px solid #441111;
            padding-bottom: 10px;
            margin-bottom: 15px;
        }

        .cargo-header h3 {
            color: #ff3333;
            font-size: 1.3rem;
            text-transform: uppercase;
        }

        .cargo-badge {
            background-color: #660000;
            color: #ffcccc;
            padding: 4px 10px;
            border-radius: 12px;
            font-size: 0.85rem;
            font-weight: bold;
            border: 1px solid #aa0000;
        }

        .cargo-descricao {
            color: #ddcccc;
            margin-bottom: 15px;
            font-size: 1rem;
        }

        .comandos-box {
            background-color: #0a0303;
            border-left: 3px solid #ff3333;
            padding: 12px;
            border-radius: 4px;
        }

        .comandos-box h4 {
            color: #ff8080;
            font-size: 0.95rem;
            margin-bottom: 8px;
            text-transform: uppercase;
        }

        .comandos-box ul {
            list-style: none;
        }

        .comandos-box li {
            font-family: 'Courier New', Courier, monospace;
            color: #ffdddd;
            margin-bottom: 6px;
            font-size: 0.92rem;
        }

        .comandos-box code {
            color: #ff5555;
            font-weight: bold;
            background: #1a0505;
            padding: 2px 6px;
            border-radius: 3px;
        }

        /* Seção de Regras e Observações da Máfia */
        .regras-mafia-container {
            margin-top: 25px;
            background: rgba(15, 5, 5, 0.95);
            border: 1px solid #661111;
            padding: 20px;
            border-radius: 8px;
        }

        .regras-mafia-container h3 {
            color: #ff4d4d;
            margin-bottom: 15px;
            font-size: 1.1rem;
            text-transform: uppercase;
            border-bottom: 1px solid #441111;
            padding-bottom: 5px;
        }

        .regra-item {
            margin-bottom: 15px;
        }

        .regra-item h4 {
            color: #ff8080;
            font-size: 0.95rem;
            margin-bottom: 5px;
        }

        .regra-item ul {
            list-style: none;
            padding-left: 10px;
        }

        .regra-item li {
            color: #d8c0c0;
            font-size: 0.9rem;
            margin-bottom: 4px;
            position: relative;
            padding-left: 18px;
        }

        .regra-item li::before {
            content: "💀";
            position: absolute;
            left: 0;
            font-size: 0.75rem;
            top: 2px;
        }

        /* ---------------------------------------------------- */
        /* ESTILOS DA SEÇÃO DE ATUALIZAÇÕES (TEMA AZUL)       */
        /* ---------------------------------------------------- */
        #atualizacoes {
            border-left: 4px solid #33bbff;
        }

        #atualizacoes h2 {
            color: #33bbff;
            border-bottom: 1px solid #1a4d66;
        }

        .card-atualizacao {
            background-color: #121813;
            border: 1px solid #2e3d30;
            border-radius: 6px;
            padding: 20px;
            margin-bottom: 20px;
        }

        .att-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #2e3d30;
            padding-bottom: 8px;
            margin-bottom: 12px;
            flex-wrap: wrap;
        }

        .att-header h3 {
            color: #33bbff;
            font-size: 1.2rem;
        }

        .att-data {
            background-color: #00334e;
            color: #80d8ff;
            font-size: 0.8rem;
            font-weight: bold;
            padding: 3px 8px;
            border-radius: 4px;
            border: 1px solid #005580;
        }

        .att-lista {
            list-style: none;
        }

        .att-lista li {
            margin-bottom: 8px;
            font-size: 0.95rem;
            color: #cce6ff;
            padding-left: 20px;
            position: relative;
        }

        .att-lista li::before {
            content: "⚡";
            position: absolute;
            left: 0;
        }

        /* Grids Genéricos */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 15px;
            margin-top: 15px;
        }

        .card {
            background-color: #121813;
            padding: 18px;
            border-radius: 6px;
            border: 1px solid #2e3d30;
        }

        .card h3 {
            color: #6b8e23;
            margin-bottom: 8px;
            font-size: 1.15rem;
        }

        .card p {
            font-size: 0.92rem;
            color: #b0c0b0;
        }

        .governo-card h3 {
            color: #5bc0de;
        }
    </style>
</head>
<body>

    <!-- Cabeçalho Principal -->
    <header>
        <h1>Exército HMO</h1>
        <p>Forças Armadas da Cidade HMO - Informações do servidor Cidade Vida Real HMO</p>
    </header>

    <!-- Menu Principal Superior -->
    <div class="menu-categorias">
        <button class="btn-categoria ativo" onclick="abrirAba('profissoes-cargos', this)">💼 Profissões & Cargos</button>
        <button class="btn-categoria att-btn" onclick="abrirAba('atualizacoes', this)">⚡ Atualizações</button>
    </div>

    <!-- Áreas de Conteúdo -->
    <div class="container">

        <!-- 1. SEÇÃO PRINCIPAL: PROFISSÕES & CARGOS -->
        <section id="profissoes-cargos" class="conteudo-secao ativo">
            <h2>💼 Guia Geral de Profissões e Cargos</h2>
            <p style="margin-bottom: 20px; color: #a3b899;">Escolha abaixo a área desejada para explorar os detalhes das profissões, facções do crime ou forças do governo:</p>

            <!-- Sub-Menu das 3 Categorias -->
            <div class="sub-menu-profissoes">
                <button class="btn-sub-prof ativo" onclick="abrirSubAba('sub-honestas', this)">Profissões Honestas</button>
                <button class="btn-sub-prof sub-mafia" onclick="abrirSubAba('sub-mafia', this)">🔴 Máfia & Crimes</button>
                <button class="btn-sub-prof" onclick="abrirSubAba('sub-governo', this)">Governo & Serviços</button>
            </div>

            <!-- SUB-ABA 1: PROFISSÕES HONESTAS -->
            <div id="sub-honestas" class="sub-conteudo ativo">
                <h3 style="color: #8fae7c; margin-bottom: 10px;">💼 Profissões Honestas</h3>
                <p>Trabalhe honestamente na cidade, ganhe seu salário, quite suas propriedades e suba na vida legalmente!</p>
                
                <div class="cards-grid">
                    <div class="card">
                        <h3>🚛 Caminhoneiro</h3>
                        <p>Transporte cargas de suprimentos e combustível por todo o mapa de San Andreas.</p>
                    </div>
                    <div class="card">
                        <h3>🚌 Motorista de Ônibus</h3>
                        <p>Faça as rotas urbanas e intermunicipais levando passageiros com segurança.</p>
                    </div>
                    <div class="card">
                        <h3>🌾 Agricultor / Fazendeiro</h3>
                        <p>Cultive, colha e forneça matéria-prima para as indústrias e comércios da cidade.</p>
                    </div>
                    <div class="card">
                        <h3>📦 Entregador</h3>
                        <p>Realize entregas rápidas de encomendas e comida usando veículos leves.</p>
                    </div>
                </div>
            </div>

            <!-- SUB-ABA 2: MÁFIA & CRIMES -->
            <div id="sub-mafia" class="sub-conteudo">
                <div class="mafia-box">
                    <h3 class="titulo-mafia">🔴 Sistema de Máfia — Cargos e Mecânicas</h3>
                    <p style="color: #e6b8b8; margin-bottom: 15px;">Selecione um cargo abaixo para visualizar o nível necessário, descrição e todos os comandos liberados:</p>

                    <!-- Abas dos 11 Cargos -->
                    <div class="mafia-cargos-nav">
                        <button class="btn-cargo-mafia ativo" onclick="mostrarCargo('cargo-1', this)">1. Traficante de Drogas</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-2', this)">2. Traficante de Armas</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-3', this)">3. Plantador de Maconha</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-4', this)">4. Produtor de Drogas</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-5', this)">5. Transp. de Drogas</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-6', this)">6. Transp. de Armas</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-7', this)">7. Ladrão de Carros</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-8', this)">8. Assaltante</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-9', this)">9. Sequestrador</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-10', this)">10. Terrorista</button>
                        <button class="btn-cargo-mafia" onclick="mostrarCargo('cargo-11', this)">11. Chefão do Crime</button>
                    </div>

                    <!-- Fichas dos Cargos -->
                    <div id="cargo-1" class="cargo-detalhe ativo">
                        <div class="cargo-header">
                            <h3>1. Traficante de Drogas</h3>
                            <span class="cargo-badge">Nível Necessário: 10 | Salário: N/A</span>
                        </div>
                        <p class="cargo-descricao">Especialista em comercialização de substâncias ilícitas. Pode realizar vendas diretamente para NPCs (bots) ou para outros jogadores espalhados pelo mapa.</p>
                        <div class="comandos-box">
                            <h4>📜 Comandos do Cargo:</h4>
                            <ul>
                                <li><code>/verdrogas</code> — Exibe o tipo e a quantidade de drogas no inventário.</li>
                                <li><code>/venderdrogabot</code> — Realiza a venda de drogas para o NPC mais próximo.</li>
                                <li><code>/venderdroga [id] [valor]</code> — Oferece e vende drogas para um jogador específico.</li>
                            </ul>
                        </div>
                    </div>

                    <div id="cargo-2" class="cargo-detalhe">
                        <div class="cargo-header">
                            <h3>2. Traficante de Armas</h3>
                            <span class="cargo-badge">Nível Necessário: 20 | Salário: N/A</span>
                        </div>
                        <p class="cargo-descricao">Armador clandestino responsável pelo mercado negro. Comercializa armamentos sem registro para jogadores e NPCs.</p>
                        <div class="comandos-box">
                            <h4>📜 Comandos do Cargo:</h4>
                            <ul>
                                <li><code>/verarmas</code> — Exibe o tipo e a quantidade de armas no inventário.</li>
                                <li><code>/venderarmabot</code> — Realiza a venda de armamentos para o NPC mais próximo.</li>
                                <li><code>/venderarma [id] [valor]</code> — Oferece e vende armamentos para um jogador específico.</li>
                            </ul>
                        </div>
                    </div>

                    <div id="cargo-3" class="cargo-detalhe">
                        <div class="cargo-header">
                            <h3>3. Plantador de Maconha</h3>
                            <span class="cargo-badge">Nível Necessário: 30 | Salário: N/A</span>
                        </div>
                        <p class="cargo-descricao">Responsável pelo cultivo e manejo agrícola de maconha, garantindo o suprimento primário da rede de tráfico.</p>
                        <div class="comandos-box">
                            <h4>📜 Comandos do Cargo:</h4>
                            <ul>
                                <li><code>/plantarmaconha</code> — Inicia o plantio no local.</li>
                                <li><code>/colhermaconha</code> — Realiza a colheita da plantação pronta.</li>
                            </ul>
                        </div>
                    </div>

                    <div id="cargo-4" class="cargo-detalhe">
                        <div class="cargo-header">
                            <h3>4. Produtor de Drogas</h3>
                            
