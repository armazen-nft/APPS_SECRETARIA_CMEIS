📘 Projeto GitHub: APPs_SECRETARIAS
🎯 Visão Geral
APPs_SECRETARIAS é uma coleção de aplicações web open source, offline-first e gratuitas desenvolvidas em HTML/CSS/JS puro (JavaScript vanilla). O projeto nasceu para atender secretários escolares da rede pública, especialmente os municípios que seguem legislações como a LDBEN 9.394/96, Deliberações do CEE/PR, e normativas do FNDE. Todos os apps funcionam sem internet, armazenam dados no localStorage do navegador e rodam em qualquer computador (Windows, Linux, Chromebook) – basta abrir o arquivo .html.

📦 Repositório no GitHub
Nome sugerido: APPs_SECRETARIAS

Descrição curta: Aplicativos offline para secretarias escolares – Matrículas (Educação Infantil) + Gestão Nutricional (MAPA CMEI). Código aberto, gratuito, baseado em legislação brasileira.

Licença: MIT (permissiva, incentiva adoção e customização)

Idioma: Português (com possibilidade de internacionalização futura)

🧩 Aplicativos incluídos (versão inicial)
1. 📋 APP-MATRÍCULAS – Educação Infantil
Finalidade: Gerenciar matrículas, vagas, lista de espera, vagas judiciais e controle de período (manhã/tarde/integral) para turmas do Infantil I ao V.

Principais funcionalidades:

✅ Definição do ano letivo (regra de corte 31/03 conforme CNE/CEB nº5/2009)

✅ Configuração do limite de alunos por turma (respeitando Del. CEE/PR 02/2014)

✅ Controle de vagas sobressalentes (até 10 por turma) e vagas judiciais (até 30 alunos)

✅ Lista de espera com expiração automática em 72 horas

✅ Consulta pública de vagas por data de nascimento (calcula idade no corte)

✅ Tabelas de alunos com campos: CGM, nome completo, data de nascimento, status (salvo/espera/vazio/judicial)

✅ Relatório geral impresso (resumo por série, turma, período)

✅ Base legal integrada (LDBEN, CNE/CEB, Pareceres, SERE/RCO, TC-PR)

Público-alvo: Secretários de escolas de Educação Infantil, diretores, equipe pedagógica.

2. 🥗 MAPA DE CMEI – Gestão Nutricional
Finalidade: Substituir planilhas manuais e papers para controle de estoque (básicos + carnes + vegetais), cardápio diário, consumo de alunos (F1) e lançamento de notas fiscais (N1 a N50).

Principais funcionalidades:

✅ Identificação do CMEI, mês/ano e dias letivos

✅ Registro diário de alunos nas refeições (café, almoço, lanche, jantar) e consumo de produtos básicos (Kg/Un)

✅ Cálculo automático das Saídas no estoque de básicos a partir do consumo da F1

✅ Aba Cálculo de Notas Fiscais: lança quantidades por NF (N1 a N50) para vegetais e carnes; automaticamente alimenta Entradas do V1 (carnes) e V2 (vegetais)

✅ Estoque V1 (básicos + carnes) e V2 (perecíveis) com saldo atual, alertas de saldo negativo

✅ Cardápio textual por dia/refeição (campo livre)

✅ Relatório final consolidado + detecção de divergências (saldos negativos)

✅ Ferramenta de correção pontual (ajusta saldo anterior, entradas ou saídas)

✅ Exportação para XLSX (espelho completo: planilhas F1, V1, F2, V2, Cálculo de Notas)

✅ Impressão amigável (PDF via window.print())

Público-alvo: Merendeiras, nutricionistas, diretores de CMEI, secretários escolares responsáveis pela prestação de contas.

🛠️ Tecnologias & Requisitos
Frontend puro: HTML5, CSS3 (flex/grid), JavaScript ES6+

Armazenamento: localStorage (permanece entre sessões)

Exportação XLSX: Biblioteca xlsx (CDN via SheetJS) – funciona offline após primeiro carregamento

Sem back-end, sem banco de dados, sem instalação – basta um navegador moderno (Chrome, Edge, Firefox, Safari)

100% offline depois de baixado (pode ser usado em escolas sem internet)

🚀 Como usar (instalação zero)
Acesse o repositório GitHub e faça o download dos arquivos .html (ou clone o repositório)

Coloque os arquivos em uma pasta local, em um pendrive, ou em um servidor interno da secretaria

Dê duplo clique no arquivo desejado (SISTEMA_DE_GERENCIAMENTO_DE_MATRICULA.html ou SISTEMA_DE_GESTAO_NUTRICIONAL.html)

O aplicativo abrirá no navegador padrão – todos os dados ficam salvos no próprio computador

Para compartilhar dados entre máquinas, exporte o relatório XLSX ou use a função "imprimir" e salve em PDF

⚠️ Importante: Nunca exclua os dados de navegação (localStorage) sem fazer um backup via exportação XLSX.

📁 Estrutura do repositório (sugestão)
text
APPs_SECRETARIAS/
├── README.md
├── LICENSE (MIT)
├── docs/
│   ├── manual_matriculas.pdf
│   └── manual_nutricao.pdf
├── apps/
│   ├── sistema_matriculas.html
│   ├── sistema_nutricional.html
├── assets/
│   ├── logo_secretaria.png
│   └── print_screens/
└── CONTRIBUTING.md
🧪 Contribuição e customização
O projeto é 100% aberto e qualquer secretário, desenvolvedor ou estudante pode:

Adaptar as cores/logo para a rede municipal

Incluir novas séries, produtos ou alterar limites legais (tudo em arrays JavaScript)

Traduzir para outros idiomas

Melhorar a lógica de expiração de espera ou relatórios

Adicionar suporte a múltiplas unidades escolares (via import/export de JSON)

Como contribuir:

Faça um fork do repositório

Crie um branch (git checkout -b feature/nova-funcionalidade)

Teste as alterações em ambiente offline

Abra um Pull Request com descrição clara

🔒 Segurança e conformidade
Os dados nunca saem do computador do usuário (sem telemetria, sem analytics)

Não há coleta de informações pessoais

O código segue as normas educacionais brasileiras, mas cada município deve validar os parâmetros (limites de alunos, datas de corte, períodos)

Sugere-se manter o ano letivo configurado corretamente antes de iniciar as matrículas

🛣️ Roadmap (ideias futuras)
Modo multi-escola (selecionar CMEI/EMEB no início)

Exportar banco de dados completo para JSON (backup/restauração)

Gerar etiquetas para crachás de alunos (matrícula)

Integração opcional com impressoras térmicas de relatórios de estoque

Versão PWA (instalável como app no celular/tablet)

Módulo de frequência (diário de classe simplificado)

Dashboard com gráficos (uso de gêneros, ocupação de vagas)

👥 Mantenedores & contato
Projeto idealizado e desenvolvido pela comunidade de secretários escolares de Piraquara–PR e aberto para adoção nacional.
GitHub issues para reportar bugs ou sugerir melhorias.
Repositório oficial: https://github.com/seu-usuario/APPs_SECRETARIAS (substitua pelo link real)

📄 Exemplo de README (trecho para colocar no GitHub)
markdown
# APPs_SECRETARIAS – Gestão Escolar Offline

![Licença MIT](https://img.shields.io/badge/licença-MIT-green)
![Status](https://img.shields.io/badge/status-estável-brightgreen)
![Plataforma](https://img.shields.io/badge/plataforma-Web_Offline-blue)

Aplicativos web gratuitos e open source para secretarias escolares.  
**Nenhuma internet necessária – rode direto do seu computador.**

## ✅ Apps disponíveis
- **Matrículas Educação Infantil** – Controle de vagas, lista de espera, turmas, judicial e período.
- **Gestão Nutricional (MAPA CMEI)** – Estoque, consumo diário, cardápio, notas fiscais e relatórios.

## 📥 Download
Baixe os arquivos `.html` da pasta [`/apps`](./apps) e abra no navegador.

## 📚 Documentação
Veja os manuais em [`/docs`](./docs).

## 🤝 Como contribuir
Leia [`CONTRIBUTING.md`](./CONTRIBUTING.md). Toda ajuda é bem-vinda!

## 🧾 Licença
MIT – use, modifique e distribua livremente, mantendo os créditos.
💡 Conclusão
O projeto APPs_SECRETARIAS entrega duas ferramentas robustas, prontas para uso imediato, que resolvem problemas reais do dia a dia de secretários escolares:

Organização de matrículas com base legal

Controle de estoque e alimentação escolar integrado com notas fiscais

Por serem offline, gratuitas e de código aberto, eliminam barreiras de custo e dependência de internet, promovendo autonomia e eficiência nas secretarias municipais. É um convite para a comunidade contribuir, adaptar e espalhar soluções que valorizam o serviço público.# APPS_SECRETARIA_CMEIS
Aplicativos Open Source facilitadores das tarefas em Secretarias

APP SISTEMA DE GERENCIAMENTO DE MATRÍCULAS
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>APP-MATRÍCULAS — Educação Infantil</title>
<style>
  :root {
    --verde: #1a5c38; --verde-claro: #2e7d52; --verde-bg: #e8f5ee;
    --azul: #1a3a5c; --amarelo: #f5a623; --cinza: #f4f4f2;
    --cinza-borda: #d0d0cc; --texto: #1a1a18; --texto-muted: #555550;
    --branco: #ffffff; --perigo: #c0392b; --espera: #e67e22; --salvo: #1a5c38;
    --roxo: #6c3483;
    --fonte-titulo: 'Georgia', serif;
    --fonte-corpo: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    --sombra: 0 2px 8px rgba(0,0,0,0.10); --raio: 8px;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: var(--fonte-corpo); background: #eef2ee; color: var(--texto); min-height: 100vh; }

  /* HEADER */
  #header { background: linear-gradient(135deg, var(--verde) 0%, var(--azul) 100%); color: white; position: sticky; top: 0; z-index: 100; box-shadow: 0 2px 12px rgba(0,0,0,0.25); }
  #header-top { display: flex; align-items: center; gap: 16px; padding: 12px 24px; }
  #header-logo { width: 54px; height: 54px; background: white; border-radius: 50%; display: flex; align-items: center; justify-content: center; flex-shrink: 0; }
  #header-logo svg { width: 38px; height: 38px; }
  #header-titulo h1 { font-family: var(--fonte-titulo); font-size: 17px; font-weight: bold; letter-spacing: 0.5px; }
  #header-titulo p { font-size: 11px; opacity: 0.85; margin-top: 2px; }
  #header-nav { background: rgba(0,0,0,0.15); display: flex; gap: 0; overflow-x: auto; }
  .nav-btn { background: none; border: none; color: rgba(255,255,255,0.85); padding: 10px 18px; cursor: pointer; font-size: 13px; font-weight: 500; white-space: nowrap; border-bottom: 3px solid transparent; transition: all 0.2s; }
  .nav-btn:hover, .nav-btn.ativo { color: white; border-bottom-color: var(--amarelo); background: rgba(255,255,255,0.08); }

  /* TELAS */
  .tela { display: none; padding: 20px 24px; max-width: 1100px; margin: 0 auto; }
  .tela.ativa { display: block; }

  /* CARDS */
  .card { background: var(--branco); border-radius: var(--raio); box-shadow: var(--sombra); margin-bottom: 20px; border: 1px solid var(--cinza-borda); }
  .card-header { background: var(--verde); color: white; padding: 12px 18px; border-radius: var(--raio) var(--raio) 0 0; font-weight: bold; font-size: 15px; display: flex; align-items: center; gap: 8px; }
  .card-body { padding: 16px 18px; }

  /* ALERTA LEGAL */
  .alerta-legal { background: #fff8e1; border: 1px solid #f5a623; border-left: 5px solid #f5a623; border-radius: var(--raio); padding: 12px 16px; margin-bottom: 16px; font-size: 13px; }
  .alerta-legal strong { display: block; margin-bottom: 4px; color: #7a5000; }

  /* SÉRIES */
  .series-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 14px; margin-bottom: 20px; }
  .serie-card { background: var(--branco); border: 2px solid var(--cinza-borda); border-radius: var(--raio); padding: 16px; text-align: center; cursor: pointer; transition: all 0.2s; }
  .serie-card:hover { border-color: var(--verde); transform: translateY(-2px); box-shadow: var(--sombra); }
  .serie-card.ativa { border-color: var(--verde); background: var(--verde-bg); }
  .serie-numeral { font-family: var(--fonte-titulo); font-size: 36px; color: var(--verde); font-weight: bold; }
  .serie-nome { font-size: 13px; color: var(--texto-muted); margin-top: 4px; }
  .badge { display: inline-block; padding: 2px 8px; border-radius: 12px; font-size: 11px; font-weight: bold; margin: 2px; }
  .badge-verde { background: #e8f5ee; color: var(--verde); }
  .badge-amarelo { background: #fff3e0; color: #7a5000; }
  .badge-cinza { background: #f0f0f0; color: #666; }
  .badge-completa { background: var(--verde); color: white; }
  .badge-roxo { background: #f3e5f5; color: var(--roxo); }

  /* TURMAS TABS */
  .turmas-tabs { display: flex; gap: 8px; margin-bottom: 16px; flex-wrap: wrap; }
  .turma-tab { padding: 8px 20px; border: 2px solid var(--cinza-borda); border-radius: 20px; cursor: pointer; font-weight: bold; font-size: 14px; background: var(--branco); transition: all 0.2s; }
  .turma-tab:hover { border-color: var(--verde); }
  .turma-tab.ativa { background: var(--verde); color: white; border-color: var(--verde); }
  .turma-tab.completa { background: var(--azul); color: white; border-color: var(--azul); }

  /* PERÍODO BOTÕES */
  .periodo-grupo { display: flex; gap: 6px; align-items: center; flex-wrap: wrap; }
  .btn-periodo { border: 2px solid var(--cinza-borda); border-radius: 20px; padding: 6px 16px; cursor: pointer; font-size: 13px; font-weight: 600; background: var(--branco); transition: all 0.2s; }
  .btn-periodo:hover { border-color: var(--azul); }
  .btn-periodo.ativo-manha { background: #fff9c4; border-color: #f9a825; color: #7a5000; }
  .btn-periodo.ativo-tarde { background: #e3f2fd; border-color: #1565c0; color: #1565c0; }
  .btn-periodo.ativo-integral { background: #f3e5f5; border-color: var(--roxo); color: var(--roxo); }

  /* TABELA ALUNOS */
  .tabela-wrapper { overflow-x: auto; }
  table.alunos { width: 100%; border-collapse: collapse; font-size: 13px; }
  table.alunos th { background: var(--verde); color: white; padding: 9px 10px; text-align: left; font-weight: 600; white-space: nowrap; }
  table.alunos td { padding: 6px 8px; border-bottom: 1px solid #eee; vertical-align: middle; }
  table.alunos tr:hover td { background: #f9fff9; }
  table.alunos tr.linha-espera td { background: #fff8f0; }
  table.alunos tr.linha-salva td { background: #f0fff5; }
  table.alunos tr.linha-judicial td { background: #fdf3ff; }

  input.campo-aluno { width: 100%; border: 1px solid var(--cinza-borda); border-radius: 5px; padding: 5px 8px; font-size: 13px; font-family: inherit; background: white; }
  input.campo-aluno:disabled { background: #f8f8f8; color: var(--texto); border-color: transparent; }
  input.campo-aluno:focus { outline: 2px solid var(--verde); }

  .num-linha { font-weight: bold; color: var(--texto-muted); text-align: center; min-width: 28px; }
  .status-dot { width: 10px; height: 10px; border-radius: 50%; display: inline-block; }
  .dot-vazio { background: #ddd; }
  .dot-espera { background: var(--espera); }
  .dot-salvo { background: var(--salvo); }
  .dot-judicial { background: var(--roxo); }

  /* BOTÕES */
  .btn { border: none; border-radius: 5px; padding: 5px 11px; cursor: pointer; font-size: 12px; font-weight: 600; transition: all 0.15s; }
  .btn:active { transform: scale(0.96); }
  .btn-salvar { background: var(--verde); color: white; }
  .btn-salvar:hover { background: var(--verde-claro); }
  .btn-corrigir { background: #2980b9; color: white; }
  .btn-corrigir:hover { background: #3498db; }
  .btn-deletar { background: var(--perigo); color: white; }
  .btn-deletar:hover { background: #e74c3c; }
  .btn-acoes { display: flex; gap: 4px; white-space: nowrap; }

  .btn-grande { padding: 10px 22px; font-size: 14px; border-radius: var(--raio); border: none; cursor: pointer; font-weight: bold; transition: all 0.2s; }
  .btn-verde-g { background: var(--verde); color: white; }
  .btn-verde-g:hover { background: var(--verde-claro); }
  .btn-completa { background: var(--azul); color: white; border: none; border-radius: var(--raio); padding: 9px 16px; cursor: pointer; font-weight: bold; font-size: 13px; transition: all 0.2s; }
  .btn-completa.marcada { background: #777; }

  /* BOTÃO ADICIONAR LINHA JUDICIAL */
  .btn-add-judicial { background: var(--roxo); color: white; border: none; border-radius: var(--raio); padding: 10px 20px; cursor: pointer; font-weight: bold; font-size: 13px; width: 100%; margin-top: 8px; transition: all 0.2s; }
  .btn-add-judicial:hover { background: #7d3c98; }
  .btn-add-judicial:disabled { background: #ccc; cursor: not-allowed; }

  /* CONSULTA */
  .consulta-box { background: var(--branco); border-radius: var(--raio); padding: 24px; box-shadow: var(--sombra); max-width: 480px; margin: 0 auto 24px; text-align: center; }
  .consulta-box h2 { color: var(--verde); margin-bottom: 8px; font-family: var(--fonte-titulo); }
  .consulta-box p { color: var(--texto-muted); font-size: 14px; margin-bottom: 18px; }
  .input-grande { width: 100%; padding: 12px 16px; font-size: 18px; border: 2px solid var(--cinza-borda); border-radius: var(--raio); text-align: center; font-family: inherit; margin-bottom: 12px; }
  .input-grande:focus { outline: none; border-color: var(--verde); }
  .resultado-consulta { margin-top: 20px; padding: 16px; border-radius: var(--raio); border: 1px solid var(--cinza-borda); text-align: left; }
  .resultado-disponivel { background: var(--verde-bg); border-color: var(--verde); }
  .resultado-espera { background: #fff8f0; border-color: var(--espera); }
  .resultado-indisponivel { background: #fff0f0; border-color: var(--perigo); }

  /* CONFIG */
  .config-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 16px; }
  .config-item { padding: 14px; background: var(--cinza); border-radius: var(--raio); }
  .config-item label { font-size: 13px; color: var(--texto-muted); display: block; margin-bottom: 6px; font-weight: 600; }
  .config-item input { width: 100%; padding: 8px 10px; border: 1px solid var(--cinza-borda); border-radius: 5px; font-size: 15px; font-family: inherit; }

  /* RESUMO */
  .resumo-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(140px, 1fr)); gap: 12px; margin-bottom: 20px; }
  .resumo-card { background: var(--branco); border-radius: var(--raio); padding: 14px; border: 1px solid var(--cinza-borda); text-align: center; }
  .resumo-numero { font-size: 30px; font-weight: bold; font-family: var(--fonte-titulo); }

  /* MODAL */
  .modal-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.5); z-index: 999; display: none; align-items: center; justify-content: center; }
  .modal-overlay.aberto { display: flex; }
  .modal { background: white; border-radius: var(--raio); padding: 24px; max-width: 420px; width: 90%; box-shadow: 0 8px 32px rgba(0,0,0,0.3); }
  .modal h3 { color: var(--verde); margin-bottom: 12px; font-family: var(--fonte-titulo); }
  .modal p { font-size: 14px; color: var(--texto-muted); margin-bottom: 16px; }
  .modal-btns { display: flex; gap: 10px; justify-content: flex-end; }

  /* LEGENDA */
  .legenda { display: flex; gap: 16px; flex-wrap: wrap; margin-bottom: 10px; font-size: 12px; align-items: center; }
  .legenda-item { display: flex; align-items: center; gap: 5px; }
  .timer-espera { font-size: 11px; color: var(--espera); font-weight: bold; white-space: nowrap; }

  /* RODAPÉ */
  #rodape { text-align: center; padding: 16px; font-size: 11px; color: var(--texto-muted); margin-top: 30px; border-top: 1px solid var(--cinza-borda); background: var(--branco); }

  @media (max-width: 600px) {
    .tela { padding: 12px; } table.alunos { font-size: 11px; } .btn { padding: 4px 7px; font-size: 11px; } .serie-numeral { font-size: 28px; }
  }
</style>
</head>
<body>

<div id="header">
  <div id="header-top">
    <div id="header-logo">
      <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
        <rect x="4" y="8" width="32" height="24" rx="3" fill="#1a5c38"/>
        <rect x="8" y="12" width="10" height="8" rx="1" fill="white"/>
        <rect x="22" y="12" width="10" height="4" rx="1" fill="white"/>
        <rect x="22" y="18" width="7" height="2" rx="1" fill="#a0d4b8"/>
        <rect x="8" y="22" width="24" height="2" rx="1" fill="#a0d4b8"/>
        <rect x="8" y="26" width="18" height="2" rx="1" fill="#a0d4b8"/>
        <circle cx="32" cy="10" r="6" fill="#f5a623"/>
        <text x="28.5" y="13.5" font-size="8" fill="white" font-weight="bold">M</text>
      </svg>
    </div>
    <div id="header-titulo">
      <h1>APP-MATRÍCULAS</h1>
      <p>Gestão de Matrículas • Educação Infantil • Piraquara–PR • Sistema Offline</p>
    </div>
  </div>
  <nav id="header-nav">
    <button class="nav-btn ativo" onclick="mostrarTela('tela-consulta', this)">🔍 Consultar Vagas</button>
    <button class="nav-btn" onclick="mostrarTela('tela-series', this)">📚 Turmas e Matrículas</button>
    <button class="nav-btn" onclick="mostrarTela('tela-config', this)">⚙️ Configurar Turmas</button>
    <button class="nav-btn" onclick="mostrarTela('tela-relatorio', this)">📊 Relatório Geral</button>
    <button class="nav-btn" onclick="mostrarTela('tela-legal', this)">⚖️ Base Legal</button>
  </nav>
</div>

<!-- TELA CONSULTA -->
<div id="tela-consulta" class="tela ativa">
  <div class="consulta-box">
    <h2>Consultar Disponibilidade de Vagas</h2>
    <p>Digite a data de nascimento para verificar vagas conforme faixa etária (LDBEN Art. 29-31 e corte 31/03)</p>
    <input type="date" id="input-datanasc" class="input-grande" oninput="consultarVaga()">
    <div id="badge-ano-letivo-consulta" style="margin-bottom:10px"></div>
    <button class="btn-grande btn-verde-g" onclick="consultarVaga()" style="width:100%">Verificar Disponibilidade</button>
    <div id="resultado-consulta"></div>
  </div>
  <div class="card">
    <div class="card-header">📋 Situação Atual das Turmas</div>
    <div class="card-body"><div id="painel-resumo-geral"></div></div>
  </div>
</div>

<!-- TELA TURMAS E MATRÍCULAS -->
<div id="tela-series" class="tela">
  <div class="alerta-legal">
    <strong>⚖️ Base Legal:</strong>
    LDBEN 9.394/1996 Art. 29-31 | CNE/CEB 5/2009 | Del. CEE/PR 02/2014 | SERE/SEED-PR | RCO | TC-PR. Corte etário: 31/03.
  </div>
  <div id="painel-series"></div>
  <div id="painel-turmas" style="display:none">
    <div class="card">
      <div class="card-header" id="titulo-turma">Turmas</div>
      <div class="card-body">
        <div class="turmas-tabs" id="tabs-turmas"></div>
        <div id="conteudo-turma"></div>
      </div>
    </div>
  </div>
</div>

<!-- TELA CONFIGURAR -->
<div id="tela-config" class="tela">

  <!-- BLOCO ANO LETIVO -->
  <div class="card">
    <div class="card-header">📅 Ano Letivo de Referência</div>
    <div class="card-body">
      <div class="alerta-legal" style="margin-bottom:14px">
        <strong>⚠️ Por que isso importa?</strong>
        A data de corte para classificação etária é <strong>31 de março do ano letivo</strong> (Resolução CNE/CEB nº 5/2009 e Parecer CNE/CEB nº 6/2010). Se o sistema for usado em dezembro para planejar o ano seguinte, o ano aqui deve ser ajustado — caso contrário, crianças nascidas entre abril e dezembro serão classificadas na série errada.
      </div>
      <div style="display:flex;align-items:center;gap:16px;flex-wrap:wrap">
        <div>
          <label style="font-size:13px;font-weight:600;color:var(--texto-muted);display:block;margin-bottom:6px">Ano Letivo (corte: 31/03/ANO)</label>
          <input type="number" id="cfg-ano-letivo" min="2020" max="2099" style="font-size:22px;font-weight:bold;width:120px;padding:8px 12px;border:2px solid var(--verde);border-radius:var(--raio);color:var(--verde);text-align:center">
        </div>
        <div id="cfg-corte-preview" style="font-size:13px;color:var(--texto-muted);padding:10px 16px;background:var(--cinza);border-radius:var(--raio);line-height:1.6"></div>
      </div>
      <div style="margin-top:14px">
        <button class="btn-grande btn-verde-g" onclick="salvarAnoLetivo()">💾 Salvar Ano Letivo</button>
      </div>
    </div>
  </div>

  <!-- BLOCO VAGAS POR TURMA -->
  <div class="card">
    <div class="card-header">⚙️ Configurar N° de Alunos por Turma</div>
    <div class="card-body">
      <div class="alerta-legal" style="margin-bottom:16px">
        <strong>ℹ️ Como funciona:</strong>
        Defina abaixo o número de vagas de cada turma. Após salvar, a aba "Turmas e Matrículas" atualizará o número de células automaticamente. Limites conforme Del. CEE/PR 02/2014: I-II até 12; III até 15; IV-V até 20.
      </div>
      <div class="config-grid" id="config-grid"></div>
      <div style="margin-top:20px;display:flex;gap:12px;flex-wrap:wrap;">
        <button class="btn-grande btn-verde-g" onclick="salvarConfig()">💾 Salvar e Aplicar nas Turmas</button>
        <button class="btn-grande" style="background:#eee;color:#333" onclick="restaurarPadroes()">↺ Restaurar Padrões</button>
      </div>
    </div>
  </div>
</div>

<!-- TELA RELATÓRIO -->
<div id="tela-relatorio" class="tela">
  <div class="card">
    <div class="card-header">📊 Relatório Geral — Educação Infantil Piraquara</div>
    <div class="card-body" id="corpo-relatorio"></div>
  </div>
  <div style="text-align:center;margin-top:12px;">
    <button class="btn-grande btn-verde-g" onclick="window.print()">🖨️ Imprimir Relatório</button>
  </div>
</div>

<!-- TELA BASE LEGAL -->
<div id="tela-legal" class="tela">
  <div class="card">
    <div class="card-header">⚖️ Normativas e Base Legal</div>
    <div class="card-body" style="display:grid;gap:14px">
      <div class="alerta-legal"><strong>📖 Lei Federal nº 9.394/1996 — LDBEN</strong>Art. 29: Educação Infantil como primeira etapa da Educação Básica. Art. 30: Creches (0–3 anos) e pré-escolas (4–5 anos). Art. 31: Avaliação mediante acompanhamento e registro.</div>
      <div class="alerta-legal"><strong>📖 Resolução CNE/CEB nº 5/2009 — DCNEI</strong>Diretrizes Curriculares Nacionais. Define faixas etárias e critérios de matrícula. Corte etário: 31 de março do ano letivo.</div>
      <div class="alerta-legal"><strong>📖 Parecer CNE/CEB nº 6/2010</strong>Crianças que completam 4 anos até 31/03 devem ser matriculadas na pré-escola obrigatoriamente.</div>
      <div class="alerta-legal"><strong>📖 Deliberação CEE/PR nº 02/2014</strong>Normas para Educação Infantil no Paraná. Turmas: I e II até 12; III até 15; IV e V até 20 alunos.</div>
      <div class="alerta-legal"><strong>📖 Portal SERE — Seed-PR</strong>Sistema Estadual de Registro Escolar. Base para CGM, matrícula e frequência. Dados devem ser migrados ao SERE pelo responsável.</div>
      <div class="alerta-legal"><strong>📖 RCO — Registro de Classe Online</strong>Substitui o diário físico. Matrículas confirmadas devem ser lançadas no RCO conforme calendário letivo.</div>
      <div class="alerta-legal"><strong>📖 TC-PR — Tribunal de Contas do Paraná</strong>Fiscaliza gestão educacional municipal via SIOPE e relatórios periódicos.</div>
      <div class="alerta-legal"><strong>📖 Vagas Judiciais (MP / Conselho Tutelar)</strong>Determinações judiciais do Ministério Público ou Conselho Tutelar podem obrigar a escola a matricular além do limite legal. Registre com o botão "Adicionar Vaga Judicial" disponível em cada turma (até 30 alunos total).</div>
      <div class="alerta-legal"><strong>📖 Espera Prioritária — 72 horas</strong>Alunos inseridos mas não confirmados ficam em espera prioritária por 72h com vaga reservada. Após o prazo, a vaga retorna ao sistema. Fluxo definido pela Secretaria de Educação de Piraquara.</div>
    </div>
  </div>
</div>

<!-- MODAL -->
<div class="modal-overlay" id="modal-overlay">
  <div class="modal">
    <h3 id="modal-titulo">Confirmar</h3>
    <p id="modal-msg"></p>
    <div class="modal-btns">
      <button class="btn-grande" style="background:#eee;color:#333" onclick="fecharModal()">Cancelar</button>
      <button class="btn-grande btn-verde-g" id="modal-confirmar">Confirmar</button>
    </div>
  </div>
</div>

<div id="rodape">APP-MATRÍCULAS • Piraquara–PR • Dados salvos localmente (offline) • LDBEN | CNE/CEB 5/2009 | Del. CEE/PR 02/2014 | SERE | RCO | TC-PR</div>

<script>
// ============================================================
// CONSTANTES
// ============================================================
const SERIES = [
  { id:'I',   numeral:'I',   nome:'Infantil I',   descricao:'0 a 1 ano e 11 meses' },
  { id:'II',  numeral:'II',  nome:'Infantil II',  descricao:'2 a 2 anos e 11 meses' },
  { id:'III', numeral:'III', nome:'Infantil III', descricao:'3 a 3 anos e 11 meses' },
  { id:'IV',  numeral:'IV',  nome:'Infantil IV',  descricao:'4 anos (obrigatório)' },
  { id:'V',   numeral:'V',   nome:'Infantil V',   descricao:'5 anos (obrigatório)' },
];
const TURMAS = ['A','B','C','D'];
const MAX_PADRAO    = { I:12, II:12, III:15, IV:20, V:20 }; // limite legal DEL CEE/PR 02/2014
const MAX_JUDICIAL  = 30;  // teto absoluto por ordem judicial
const MAX_SOBRESS   = 10;  // sobressalentes normais
const ESPERA_HORAS  = 72;

// ============================================================
// STORAGE
// ============================================================
function getDB()  { try { return JSON.parse(localStorage.getItem('seme_pira') || '{}'); } catch(e) { return {}; } }
function setDB(d) { localStorage.setItem('seme_pira', JSON.stringify(d)); }
function getConfig()  { try { return JSON.parse(localStorage.getItem('seme_cfg') || '{}'); } catch(e) { return {}; } }
function setConfig(c) { localStorage.setItem('seme_cfg', JSON.stringify(c)); }

// ============================================================
// HELPERS DE CONFIGURAÇÃO
// ============================================================

// Limite configurado pelo secretário (ou padrão legal)
function getMaxConfig(sid, t) {
  const cfg = getConfig();
  const key = `${sid}_${t}`;
  if (cfg[key] !== undefined) return parseInt(cfg[key]);
  return MAX_PADRAO[sid] || 12;
}

// Linhas realmente abertas na turma (considera sobressalentes + judiciais)
function getLinhasAbertas(sid, t) {
  const db = getDB();
  if (!db[sid] || !db[sid][t]) return getMaxConfig(sid, t);
  // linhasAbertas só é setado quando > maxConfig; do contrário usa maxConfig
  const stored = db[sid][t].linhasAbertas;
  if (stored !== undefined && stored > getMaxConfig(sid, t)) return stored;
  return getMaxConfig(sid, t);
}

function setLinhasAbertas(sid, t, n) {
  const db = getDB();
  if (!db[sid] || !db[sid][t]) return;
  db[sid][t].linhasAbertas = n;
  while (db[sid][t].alunos.length < n)
    db[sid][t].alunos.push({ cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null, judicial:false });
  setDB(db);
}

// ============================================================
// INIT DB
// ============================================================
function initDB() {
  const db = getDB();
  SERIES.forEach(s => {
    if (!db[s.id]) db[s.id] = {};
    TURMAS.forEach(t => {
      if (!db[s.id][t]) db[s.id][t] = { alunos:[], completa:false, periodo:'' };
      // garante campos periodo
      if (db[s.id][t].periodo === undefined) db[s.id][t].periodo = '';
      const max = getMaxConfig(s.id, t);
      const linhas = getLinhasAbertas(s.id, t);
      const alvo = Math.max(max, linhas);
      while (db[s.id][t].alunos.length < alvo)
        db[s.id][t].alunos.push({ cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null, judicial:false });
    });
  });
  setDB(db);
}

// ============================================================
// NAVEGAÇÃO
// ============================================================
function mostrarTela(id, btn) {
  document.querySelectorAll('.tela').forEach(t => t.classList.remove('ativa'));
  document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('ativo'));
  document.getElementById(id).classList.add('ativa');
  if (btn) btn.classList.add('ativo');
  if (id === 'tela-series')   renderSeries();
  if (id === 'tela-relatorio') renderRelatorio();
  if (id === 'tela-config')   renderConfig();
  if (id === 'tela-consulta') renderResumoConsulta();
}

// ============================================================
// ANO LETIVO DE REFERÊNCIA
// ============================================================
function getAnoLetivo() {
  const cfg = getConfig();
  return cfg._anoLetivo || new Date().getFullYear();
}

function salvarAnoLetivo() {
  const el  = document.getElementById('cfg-ano-letivo');
  const ano = parseInt(el.value);
  if (isNaN(ano) || ano < 2020 || ano > 2099) {
    alert('Informe um ano válido entre 2020 e 2099.'); return;
  }
  const cfg = getConfig();
  cfg._anoLetivo = ano;
  setConfig(cfg);
  atualizarPreviewCorte(ano);
  atualizarBadgeAno();
  alert(`✅ Ano Letivo ${ano} salvo.\nData de corte etário: 31/03/${ano}`);
  if (document.getElementById('input-datanasc').value) consultarVaga();
}

function atualizarPreviewCorte(ano) {
  const el = document.getElementById('cfg-corte-preview');
  if (!el) return;
  el.innerHTML = `
    <strong style="color:var(--verde)">Data de corte ativa: 31/03/${ano}</strong><br>
    <span style="font-size:12px">
    Infantil I &nbsp;&nbsp;→ 01/04/${ano-2} até 31/03/${ano-1} &nbsp;(0–1 ano)<br>
    Infantil II &nbsp;→ 01/04/${ano-3} até 31/03/${ano-2} &nbsp;(2 anos)<br>
    Infantil III → 01/04/${ano-4} até 31/03/${ano-3} &nbsp;(3 anos)<br>
    Infantil IV &nbsp;→ 01/04/${ano-5} até 31/03/${ano-4} &nbsp;(4 anos — obrigatório)<br>
    Infantil V &nbsp;&nbsp;→ 01/04/${ano-6} até 31/03/${ano-5} &nbsp;(5 anos — obrigatório)
    </span>`;
}

function atualizarBadgeAno() {
  const ano   = getAnoLetivo();
  const badge = document.getElementById('badge-ano-letivo-consulta');
  if (!badge) return;
  const aviso = ano !== new Date().getFullYear()
    ? ` &nbsp;<span style="color:var(--espera);font-weight:bold">⚠️ Diferente do ano atual (${new Date().getFullYear()})</span>` : '';
  badge.innerHTML = `<div style="display:inline-flex;align-items:center;gap:8px;padding:6px 14px;background:#e8f0fe;border:1px solid #3f6bc4;border-radius:20px;font-size:12px;color:#1a3a5c;margin-bottom:4px">
    📅 <strong>Ano Letivo: ${ano}</strong> &nbsp;|&nbsp; Corte: 31/03/${ano}${aviso}
    &nbsp;<button onclick="mostrarTela('tela-config',document.querySelectorAll('.nav-btn')[2])" style="background:none;border:none;color:var(--verde);cursor:pointer;font-size:12px;font-weight:bold;text-decoration:underline;padding:0">Alterar</button>
  </div>`;
}

// ============================================================
// TELA CONSULTA
// ============================================================
function calcularIdadeCorte(dn) {
  const ano   = getAnoLetivo();
  const corte = new Date(ano, 2, 31); // 31/03 do ano letivo configurado
  const nasc  = new Date(dn + 'T12:00:00');
  let anos = corte.getFullYear() - nasc.getFullYear();
  const m = corte.getMonth() - nasc.getMonth();
  if (m < 0 || (m === 0 && corte.getDate() < nasc.getDate())) anos--;
  return anos;
}
function idadeParaSerie(idade) {
  if (idade <= 1) return 'I';
  if (idade === 2) return 'II';
  if (idade === 3) return 'III';
  if (idade === 4) return 'IV';
  if (idade === 5) return 'V';
  return null;
}
function expirou(ts) { return !ts || (Date.now() - ts) > ESPERA_HORAS * 3600000; }
function tempoRestante(ts) {
  const r = (ts + ESPERA_HORAS * 3600000) - Date.now();
  if (r <= 0) return 'Expirado';
  return `${Math.floor(r/3600000)}h ${Math.floor((r%3600000)/60000)}min`;
}

function consultarVaga() {
  const dn = document.getElementById('input-datanasc').value;
  const res = document.getElementById('resultado-consulta');
  if (!dn) { res.innerHTML = ''; return; }
  const idade = calcularIdadeCorte(dn);
  const sid   = idadeParaSerie(idade);
  const db    = getDB();
  if (!sid) {
    res.innerHTML = `<div class="resultado-consulta resultado-indisponivel"><strong>⚠️ Fora da faixa etária</strong><br>Idade em 31/03/${getAnoLetivo()}: <strong>${idade} anos</strong>. A Ed. Infantil atende de 0 a 5 anos.</div>`;
    return;
  }
  const serieInfo = SERIES.find(s => s.id === sid);
  let vagas = [];
  TURMAS.forEach(t => {
    if (!db[sid] || !db[sid][t]) return;
    const turma = db[sid][t];
    const linhas = getLinhasAbertas(sid, t);
    const mat = turma.alunos.slice(0, linhas).filter(a => a.status === 'salvo').length;
    const esp = turma.alunos.slice(0, linhas).filter(a => a.status === 'espera' && !expirou(a.timestamp)).length;
    const liv = linhas - mat - esp;
    const periodo = turma.periodo ? ` (${turma.periodo})` : '';
    if (liv > 0 && !turma.completa) vagas.push({ t, liv, mat, esp, periodo });
  });
  if (vagas.length > 0) {
    let html = `<div class="resultado-consulta resultado-disponivel"><strong>✅ Vagas disponíveis — ${serieInfo.nome}</strong><br>Idade em 31/03/${getAnoLetivo()}: <strong>${idade} anos</strong> — ${serieInfo.descricao}<br><br>
    <table style="width:100%;font-size:13px;border-collapse:collapse">
    <tr style="font-weight:bold;border-bottom:1px solid #ccc"><td>Turma</td><td style="text-align:center">Matrículas</td><td style="text-align:center">Espera</td><td style="text-align:center;color:var(--verde)">Vagas Livres</td></tr>`;
    vagas.forEach(v => {
      html += `<tr style="border-bottom:1px solid #eee"><td><strong>Turma ${v.t}${v.periodo}</strong></td><td style="text-align:center">${v.mat}</td><td style="text-align:center">${v.esp}</td><td style="text-align:center;font-weight:bold;color:var(--verde)">${v.liv}</td></tr>`;
    });
    html += `</table><br><em style="font-size:12px">Compareça à secretaria com os documentos.</em></div>`;
    res.innerHTML = html;
  } else {
    res.innerHTML = `<div class="resultado-consulta resultado-espera"><strong>⏳ Sem vagas — ${serieInfo.nome}</strong><br>Idade em 31/03/${getAnoLetivo()}: <strong>${idade} anos</strong>. Solicite inclusão na lista de espera.</div>`;
  }
}

function renderResumoConsulta() {
  initDB();
  const db = getDB();
  let html = '<div class="resumo-grid">';
  let tm = 0, te = 0, tv = 0, tl = 0;
  SERIES.forEach(s => {
    let mat = 0, esp = 0, lin = 0;
    TURMAS.forEach(t => {
      if (!db[s.id] || !db[s.id][t]) return;
      const turma = db[s.id][t];
      const linhas = getLinhasAbertas(s.id, t);
      lin += linhas;
      mat += turma.alunos.slice(0, linhas).filter(a => a.status === 'salvo').length;
      esp += turma.alunos.slice(0, linhas).filter(a => a.status === 'espera' && !expirou(a.timestamp)).length;
    });
    const vaga = lin - mat - esp;
    tm += mat; te += esp; tv += vaga; tl += lin;
    html += `<div class="resumo-card">
      <div class="resumo-numero" style="color:var(--verde)">${s.numeral}</div>
      <div style="font-size:13px;font-weight:bold;margin:4px 0">${s.nome}</div>
      <div style="font-size:11px;color:var(--azul);font-weight:bold;margin-bottom:6px">${lin} vagas abertas</div>
      <div style="font-size:12px">
        <span class="badge badge-verde">✓ ${mat}</span>
        <span class="badge badge-amarelo">⏳ ${esp}</span>
        <span class="badge ${vaga>0?'badge-verde':'badge-cinza'}">🟢 ${vaga} livres</span>
      </div></div>`;
  });
  html += `<div class="resumo-card" style="border:2px solid var(--verde)">
    <div class="resumo-numero" style="color:var(--azul)">∑</div>
    <div style="font-size:13px;font-weight:bold;margin:4px 0">Total Geral</div>
    <div style="font-size:11px;color:var(--azul);font-weight:bold;margin-bottom:6px">${tl} vagas abertas</div>
    <div style="font-size:12px">
      <span class="badge badge-verde">✓ ${tm}</span>
      <span class="badge badge-amarelo">⏳ ${te}</span>
      <span class="badge ${tv>0?'badge-verde':'badge-cinza'}">🟢 ${tv}</span>
    </div></div>`;
  html += '</div>';
  document.getElementById('painel-resumo-geral').innerHTML = html;
}

// ============================================================
// TELA SÉRIES
// ============================================================
let serieAtiva = null, turmaAtiva = null;

function renderSeries() {
  initDB();
  const db = getDB();
  let html = '<div class="series-grid">';
  SERIES.forEach(s => {
    let mat = 0, esp = 0, vag = 0, lin = 0, comp = 0;
    TURMAS.forEach(t => {
      if (!db[s.id] || !db[s.id][t]) return;
      const turma = db[s.id][t];
      const linhas = getLinhasAbertas(s.id, t);
      lin += linhas;
      const m = turma.alunos.slice(0, linhas).filter(a => a.status === 'salvo').length;
      const e = turma.alunos.slice(0, linhas).filter(a => a.status === 'espera' && !expirou(a.timestamp)).length;
      mat += m; esp += e; vag += (linhas - m - e);
      if (turma.completa) comp++;
    });
    html += `<div class="serie-card ${serieAtiva===s.id?'ativa':''}" onclick="selecionarSerie('${s.id}')">
      <div class="serie-numeral">${s.numeral}</div>
      <div class="serie-nome">${s.nome}</div>
      <div style="font-size:11px;color:var(--texto-muted);margin:3px 0">${s.descricao}</div>
      <div style="font-size:11px;color:var(--azul);font-weight:bold;margin:4px 0">${lin} vagas abertas</div>
      <div style="font-size:12px">
        <span class="badge badge-verde">✓ ${mat}</span>
        <span class="badge badge-amarelo">⏳ ${esp}</span>
        <span class="badge ${vag>0?'badge-verde':'badge-cinza'}">⬜ ${vag} livres</span>
        ${comp>0?`<span class="badge badge-completa">🔒 ${comp}</span>`:''}
      </div></div>`;
  });
  html += '</div>';
  document.getElementById('painel-series').innerHTML = html;
  if (serieAtiva) renderTurmas(serieAtiva);
}

function selecionarSerie(sid) {
  serieAtiva = sid;
  turmaAtiva = turmaAtiva || 'A';
  document.getElementById('painel-turmas').style.display = 'block';
  renderSeries();
}

function renderTurmas(sid) {
  const db = getDB();
  const serie = SERIES.find(s => s.id === sid);
  document.getElementById('titulo-turma').textContent = `📚 ${serie.nome} — Turmas`;
  let tabs = '';
  TURMAS.forEach(t => {
    const turma = db[sid] && db[sid][t];
    const comp = turma && turma.completa;
    const per  = turma && turma.periodo ? ` ${turma.periodo === 'Manhã' ? '🌅' : turma.periodo === 'Tarde' ? '🌇' : '🔆'}` : '';
    tabs += `<button class="turma-tab ${turmaAtiva===t?'ativa':''} ${comp?'completa':''}" onclick="selecionarTurma('${sid}','${t}')">
      Turma ${t}${per}${comp?' 🔒':''}
    </button>`;
  });
  document.getElementById('tabs-turmas').innerHTML = tabs;
  renderListaAlunos(sid, turmaAtiva || 'A');
}

function selecionarTurma(sid, t) {
  turmaAtiva = t;
  renderTurmas(sid);
}

// ============================================================
// LISTA DE ALUNOS
// ============================================================
function renderListaAlunos(sid, t) {
  const db = getDB();
  if (!db[sid] || !db[sid][t]) { initDB(); return renderListaAlunos(sid, t); }
  const turma    = db[sid][t];
  const maxCfg   = getMaxConfig(sid, t);           // configurado pelo secretário
  const linhas   = getLinhasAbertas(sid, t);        // abertas atualmente
  const sobr     = Math.max(0, linhas - maxCfg);    // sobressalentes usados (normais)
  const judiciais = turma.alunos.filter(a => a.judicial).length;
  const alunos   = turma.alunos;
  const periodo  = turma.periodo || '';

  // Limpa expirados
  let alt = false;
  alunos.forEach(a => {
    if (a.status === 'espera' && expirou(a.timestamp)) {
      Object.assign(a, { cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null });
      alt = true;
    }
  });
  if (alt) setDB(db);

  const salvos  = alunos.slice(0, linhas).filter(a => a.status === 'salvo').length;
  const espera  = alunos.slice(0, linhas).filter(a => a.status === 'espera').length;
  const vazios  = alunos.slice(0, linhas).filter(a => a.status === 'vazio').length;

  // Botão sobressalente
  const sobrRestantes = MAX_SOBRESS - sobr;
  const podeSobr = !turma.completa && sobrRestantes > 0 && linhas < MAX_JUDICIAL;
  const btnSobr = podeSobr
    ? `<button class="btn-grande" style="background:var(--amarelo);color:white;font-size:12px;padding:7px 14px" onclick="addSobressalente('${sid}','${t}')">➕ Sobressalente (${sobr}/${MAX_SOBRESS})</button>`
    : (sobrRestantes<=0 ? `<span style="font-size:12px;color:var(--perigo)">⚠️ Máx sobressalentes atingido</span>` : '');

  // Botão período
  const perBtns = ['Manhã','Tarde','Integral'].map(p =>
    `<button class="btn-periodo ${periodo===p?'ativo-'+p.toLowerCase():''}" onclick="setPeriodo('${sid}','${t}','${p}')">${p==='Manhã'?'🌅':''}${p==='Tarde'?'🌇':''}${p==='Integral'?'🔆':''} ${p}</button>`
  ).join('');

  let html = `
  <div style="display:flex;flex-wrap:wrap;gap:10px;align-items:center;justify-content:space-between;margin-bottom:10px">
    <div>
      <div style="font-size:12px;font-weight:bold;color:var(--texto-muted);margin-bottom:4px">PERÍODO DA TURMA</div>
      <div class="periodo-grupo">${perBtns}</div>
    </div>
    <div>
      <span class="badge badge-verde">✓ ${salvos} mat.</span>
      <span class="badge badge-amarelo">⏳ ${espera} espera</span>
      <span class="badge badge-cinza">⬜ ${vazios} livres</span>
      <span class="badge badge-cinza">📋 ${linhas} linhas (cfg: ${maxCfg})</span>
      ${judiciais>0?`<span class="badge badge-roxo">⚖️ ${judiciais} judiciais</span>`:''}
    </div>
  </div>
  <div class="legenda">
    <span class="legenda-item"><span class="status-dot dot-vazio"></span> Vazio</span>
    <span class="legenda-item"><span class="status-dot dot-espera"></span> Espera 72h</span>
    <span class="legenda-item"><span class="status-dot dot-salvo"></span> Confirmado</span>
    <span class="legenda-item"><span class="status-dot dot-judicial"></span> Judicial</span>
  </div>
  <div style="display:flex;gap:8px;flex-wrap:wrap;align-items:center;margin-bottom:10px">
    <button class="btn-completa ${turma.completa?'marcada':''}" onclick="toggleCompleta('${sid}','${t}')">
      ${turma.completa?'🔒 COMPLETA — Desmarcar':'📌 Marcar como COMPLETA'}
    </button>
    ${btnSobr}
  </div>
  ${turma.completa?`<div style="margin-bottom:10px;padding:10px;background:#e8f0fe;border-radius:6px;font-size:13px">🔒 Turma fechada. Número definitivo: <strong>${salvos} alunos</strong> matriculados.</div>`:''}
  ${sobr>0?`<div style="margin-bottom:8px;padding:7px 12px;background:#fff8e1;border-left:4px solid var(--amarelo);border-radius:6px;font-size:12px">⚠️ <strong>${sobr} vaga(s) sobressalente(s)</strong> além do limite configurado (${maxCfg}).</div>`:''}

  <div class="tabela-wrapper">
  <table class="alunos">
    <thead><tr>
      <th style="width:30px">#</th><th style="width:12px"></th>
      <th style="width:95px">CGM</th><th>Nome do Aluno</th>
      <th style="width:125px">Nascimento</th><th style="width:105px">Situação</th>
      <th style="width:155px">Ações</th>
    </tr></thead>
    <tbody>`;

  for (let i = 0; i < linhas; i++) {
    const a = alunos[i] || { cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null, judicial:false };
    const isSalvo  = a.status === 'salvo';
    const isEspera = a.status === 'espera' && !expirou(a.timestamp);
    const isVazio  = a.status === 'vazio';
    const isJudicial = !!a.judicial;

    const rowClass = isSalvo ? (isJudicial?'linha-judicial':'linha-salva') : (isEspera?'linha-espera':'');
    const disabled = isSalvo ? 'disabled' : '';
    const dot = isVazio ? 'dot-vazio' : (isEspera ? 'dot-espera' : (isJudicial ? 'dot-judicial' : 'dot-salvo'));

    const situacao = isEspera
      ? `<span class="timer-espera">⏳ ${tempoRestante(a.timestamp)}</span>`
      : isSalvo
        ? `<span class="badge ${isJudicial?'badge-roxo':'badge-verde'}">${isJudicial?'⚖️ Judicial':'✓ Conf.'}</span>`
        : `<span style="font-size:11px;color:#bbb">—</span>`;

    let botoes = '';
    if (turma.completa && isVazio) {
      botoes = `<span style="font-size:11px;color:#aaa">Completa</span>`;
    } else if (isSalvo) {
      botoes = `<div class="btn-acoes">
        <button class="btn btn-corrigir" onclick="corrigirAluno('${sid}','${t}',${i})">✏️</button>
        <button class="btn btn-deletar" onclick="confirmarDeletar('${sid}','${t}',${i})">🗑</button>
      </div>`;
    } else if (isEspera) {
      botoes = `<div class="btn-acoes">
        <button class="btn btn-salvar" onclick="salvarAluno('${sid}','${t}',${i})">💾 Confirmar</button>
        <button class="btn btn-deletar" onclick="limparAluno('${sid}','${t}',${i})">✕</button>
      </div>`;
    } else {
      botoes = `<div class="btn-acoes">
        <button class="btn btn-salvar" onclick="salvarAluno('${sid}','${t}',${i})">💾 Salvar</button>
        <button class="btn btn-deletar" style="background:#aaa" onclick="limparAluno('${sid}','${t}',${i})">✕</button>
      </div>`;
    }

    html += `<tr class="${rowClass}" id="linha-${sid}-${t}-${i}">
      <td class="num-linha">${i+1}${isJudicial?'<span title="Judicial" style="color:var(--roxo);font-size:9px">⚖</span>':''}</td>
      <td><span class="status-dot ${dot}"></span></td>
      <td><input class="campo-aluno" id="cgm-${sid}-${t}-${i}" value="${escHtml(a.cgm)}" placeholder="CGM" ${disabled}></td>
      <td><input class="campo-aluno" id="nome-${sid}-${t}-${i}" value="${escHtml(a.nome)}" placeholder="Nome completo" ${disabled}></td>
      <td><input class="campo-aluno" type="date" id="dn-${sid}-${t}-${i}" value="${a.dataNasc||''}" ${disabled}></td>
      <td>${situacao}</td>
      <td>${botoes}</td>
    </tr>`;
  }

  // Botão adicionar vaga judicial — aparece após a última linha
  const podeJudicial = !turma.completa && linhas < MAX_JUDICIAL;
  html += `</tbody></table></div>
  <button class="btn-add-judicial" ${podeJudicial?'':`disabled title="Limite de ${MAX_JUDICIAL} atingido"`} onclick="addJudicial('${sid}','${t}')">
    ⚖️ Adicionar Vaga por Determinação Judicial / MP / Conselho Tutelar ${podeJudicial?`(${MAX_JUDICIAL-linhas} disponíveis)`:`— Limite de ${MAX_JUDICIAL} atingido`}
  </button>`;

  document.getElementById('conteudo-turma').innerHTML = html;
}

function escHtml(s) { return (s||'').replace(/&/g,'&amp;').replace(/"/g,'&quot;').replace(/</g,'&lt;'); }

// ============================================================
// AÇÕES NAS TURMAS
// ============================================================
function setPeriodo(sid, t, p) {
  const db = getDB();
  db[sid][t].periodo = (db[sid][t].periodo === p) ? '' : p; // toggle
  setDB(db);
  renderListaAlunos(sid, t);
  renderTurmas(sid);
}

function salvarAluno(sid, t, i) {
  const db   = getDB();
  const nome = document.getElementById(`nome-${sid}-${t}-${i}`).value.trim();
  if (!nome) { alert('Preencha o nome antes de salvar.'); return; }
  const a = db[sid][t].alunos[i];
  a.cgm      = document.getElementById(`cgm-${sid}-${t}-${i}`).value.trim();
  a.nome     = nome;
  a.dataNasc = document.getElementById(`dn-${sid}-${t}-${i}`).value;
  a.status   = 'salvo';
  a.timestamp= Date.now();
  setDB(db);
  renderListaAlunos(sid, t);
  renderSeries();
  renderResumoConsulta();
}

function corrigirAluno(sid, t, i) {
  // Desbloqueia campos diretamente no DOM sem re-render
  ['cgm','nome','dn'].forEach(p => {
    const el = document.getElementById(`${p}-${sid}-${t}-${i}`);
    if (el) el.disabled = false;
  });
  const linha = document.getElementById(`linha-${sid}-${t}-${i}`);
  if (linha) {
    linha.querySelector('td:last-child').innerHTML = `<div class="btn-acoes">
      <button class="btn btn-salvar" onclick="salvarCorrecao('${sid}','${t}',${i})">💾 Salvar</button>
      <button class="btn" style="background:#999;color:white" onclick="renderListaAlunos('${sid}','${t}')">✕</button>
    </div>`;
  }
}

function salvarCorrecao(sid, t, i) {
  const db = getDB();
  const a  = db[sid][t].alunos[i];
  a.cgm      = document.getElementById(`cgm-${sid}-${t}-${i}`).value.trim();
  a.nome     = document.getElementById(`nome-${sid}-${t}-${i}`).value.trim();
  a.dataNasc = document.getElementById(`dn-${sid}-${t}-${i}`).value;
  a.status   = 'salvo';
  setDB(db);
  renderListaAlunos(sid, t);
}

function limparAluno(sid, t, i) {
  const db = getDB();
  Object.assign(db[sid][t].alunos[i], { cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null, judicial:false });
  setDB(db);
  renderListaAlunos(sid, t);
  renderResumoConsulta();
}

let modalCb = null;
function confirmarDeletar(sid, t, i) {
  const nome = getDB()[sid][t].alunos[i].nome || `Linha ${i+1}`;
  document.getElementById('modal-titulo').textContent = 'Confirmar Exclusão';
  document.getElementById('modal-msg').textContent = `Excluir matrícula de "${nome}"? Esta ação não pode ser desfeita.`;
  document.getElementById('modal-confirmar').style.background = 'var(--perigo)';
  document.getElementById('modal-confirmar').textContent = 'Excluir';
  document.getElementById('modal-confirmar').onclick = () => { limparAluno(sid, t, i); fecharModal(); };
  document.getElementById('modal-overlay').classList.add('aberto');
}
function fecharModal() { document.getElementById('modal-overlay').classList.remove('aberto'); }

function toggleCompleta(sid, t) {
  const db = getDB();
  db[sid][t].completa = !db[sid][t].completa;
  setDB(db);
  renderTurmas(sid);
  renderSeries();
  renderResumoConsulta();
}

function addSobressalente(sid, t) {
  const maxCfg = getMaxConfig(sid, t);
  const linhas = getLinhasAbertas(sid, t);
  const sobr   = Math.max(0, linhas - maxCfg);
  if (sobr >= MAX_SOBRESS) { alert('Limite de sobressalentes atingido.'); return; }
  if (linhas >= MAX_JUDICIAL) { alert(`Limite absoluto de ${MAX_JUDICIAL} alunos atingido.`); return; }
  if (!confirm(`Abrir +1 vaga sobressalente?\n\nConfigurdo: ${maxCfg} | Sobressalentes: ${sobr}/${MAX_SOBRESS}`)) return;
  setLinhasAbertas(sid, t, linhas + 1);
  renderListaAlunos(sid, t);
  renderSeries();
  renderResumoConsulta();
}

function addJudicial(sid, t) {
  const linhas = getLinhasAbertas(sid, t);
  if (linhas >= MAX_JUDICIAL) { alert(`Limite absoluto de ${MAX_JUDICIAL} atingido.`); return; }
  const db = getDB();
  const novaLinhas = linhas + 1;
  db[sid][t].linhasAbertas = novaLinhas;
  // Empurra nova vaga marcada como judicial
  if (db[sid][t].alunos.length < novaLinhas)
    db[sid][t].alunos.push({ cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null, judicial:true });
  else
    db[sid][t].alunos[novaLinhas-1].judicial = true;
  setDB(db);
  renderListaAlunos(sid, t);
  renderSeries();
  renderResumoConsulta();
}

// ============================================================
// CONFIGURAÇÕES — INTERAÇÃO COM TURMAS
// ============================================================
function renderConfig() {
  // Carrega ano letivo
  const anoAtual = getAnoLetivo();
  const elAno = document.getElementById('cfg-ano-letivo');
  if (elAno) elAno.value = anoAtual;
  atualizarPreviewCorte(anoAtual);
  // Atualiza preview em tempo real ao digitar
  if (elAno) elAno.oninput = () => {
    const v = parseInt(elAno.value);
    if (v >= 2020 && v <= 2099) atualizarPreviewCorte(v);
  };

  const cfg = getConfig();
  let html = '';
  SERIES.forEach(s => {
    TURMAS.forEach(t => {
      const key = `${s.id}_${t}`;
      const val = cfg[key] !== undefined ? cfg[key] : MAX_PADRAO[s.id];
      html += `<div class="config-item">
        <label>${s.nome} — Turma ${t}</label>
        <input type="number" id="cfg-${key}" value="${val}" min="1" max="${MAX_JUDICIAL}" placeholder="Nº de alunos">
      </div>`;
    });
  });
  document.getElementById('config-grid').innerHTML = html;
}

function salvarConfig() {
  const cfg = {};
  SERIES.forEach(s => {
    TURMAS.forEach(t => {
      const key = `${s.id}_${t}`;
      const el  = document.getElementById(`cfg-${key}`);
      if (el) {
        let v = parseInt(el.value);
        if (isNaN(v) || v < 1) v = MAX_PADRAO[s.id];
        if (v > MAX_JUDICIAL) v = MAX_JUDICIAL;
        cfg[key] = v;
      }
    });
  });
  setConfig(cfg);

  // Sincroniza o DB: garante que cada turma tem células suficientes para o novo valor
  const db = getDB();
  SERIES.forEach(s => {
    TURMAS.forEach(t => {
      if (!db[s.id] || !db[s.id][t]) return;
      const novoMax = cfg[`${s.id}_${t}`] || MAX_PADRAO[s.id];
      // Reseta linhasAbertas se a nova config for maior que o valor guardado
      if (!db[s.id][t].linhasAbertas || db[s.id][t].linhasAbertas < novoMax)
        db[s.id][t].linhasAbertas = novoMax;
      while (db[s.id][t].alunos.length < db[s.id][t].linhasAbertas)
        db[s.id][t].alunos.push({ cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null, judicial:false });
    });
  });
  setDB(db);

  alert('✅ Configurações salvas! As turmas foram atualizadas.');
  // Atualiza telas se abertas
  if (serieAtiva) { renderSeries(); }
  renderResumoConsulta();
}

function restaurarPadroes() {
  if (!confirm('Restaurar limites padrão (Del. CEE/PR 02/2014)? As células nas turmas serão ajustadas.')) return;
  setConfig({});
  const db = getDB();
  SERIES.forEach(s => {
    TURMAS.forEach(t => {
      if (!db[s.id] || !db[s.id][t]) return;
      delete db[s.id][t].linhasAbertas;
      // Garante array mínimo
      const pad = MAX_PADRAO[s.id];
      while (db[s.id][t].alunos.length < pad)
        db[s.id][t].alunos.push({ cgm:'', nome:'', dataNasc:'', status:'vazio', timestamp:null, judicial:false });
    });
  });
  setDB(db);
  renderConfig();
  if (serieAtiva) renderSeries();
  renderResumoConsulta();
}

// ============================================================
// RELATÓRIO
// ============================================================
function renderRelatorio() {
  initDB();
  const db = getDB();
  const hoje = new Date().toLocaleDateString('pt-BR');
  let html = `<p style="font-size:12px;color:var(--texto-muted);margin-bottom:16px">Gerado em: ${hoje} | Piraquara–PR</p>`;
  SERIES.forEach(s => {
    html += `<h3 style="color:var(--verde);margin:16px 0 8px;font-family:var(--fonte-titulo)">${s.numeral} — ${s.nome} <small style="font-size:12px;font-weight:normal;color:var(--texto-muted)">(${s.descricao})</small></h3>`;
    html += `<table style="width:100%;border-collapse:collapse;font-size:13px;margin-bottom:12px">
      <thead><tr style="background:var(--verde);color:white">
        <th style="padding:8px;text-align:left">Turma</th>
        <th style="padding:8px;text-align:left">Período</th>
        <th style="padding:8px;text-align:center">Vagas Abertas</th>
        <th style="padding:8px;text-align:center">Matrículas</th>
        <th style="padding:8px;text-align:center">Espera</th>
        <th style="padding:8px;text-align:center">Livres</th>
        <th style="padding:8px;text-align:center">Judiciais</th>
        <th style="padding:8px;text-align:center">Situação</th>
      </tr></thead><tbody>`;
    TURMAS.forEach(t => {
      if (!db[s.id] || !db[s.id][t]) return;
      const turma  = db[s.id][t];
      const linhas = getLinhasAbertas(s.id, t);
      const mat    = turma.alunos.slice(0,linhas).filter(a => a.status==='salvo').length;
      const esp    = turma.alunos.slice(0,linhas).filter(a => a.status==='espera' && !expirou(a.timestamp)).length;
      const jud    = turma.alunos.filter(a => a.judicial).length;
      const liv    = linhas - mat - esp;
      html += `<tr style="border-bottom:1px solid #eee">
        <td style="padding:6px 8px">Turma ${t}</td>
        <td style="padding:6px 8px">${turma.periodo||'—'}</td>
        <td style="text-align:center;padding:6px">${linhas}</td>
        <td style="text-align:center;padding:6px;font-weight:bold;color:var(--verde)">${mat}</td>
        <td style="text-align:center;padding:6px;color:var(--espera)">${esp}</td>
        <td style="text-align:center;padding:6px;color:${liv>0?'var(--verde)':'var(--perigo)'}">${liv}</td>
        <td style="text-align:center;padding:6px;color:var(--roxo)">${jud||'—'}</td>
        <td style="text-align:center;padding:6px">${turma.completa?'<span class="badge badge-completa">🔒 Completa</span>':'<span class="badge badge-cinza">Aberta</span>'}</td>
      </tr>`;
    });
    html += '</tbody></table>';
  });
  document.getElementById('corpo-relatorio').innerHTML = html;
}

// ============================================================
// INIT
// ============================================================
document.addEventListener('DOMContentLoaded', () => {
  document.getElementById('input-datanasc').max = new Date().toISOString().split('T')[0];
  initDB();
  atualizarBadgeAno();
  renderResumoConsulta();
  renderSeries();
  renderConfig();
});

setInterval(() => {
  if (serieAtiva && turmaAtiva) renderListaAlunos(serieAtiva, turmaAtiva);
  renderResumoConsulta();
}, 60000);
</script>
</body>
</html>


***


APP SISTEMA DE GESTÃO NUTRICIONAL
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MAPA DE CMEI — Gestão Nutricional · Piraquara</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;600;700;800&family=Barlow:wght@400;500;600&display=swap');
:root{
  --g1:#1b5e3b;--g2:#0d3b26;--g3:#2e7d52;--g4:#e8f5ee;
  --b1:#1a3a5c;--b2:#0f2540;--b3:#2a5a8c;
  --am:#f5a623;--am2:#e6951a;
  --verm:#c0392b;--verm2:#e74c3c;
  --cinza:#f0f2f0;--borda:#d0d6d0;
  --txt:#1a1a18;--txt2:#4a5048;--txt3:#7a8078;
  --branco:#ffffff;
  --fnt-h:'Barlow Condensed',sans-serif;
  --fnt-b:'Barlow',sans-serif;
  --sh:0 2px 12px rgba(0,0,0,.12);
  --r:8px;
}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:var(--fnt-b);background:#e8ece8;color:var(--txt);min-height:100vh;font-size:13px}

/* ── HEADER ── */
#hdr{background:linear-gradient(135deg,var(--g2) 0%,var(--b2) 55%,var(--g2) 100%);
  color:#fff;position:sticky;top:0;z-index:200;box-shadow:0 3px 16px rgba(0,0,0,.35)}
#hdr-top{display:flex;align-items:center;gap:14px;padding:10px 20px}
#hdr-logo{width:44px;height:44px;background:linear-gradient(135deg,var(--am),var(--am2));
  border-radius:10px;display:flex;align-items:center;justify-content:center;flex-shrink:0;
  box-shadow:0 2px 8px rgba(245,166,35,.4)}
#hdr-logo svg{width:26px;height:26px}
#hdr-titulo h1{font-family:var(--fnt-h);font-size:18px;font-weight:800;letter-spacing:.5px;
  text-transform:uppercase}
#hdr-titulo p{font-size:11px;opacity:.75;margin-top:1px}
#hdr-badge{margin-left:auto;display:flex;gap:10px;align-items:center}
.hdr-chip{background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.2);
  border-radius:20px;padding:4px 12px;font-size:11px;font-weight:600;white-space:nowrap}
.hdr-chip.ok{background:rgba(46,125,82,.5);border-color:rgba(46,125,82,.8)}
.hdr-chip.warn{background:rgba(245,166,35,.35);border-color:rgba(245,166,35,.7);color:#ffd88a}

/* ── TABS ── */
#tabs{background:rgba(0,0,0,.22);display:flex;overflow-x:auto;border-top:1px solid rgba(255,255,255,.08)}
.tb{background:none;border:none;color:rgba(255,255,255,.72);padding:9px 18px;cursor:pointer;
  font-family:var(--fnt-h);font-size:13px;font-weight:700;letter-spacing:.3px;
  white-space:nowrap;border-bottom:3px solid transparent;transition:all .2s;text-transform:uppercase}
.tb:hover,.tb.at{color:#fff;border-bottom-color:var(--am);background:rgba(255,255,255,.07)}
.tb .dot{width:7px;height:7px;border-radius:50%;background:var(--am);display:inline-block;
  margin-left:5px;vertical-align:middle;opacity:0}
.tb .dot.on{opacity:1}

/* ── MAIN ── */
#main{padding:16px 20px;max-width:1600px;margin:0 auto}
.tela{display:none}.tela.at{display:block}

/* ── CARDS ── */
.card{background:var(--branco);border-radius:var(--r);box-shadow:var(--sh);
  margin-bottom:14px;border:1px solid var(--borda)}
.ch{padding:10px 16px;border-radius:var(--r) var(--r) 0 0;font-family:var(--fnt-h);
  font-size:15px;font-weight:700;letter-spacing:.3px;display:flex;
  align-items:center;justify-content:space-between;gap:8px}
.ch-g{background:linear-gradient(90deg,var(--g1),var(--g2));color:#fff}
.ch-b{background:linear-gradient(90deg,var(--b1),var(--b2));color:#fff}
.ch-am{background:linear-gradient(90deg,#7a5000,#a06800);color:#fff}
.ch-r{background:linear-gradient(90deg,var(--verm),#922b21);color:#fff}
.cb{padding:12px 16px}

/* ── SEC TITULO ── */
.stit{font-family:var(--fnt-h);font-size:20px;font-weight:800;letter-spacing:.5px;
  text-transform:uppercase;color:var(--g1);margin-bottom:12px;
  display:flex;align-items:center;gap:10px;border-left:4px solid var(--am);padding-left:10px}
.stit .tag{background:var(--am);color:#1a0a00;padding:2px 10px;border-radius:12px;
  font-size:11px;font-weight:800}

/* ── FORM ── */
.fg-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:12px;margin-bottom:14px}
.fg label{display:block;font-size:10px;font-weight:700;text-transform:uppercase;
  letter-spacing:.5px;color:var(--txt2);margin-bottom:4px}
.fg input,.fg select{width:100%;padding:8px 10px;border:1.5px solid var(--borda);
  border-radius:6px;font-size:13px;font-family:var(--fnt-b);transition:border-color .2s;background:#fff}
.fg input:focus,.fg select:focus{outline:none;border-color:var(--g1);box-shadow:0 0 0 3px rgba(27,94,59,.1)}

/* ── BOTÕES ── */
.btn{border:none;border-radius:6px;padding:8px 16px;cursor:pointer;font-family:var(--fnt-h);
  font-size:13px;font-weight:700;letter-spacing:.3px;transition:all .15s;
  display:inline-flex;align-items:center;gap:6px;text-transform:uppercase}
.btn:active{transform:scale(.97)}
.btn-g{background:linear-gradient(135deg,var(--g3),var(--g1));color:#fff;box-shadow:0 2px 8px rgba(27,94,59,.3)}
.btn-g:hover{background:linear-gradient(135deg,var(--g3),var(--g3))}
.btn-b{background:linear-gradient(135deg,var(--b3),var(--b1));color:#fff;box-shadow:0 2px 8px rgba(26,58,92,.3)}
.btn-am{background:linear-gradient(135deg,var(--am),var(--am2));color:#1a0a00;font-weight:800}
.btn-r{background:linear-gradient(135deg,var(--verm2),var(--verm));color:#fff}
.btn-c{background:#888;color:#fff}
.btn-sm{padding:4px 10px;font-size:11px}
.brow{display:flex;gap:8px;flex-wrap:wrap;margin:10px 0}

/* ── TABELAS ── */
.tw{overflow-x:auto;max-height:62vh;overflow-y:auto;border-radius:0 0 var(--r) var(--r)}
table{border-collapse:collapse;font-size:12px;width:100%}
thead th{background:var(--g1);color:#fff;padding:7px 8px;text-align:center;
  white-space:nowrap;position:sticky;top:0;z-index:10}
thead th.sk{position:sticky;left:0;z-index:20;background:var(--b1)}
thead th.sk2{position:sticky;left:0;z-index:20;background:var(--g2);text-align:left;padding-left:10px}
tbody td{padding:4px 6px;border-bottom:1px solid #ebebeb;border-right:1px solid #ebebeb;
  text-align:center;vertical-align:middle}
tbody td.nc{text-align:left;white-space:nowrap;position:sticky;left:0;background:#f7faf7;
  font-size:11px;z-index:5;border-right:2px solid var(--g3);padding:4px 8px;min-width:160px}
tbody tr:hover td{background:#f0faf3}
tbody tr:hover td.nc{background:#dff2e5}
.tr-tot td{background:#e3f5ec!important;font-weight:700;color:var(--g1)}
.tr-tot td.nc{background:#c8ecd5!important}
.tr-sep td{background:#f0f4ff!important;font-weight:700;color:var(--b1);font-family:var(--fnt-h);font-size:12px;text-align:left;padding:5px 10px}
.neg{background:#fdecea!important;color:var(--verm)!important;font-weight:700}
.entr{background:#e8f5ee!important;color:var(--g1)!important;font-weight:700}
.said{background:#fef9ec!important;color:#7a5000!important;font-weight:700}

input.inp{width:68px;border:1px solid #ccc;border-radius:4px;padding:3px 5px;
  font-size:11px;text-align:center;font-family:var(--fnt-b)}
input.inp:focus{outline:2px solid var(--g1);border-color:var(--g1)}
input.inp-lg{width:85px}
input.inp-w{width:100%}
textarea.inp-ta{width:100%;border:1px solid #ccc;border-radius:4px;padding:3px 6px;
  font-size:11px;resize:vertical;min-height:34px;font-family:var(--fnt-b)}
textarea.inp-ta:focus{outline:2px solid var(--g1)}

/* ── F1 HEADER VERTICAL ── */
th.vert{writing-mode:vertical-rl;transform:rotate(180deg);max-height:90px;
  height:90px;font-size:10px;padding:4px 5px;line-height:1.2}

/* ── NF SELECTOR ── */
.nf-sel{display:flex;gap:5px;flex-wrap:wrap;align-items:center;margin-bottom:10px;
  background:#f7f9f7;border-radius:6px;padding:10px;border:1px solid var(--borda)}
.nf-btn{padding:4px 9px;border:2px solid var(--borda);border-radius:14px;cursor:pointer;
  font-size:11px;font-weight:700;background:#fff;transition:all .15s;font-family:var(--fnt-h)}
.nf-btn.has{border-color:var(--g1);color:var(--g1);background:var(--g4)}
.nf-btn.ativo{background:var(--b1);color:#fff;border-color:var(--b1)}
.nf-btn.has.ativo{background:var(--g1);color:#fff;border-color:var(--g1)}

/* ── BADGES ── */
.badge{display:inline-block;padding:2px 8px;border-radius:10px;font-size:10px;
  font-weight:700;letter-spacing:.3px}
.b-ok{background:#d4edda;color:#155724}
.b-av{background:#fff3cd;color:#856404}
.b-er{background:#f8d7da;color:#721c24}
.b-in{background:#cce5ff;color:#004085}

/* ── RELATÓRIO ── */
.rel-g{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:10px;margin-bottom:14px}
.rel-item{background:#f7faf7;border:1px solid var(--borda);border-radius:6px;padding:10px 14px}
.rel-item h4{font-size:10px;text-transform:uppercase;letter-spacing:.5px;color:var(--txt3);margin-bottom:3px}
.rel-item p{font-family:var(--fnt-h);font-size:20px;font-weight:800;color:var(--g1)}
.rel-item.alert{background:#fff5f5;border-color:var(--verm)}
.rel-item.alert p{color:var(--verm)}

/* ── DIVERGÊNCIAS ── */
.div-lista{list-style:none}
.div-lista li{display:flex;justify-content:space-between;align-items:center;
  padding:7px 10px;border-bottom:1px solid #f0e8e8;font-size:12px;gap:8px}
.div-lista li:last-child{border-bottom:none}
.div-lista li .esq{display:flex;flex-direction:column;gap:2px}
.div-lista li .dir{display:flex;gap:4px;flex-shrink:0}

/* ── CORREÇÃO ── */
.corr-box{background:linear-gradient(135deg,#fffbf0,#fff9e6);border:2px solid var(--am);
  border-radius:8px;padding:14px;margin:12px 0}
.corr-box h4{color:#7a5000;font-family:var(--fnt-h);font-size:14px;font-weight:800;margin-bottom:10px}
.corr-row{display:flex;gap:8px;align-items:center;flex-wrap:wrap}
.corr-row select,.corr-row input{padding:7px 10px;border:1.5px solid #d4b860;border-radius:6px;
  font-size:12px;font-family:var(--fnt-b);background:#fff}
.corr-row select{flex:3;min-width:200px}
.corr-row input{flex:1;min-width:90px}

/* ── RESP ── */
.resp-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:10px}

/* ── PRINT ── */
@media print{
  #hdr,#tabs,.brow,.btn,.corr-box,#hdr-badge{display:none!important}
  .tela{display:block!important}
  .card{break-inside:avoid;box-shadow:none;border:1px solid #999}
  body{background:#fff}
  .stit{color:#000;border-left:3px solid #000}
}

/* ── INFO PANEL ── */
.info-box{background:linear-gradient(135deg,var(--g4),#fff);border:1px solid #b8dfc8;
  border-radius:8px;padding:12px 14px;margin-bottom:12px;font-size:12px;color:var(--txt2)}
.info-box strong{color:var(--g1)}

/* ── PROGRESS INDICATOR ── */
.prog-bar{height:4px;background:#e0e8e0;border-radius:2px;margin-top:6px;overflow:hidden}
.prog-fill{height:100%;background:linear-gradient(90deg,var(--g3),var(--am));border-radius:2px;transition:width .3s}

/* ── TOOLTIP ── */
.tip{font-size:10px;color:var(--txt3);font-style:italic;margin-top:2px}

/* ── SCROLLBAR ── */
.tw::-webkit-scrollbar{width:6px;height:6px}
.tw::-webkit-scrollbar-track{background:#f0f0f0}
.tw::-webkit-scrollbar-thumb{background:#b0b8b0;border-radius:3px}
</style>
</head>
<body>

<!-- HEADER -->
<div id="hdr">
  <div id="hdr-top">
    <div id="hdr-logo">
      <svg viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg">
        <rect x="2" y="13" width="22" height="11" rx="2" fill="#1a0800"/>
        <polygon points="13,2 24,13 2,13" fill="#1a0800" opacity=".8"/>
        <rect x="9" y="17" width="8" height="7" fill="#fff" opacity=".7"/>
      </svg>
    </div>
    <div id="hdr-titulo">
      <h1>MAPA DE CMEI · Sistema de Gestão Nutricional</h1>
      <p>Prefeitura de Piraquara — Controle de Estoque, Cardápio e Notas Fiscais</p>
    </div>
    <div id="hdr-badge">
      <span class="hdr-chip" id="chip-cmei">—</span>
      <span class="hdr-chip" id="chip-mes">—</span>
      <span class="hdr-chip" id="chip-div">—</span>
    </div>
  </div>
  <div id="tabs">
    <button class="tb at" onclick="goto('info')">📋 Informações</button>
    <button class="tb" onclick="goto('f1')">F1 — Mapa CMEI<span class="dot" id="dot-f1"></span></button>
    <button class="tb" onclick="goto('v1')">V1 — Est. Básicos<span class="dot" id="dot-v1"></span></button>
    <button class="tb" onclick="goto('f2')">F2 — Cardápio<span class="dot" id="dot-f2"></span></button>
    <button class="tb" onclick="goto('v2')">V2 — Est. Perecíveis<span class="dot" id="dot-v2"></span></button>
    <button class="tb" onclick="goto('calc')">📊 Cálculo de Notas<span class="dot" id="dot-calc"></span></button>
    <button class="tb" onclick="goto('rel')">📑 Relatório</button>
  </div>
</div>

<div id="main">

<!-- ══════════════════════════════════════════════════════ INFORMAÇÕES -->
<div id="tela-info" class="tela at">
  <div class="stit">📋 Informações Gerais <span class="tag">INÍCIO</span></div>
  <div class="card">
    <div class="ch ch-g">Identificação do CMEI e Período</div>
    <div class="cb">
      <div class="fg-grid">
        <div class="fg">
          <label>Nome do CMEI</label>
          <input type="text" id="inf-cmei" placeholder="Ex: CMEI Girassol" oninput="si()">
        </div>
        <div class="fg">
          <label>Mês de Referência</label>
          <select id="inf-mes" onchange="si()">
            <option value="">— Selecione —</option>
            <option>Janeiro</option><option>Fevereiro</option><option>Março</option>
            <option>Abril</option><option>Maio</option><option>Junho</option>
            <option>Julho</option><option>Agosto</option><option>Setembro</option>
            <option>Outubro</option><option>Novembro</option><option>Dezembro</option>
          </select>
        </div>
        <div class="fg">
          <label>Ano</label>
          <input type="number" id="inf-ano" value="2025" min="2020" max="2040" oninput="si()">
        </div>
        <div class="fg">
          <label>Nº de Dias do Mês (úteis/letivos)</label>
          <input type="number" id="inf-dias" value="23" min="1" max="31" oninput="si();rebuildF1();rebuildF2()">
          <div class="tip">Máx. 31 dias. Original usa 23 dias letivos.</div>
        </div>
      </div>
      <div class="card" style="margin-top:4px">
        <div class="ch ch-b" style="font-size:13px">Responsáveis</div>
        <div class="cb">
          <div class="resp-grid">
            <div class="fg"><label>Responsável pelas Informações (Merendeira)</label>
              <input type="text" id="inf-r1" placeholder="Nome — Cargo" oninput="si()"></div>
            <div class="fg"><label>Responsável pelo Preenchimento (Secretário)</label>
              <input type="text" id="inf-r2" placeholder="Nome — Cargo" oninput="si()"></div>
            <div class="fg"><label>Visto da Diretora</label>
              <input type="text" id="inf-r3" placeholder="Nome — Diretora" oninput="si()"></div>
            <div class="fg"><label>Data de Fechamento</label>
              <input type="date" id="inf-data" oninput="si()"></div>
          </div>
        </div>
      </div>
      <div class="brow" style="margin-top:14px">
        <button class="btn btn-g" onclick="goto('f1')">▶ Iniciar F1 — Mapa CMEI</button>
        <button class="btn btn-b" onclick="goto('rel')">📑 Ver Relatório Final</button>
        <button class="btn btn-c" onclick="resetAll()" style="margin-left:auto">🗑 Limpar Tudo</button>
      </div>
    </div>
  </div>
  <div class="info-box">
    <strong>Como usar:</strong> Preencha as abas na ordem — <strong>Cálculo de Notas</strong> (lançar NFs) →
    <strong>F1</strong> (registrar consumo diário) → <strong>V1/V2</strong> (conferir estoques, já calculados automaticamente) →
    <strong>F2</strong> (cardápio) → <strong>Relatório</strong> (revisar, corrigir e exportar).
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ F1 -->
<div id="tela-f1" class="tela">
  <div class="stit">F1 — Mapa de CMEI <span class="tag">CONSUMO DIÁRIO</span></div>
  <div class="info-box">
    <strong>F1:</strong> Registre o nº de alunos em cada refeição e o consumo de cada produto básico por dia.
    A linha <strong>TOTAL</strong> soma automaticamente e alimenta as <strong>Saídas da V1</strong>.
  </div>
  <div class="card">
    <div class="ch ch-g">
      Registro Diário de Alunos e Consumo de Produtos
      <button class="btn btn-r btn-sm" onclick="zerarF1()">⚠ Zerar F1</button>
    </div>
    <div class="cb" style="padding:8px">
      <div class="tw" id="f1-tbl"></div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ V1 -->
<div id="tela-v1" class="tela">
  <div class="stit">V1 — Estoque de Básicos <span class="tag">SECOS</span></div>
  <div class="info-box">
    <strong>V1 Básicos:</strong> Saídas calculadas automaticamente da <strong>F1</strong> (linha TOTAL).
    Preencha apenas <em>Saldo Anterior</em> e <em>Entradas</em>.
    <strong>V1 Carnes:</strong> Entradas calculadas automaticamente do <strong>Cálculo de Notas</strong>. Preencha <em>Sobra Anterior</em> e <em>Saídas</em>.
  </div>
  <div class="card">
    <div class="ch ch-g">Produtos Básicos / Secos — Saídas automáticas da F1</div>
    <div class="cb" style="padding:8px"><div class="tw" id="v1-bas"></div></div>
  </div>
  <div class="card">
    <div class="ch ch-b">Perecíveis — Carnes — Entradas automáticas do Cálculo de Notas</div>
    <div class="cb" style="padding:8px"><div class="tw" id="v1-car"></div></div>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ F2 -->
<div id="tela-f2" class="tela">
  <div class="stit">F2 — Cardápio <span class="tag">REFEIÇÕES</span></div>
  <div class="info-box">
    <strong>F2:</strong> Cardápio por dia e refeição. Os dias são sincronizados com a F1.
    Por padrão "Segue conforme o cardápio" — edite conforme necessário.
  </div>
  <div class="card">
    <div class="ch ch-g">Cardápio por Dia e Refeição</div>
    <div class="cb" style="padding:8px"><div class="tw" id="f2-tbl"></div></div>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ V2 -->
<div id="tela-v2" class="tela">
  <div class="stit">V2 — Estoque Perecíveis/Vegetais <span class="tag">FRESCOS</span></div>
  <div class="info-box">
    <strong>V2:</strong> Entradas calculadas automaticamente do <strong>Cálculo de Notas</strong> (coluna TOTAIS).
    Preencha <em>Sobra Anterior</em> e <em>Saídas</em>.
  </div>
  <div class="card">
    <div class="ch ch-g">Vegetais e Frutas — Entradas automáticas do Cálculo de Notas</div>
    <div class="cb" style="padding:8px"><div class="tw" id="v2-tbl"></div></div>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ CÁLCULO DE NOTAS -->
<div id="tela-calc" class="tela">
  <div class="stit">📊 Cálculo de Notas Fiscais <span class="tag">N1 — N50</span></div>
  <div class="info-box">
    <strong>Cálculo de Notas:</strong> Selecione uma nota fiscal e lance as quantidades de cada produto.
    A coluna <strong>TOTAIS</strong> alimenta automaticamente as <em>Entradas da V2</em> (vegetais) e <em>Entradas da V1</em> (carnes).
  </div>
  <div class="card">
    <div class="ch ch-b">
      Notas Fiscais — Clique numa NF para lançar quantidades
      <span id="nf-info" style="font-size:11px;font-weight:400;opacity:.85"></span>
    </div>
    <div class="cb">
      <div class="nf-sel" id="nf-sel"></div>
      <div class="tw" id="calc-tbl"></div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════ RELATÓRIO -->
<div id="tela-rel" class="tela">
  <div class="stit">📑 Relatório Final <span class="tag">SÍNTESE</span></div>
  <div class="brow">
    <button class="btn btn-g" onclick="buildRel()">🔄 Atualizar</button>
    <button class="btn btn-b" onclick="expPDF()">🖨 Exportar PDF</button>
    <button class="btn btn-am" onclick="expXLSX()">📊 Exportar XLSX Espelho</button>
  </div>
  <div id="rel"></div>
</div>

</div><!-- /main -->

<script>
// ╔═══════════════════════════════════════════════════════════════════╗
// ║  DADOS — LISTAS DE PRODUTOS                                       ║
// ╚═══════════════════════════════════════════════════════════════════╝
const V1B = [
  {id:'b01',n:'Açafrão',u:'Kg'},{id:'b02',n:'Alecrim 0,05',u:'Kg'},
  {id:'b03',n:'Amido de milho',u:'Kg'},{id:'b04',n:'Arroz - 1 kg',u:'Kg'},
  {id:'b05',n:'Arroz Integral 1kg',u:'Kg'},{id:'b06',n:'Aveia',u:'Kg'},
  {id:'b07',n:'Aveia Em flocos',u:'Kg'},{id:'b08',n:'Azeite de oliva (dieta)',u:'L'},
  {id:'b09',n:'Cacau em pó 0,5',u:'Kg'},{id:'b10',n:'Canela em pó',u:'Kg'},
  {id:'b11',n:'Canjica',u:'Kg'},{id:'b12',n:'Canjica 0,5',u:'Kg'},
  {id:'b13',n:'Chá de erva cidreira',u:'100g'},{id:'b14',n:'Chá Erva doce - 1 kg',u:'Kg'},
  {id:'b15',n:'Coco ralado',u:'Kg'},{id:'b16',n:'Colorau 0,5',u:'Kg'},
  {id:'b17',n:'Creme de leite (dieta)',u:'Un.'},{id:'b18',n:'Doce de Banana',u:'Pote'},
  {id:'b19',n:'Ervilha',u:'Un.'},{id:'b20',n:'Extrato de tomate 0,350GR',u:'Kg'},
  {id:'b21',n:'Farelo de aveia',u:'Kg'},{id:'b22',n:'Farelo de trigo',u:'Kg'},
  {id:'b23',n:'Farinha de Kibe 0,5',u:'Kg'},{id:'b24',n:'Farinha de mandióca 1kg',u:'Kg'},
  {id:'b25',n:'Farinha de milho 1kg',u:'Kg'},{id:'b26',n:'Farinha de trigo 1kg',u:'Kg'},
  {id:'b27',n:'Farinha de trigo integral 1kg',u:'Kg'},{id:'b28',n:'Feijão 1kg',u:'Kg'},
  {id:'b29',n:'Feijão carióca',u:'Kg'},{id:'b30',n:'Fermento biológico pão 10g',u:'Un.'},
  {id:'b31',n:'Fermento biológico pão 125g',u:'Un.'},{id:'b32',n:'Fermento químico bolo 0,100g',u:'Un.'},
  {id:'b33',n:'Fibra de Trigo',u:'Kg'},{id:'b34',n:'fubá pré cozido 1kg',u:'Kg'},
  {id:'b35',n:'Leite de soja',u:'Cx'},{id:'b36',n:'Leite em pó (400g e 1kg)',u:'Kg'},
  {id:'b37',n:'Leite integral UHT 1 lt',u:'L'},{id:'b38',n:'Leite sem lactose',u:'L'},
  {id:'b39',n:'Lentilha 0,5',u:'Kg'},{id:'b40',n:'Macarrão Argolinha (sopa) 0,5',u:'Kg'},
  {id:'b41',n:'Macarrão ave maria 0,5',u:'Kg'},{id:'b42',n:'Macarrão conchinha 0,5',u:'Kg'},
  {id:'b43',n:'Macarrão Parafuso 0,5',u:'Kg'},{id:'b44',n:'Macarrão Penne 0,5',u:'Kg'},
  {id:'b45',n:'Macarrão sopa 0,5',u:'Kg'},{id:'b46',n:'Margarina/manteiga',u:'Un.'},
  {id:'b47',n:'Milho verde',u:'Un.'},{id:'b48',n:'Molho de tomate 0,340Grs',u:'Kg'},
  {id:'b49',n:'Óleo de milho 0,900ml',u:'Un.'},{id:'b50',n:'Óleo de soja 0,900 ml',u:'Un.'},
  {id:'b51',n:'Páprica',u:'Kg'},{id:'b52',n:'Pipoca 0,5',u:'Kg'},
  {id:'b53',n:'Polvilho doce ou azedo',u:'Kg'},{id:'b54',n:'Proteína de soja (dieta)',u:'Kg'},
  {id:'b55',n:'Quiréra',u:'Kg'},{id:'b56',n:'Requeijão',u:'Kg'},
  {id:'b57',n:'Sal 1kg',u:'Kg'},{id:'b58',n:'Sardinha 0,125GRs',u:'Un.'},
  {id:'b59',n:'Suco 1lt',u:'L'},{id:'b60',n:'Tomilho',u:'Kg'},
  {id:'b61',n:'Vinagre 750ml',u:'Un.'},
  {id:'bc1',n:'',u:'Kg',custom:1},{id:'bc2',n:'',u:'Kg',custom:1},
  {id:'bc3',n:'',u:'Kg',custom:1},{id:'bc4',n:'',u:'Kg',custom:1},
  {id:'bc5',n:'',u:'Kg',custom:1},{id:'bc6',n:'',u:'Kg',custom:1},
  {id:'bc7',n:'',u:'Kg',custom:1},{id:'bc8',n:'',u:'Kg',custom:1},
  {id:'bc9',n:'',u:'Kg',custom:1},{id:'bc10',n:'',u:'Kg',custom:1},
];

const V1C = [
  {id:'c01',n:'Acém',u:'Kg'},{id:'c02',n:'Cação',u:'Kg'},
  {id:'c03',n:'Copa lombo iscas/tiras/bife',u:'Kg'},{id:'c04',n:'Coxa com sobrecoxa',u:'Kg'},
  {id:'c05',n:'Coxão mole cubos',u:'Kg'},{id:'c06',n:'Coxão mole tiras',u:'Kg'},
  {id:'c07',n:'Fígado de galinha',u:'Kg'},{id:'c08',n:'Filé de peito de frango',u:'Kg'},
  {id:'c09',n:'Filé de tilápia',u:'Kg'},{id:'c10',n:'Frango',u:'Kg'},
  {id:'c11',n:'Lingüiça de frango',u:'Kg'},{id:'c12',n:'Moela',u:'Kg'},
  {id:'c13',n:'Moída de frango',u:'Kg'},{id:'c14',n:'Músculo cubos',u:'Kg'},
  {id:'c15',n:'Ovos',u:'Dz'},{id:'c16',n:'Patinho moído/iscas/CUBOS',u:'Kg'},
  {id:'c17',n:'Peito de frango',u:'Kg'},{id:'c18',n:'Peito de frango sem osso',u:'Kg'},
  {id:'c19',n:'Peito de frango sem osso Filé',u:'Kg'},{id:'c20',n:'Pernil Iscas',u:'Kg'},
  {id:'c21',n:'Posta lagarto',u:'Kg'},{id:'c22',n:'Posta vermelha',u:'Kg'},
  {id:'c23',n:'Sassami',u:'Kg'},
  {id:'cc1',n:'',u:'Kg',custom:1},{id:'cc2',n:'',u:'Kg',custom:1},
  {id:'cc3',n:'',u:'Kg',custom:1},{id:'cc4',n:'',u:'Kg',custom:1},
  {id:'cc5',n:'',u:'Kg',custom:1},{id:'cc6',n:'',u:'Kg',custom:1},
];

const V2V = [
  {id:'v01',n:'Abacaxi',u:'Kg'},{id:'v02',n:'Abacate',u:'Kg'},
  {id:'v03',n:'Abóbora',u:'Kg'},{id:'v04',n:'Abóbrinha',u:'Kg'},
  {id:'v05',n:'Açafrão',u:'gm'},{id:'v06',n:'Acelga',u:'Kg'},
  {id:'v07',n:'Agrião',u:'Kg'},{id:'v08',n:'Aipim',u:'Kg'},
  {id:'v09',n:'Alecrim',u:'gm'},{id:'v10',n:'Alface',u:'Kg'},
  {id:'v11',n:'Alho',u:'Kg'},{id:'v12',n:'Almeirão',u:'Kg'},
  {id:'v13',n:'Ameixa',u:'Kg'},{id:'v14',n:'Banana',u:'Kg'},
  {id:'v15',n:'Batata',u:'Kg'},{id:'v16',n:'Batata doce',u:'Kg'},
  {id:'v17',n:'Batata salsa',u:'Kg'},{id:'v18',n:'Beringela',u:'Kg'},
  {id:'v19',n:'Beterraba',u:'Kg'},{id:'v20',n:'Brócolis',u:'Kg'},
  {id:'v21',n:'Caqui',u:'Kg'},{id:'v22',n:'Carambola',u:'Kg'},
  {id:'v23',n:'Cebola',u:'Kg'},{id:'v24',n:'Cebolinha',u:'Kg'},
  {id:'v25',n:'Cenoura',u:'Kg'},{id:'v26',n:'Cheiro verde',u:'Kg'},
  {id:'v27',n:'Chuchu',u:'Kg'},{id:'v28',n:'Couve manteiga',u:'Kg'},
  {id:'v29',n:'Couve-flor',u:'Kg'},{id:'v30',n:'Curry',u:'gm'},
  {id:'v31',n:'Ervas finas',u:'gm'},{id:'v32',n:'Ervilha',u:'Kg'},
  {id:'v33',n:'Escarola',u:'gm'},{id:'v34',n:'Espinafre',u:'Kg'},
  {id:'v35',n:'Goiaba',u:'Kg'},{id:'v36',n:'Laranja',u:'Kg'},
  {id:'v37',n:'Limão',u:'Kg'},{id:'v38',n:'Linhaça',u:'Kg'},
  {id:'v39',n:'Louro',u:'gm'},{id:'v40',n:'Maçã',u:'Kg'},
  {id:'v41',n:'Mamão',u:'Kg'},{id:'v42',n:'Mandióca',u:'Kg'},
  {id:'v43',n:'Manga',u:'Kg'},{id:'v44',n:'Manjericão',u:'0,1'},
  {id:'v45',n:'Manjerona',u:'0,05'},{id:'v46',n:'Maracujá',u:'Kg'},
  {id:'v47',n:'Melância',u:'Kg'},{id:'v48',n:'Melão',u:'Kg'},
  {id:'v49',n:'Melão pele de sapo',u:'Kg'},{id:'v50',n:'Milho',u:'Kg'},
  {id:'v51',n:'Morango',u:'Kg'},{id:'v52',n:'Morgote',u:'Kg'},
  {id:'v53',n:'Mostarda',u:'Kg'},{id:'v54',n:'Pepino',u:'Kg'},
  {id:'v55',n:'Pêra',u:'Kg'},{id:'v56',n:'Pêssego',u:'Kg'},
  {id:'v57',n:'Pimentão',u:'Kg'},{id:'v58',n:'Pokan, mexerica',u:'Kg'},
  {id:'v59',n:'Rabanete',u:'Kg'},{id:'v60',n:'Repolho',u:'Kg'},
  {id:'v61',n:'Rúcula',u:'Kg'},{id:'v62',n:'Salsinha',u:'Kg'},
  {id:'v63',n:'Tempero completo',u:'Kg'},{id:'v64',n:'Tomate',u:'0,5'},
  {id:'v65',n:'Tomate cereja',u:'Kg'},{id:'v66',n:'Uva',u:'Kg'},
  {id:'v67',n:'Vagem',u:'Kg'},
  {id:'vc1',n:'',u:'Kg',custom:1},{id:'vc2',n:'',u:'Kg',custom:1},
  {id:'vc3',n:'',u:'Kg',custom:1},{id:'vc4',n:'',u:'Kg',custom:1},
  {id:'vc5',n:'',u:'Kg',custom:1},
];

const CALC_ALL = [...V2V,...V1C]; // all products in Cálculo de Notas

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  ESTADO                                                           ║
// ╚═══════════════════════════════════════════════════════════════════╝
let S = {};
let nfAtiva = 'N1';
let telaCurrent = 'info';

function initS(){
  S = {
    info:{cmei:'',mes:'',ano:new Date().getFullYear(),dias:23,r1:'',r2:'',r3:'',data:''},
    f1: Array(31).fill(null).map(()=>({cafe:0,almoco:0,lanche:0,jantar:0,c:{}})),
    v1b:{}, v1c:{},
    f2: Array(31).fill(null).map(()=>({cafe:'Segue conforme o cardápio',almoco:'Segue conforme o cardápio',lanche:'Segue conforme o cardápio',jantar:'Segue conforme o cardápio'})),
    v2:{}, calc:{}
  };
  V1B.forEach(p=>{S.v1b[p.id]={sa:0,ent:0,nome:p.n,u:p.u}});
  V1C.forEach(p=>{S.v1c[p.id]={sa:0,said:0,nome:p.n,u:p.u}});
  V2V.forEach(p=>{S.v2[p.id]={sa:0,said:0,nome:p.n,u:p.u}});
  CALC_ALL.forEach(p=>{S.calc[p.id]={}});
}

function save(){try{localStorage.setItem('cmei_s',JSON.stringify(S))}catch(e){}}

function load(){
  try{
    const raw=localStorage.getItem('cmei_s');
    if(!raw) return;
    const d=JSON.parse(raw);
    if(d.info) S.info={...S.info,...d.info};
    if(d.f1&&d.f1.length) S.f1=d.f1.map((x,i)=>x||S.f1[i]);
    if(d.v1b) Object.keys(d.v1b).forEach(k=>{if(S.v1b[k]) S.v1b[k]={...S.v1b[k],...d.v1b[k]}});
    if(d.v1c) Object.keys(d.v1c).forEach(k=>{if(S.v1c[k]) S.v1c[k]={...S.v1c[k],...d.v1c[k]}});
    if(d.f2&&d.f2.length) S.f2=d.f2.map((x,i)=>x||S.f2[i]);
    if(d.v2) Object.keys(d.v2).forEach(k=>{if(S.v2[k]) S.v2[k]={...S.v2[k],...d.v2[k]}});
    if(d.calc) Object.keys(d.calc).forEach(k=>{if(S.calc[k]!==undefined) S.calc[k]={...S.calc[k],...d.calc[k]}});
  }catch(e){}
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  CÁLCULOS                                                         ║
// ╚═══════════════════════════════════════════════════════════════════╝
function f1TotProd(){
  const t={};
  V1B.forEach(p=>{t[p.id]=0});
  S.f1.forEach(d=>{
    if(!d||!d.c)return;
    V1B.forEach(p=>{t[p.id]+=+(d.c[p.id]||0)});
  });
  return t;
}

function f1TotAlunos(){
  let c=0,a=0,l=0,j=0;
  S.f1.forEach(d=>{c+=+(d.cafe||0);a+=+(d.almoco||0);l+=+(d.lanche||0);j+=+(d.jantar||0)});
  return{cafe:c,almoco:a,lanche:l,jantar:j};
}

function calcTot(){
  const t={};
  CALC_ALL.forEach(p=>{
    let s=0;
    for(let i=1;i<=50;i++) s+=+(S.calc[p.id]?.[`N${i}`]||0);
    t[p.id]=round2(s);
  });
  return t;
}

function v1bCalc(){
  const f=f1TotProd();
  const r={};
  V1B.forEach(p=>{
    const d=S.v1b[p.id]||{};
    const sa=+(d.sa||0),ent=+(d.ent||0),said=round2(f[p.id]||0);
    r[p.id]={sa,ent,said,saldo:round2(sa+ent-said)};
  });
  return r;
}

function v1cCalc(){
  const ct=calcTot();
  const r={};
  V1C.forEach(p=>{
    const d=S.v1c[p.id]||{};
    const sa=+(d.sa||0),ent=round2(ct[p.id]||0),said=+(d.said||0);
    r[p.id]={sa,ent,said,saldo:round2(sa+ent-said)};
  });
  return r;
}

function v2Calc(){
  const ct=calcTot();
  const r={};
  V2V.forEach(p=>{
    const d=S.v2[p.id]||{};
    const sa=+(d.sa||0),ent=round2(ct[p.id]||0),said=+(d.said||0);
    r[p.id]={sa,ent,said,saldo:round2(sa+ent-said)};
  });
  return r;
}

function round2(v){return Math.round(v*1000)/1000}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  NAVEGAÇÃO                                                        ║
// ╚═══════════════════════════════════════════════════════════════════╝
function goto(id){
  document.querySelectorAll('.tela').forEach(t=>t.classList.remove('at'));
  document.querySelectorAll('.tb').forEach(b=>b.classList.remove('at'));
  document.getElementById('tela-'+id).classList.add('at');
  document.querySelectorAll('.tb').forEach(b=>{
    if(b.getAttribute('onclick')===`goto('${id}')`) b.classList.add('at');
  });
  telaCurrent=id;
  if(id==='f1') renderF1();
  if(id==='v1') renderV1();
  if(id==='f2') renderF2();
  if(id==='v2') renderV2();
  if(id==='calc') renderCalc();
  if(id==='rel') buildRel();
  updateHeaderChips();
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  INFORMAÇÕES                                                      ║
// ╚═══════════════════════════════════════════════════════════════════╝
function si(){
  S.info.cmei=el('inf-cmei').value;
  S.info.mes=el('inf-mes').value;
  S.info.ano=el('inf-ano').value;
  S.info.dias=parseInt(el('inf-dias').value)||23;
  S.info.r1=el('inf-r1').value;
  S.info.r2=el('inf-r2').value;
  S.info.r3=el('inf-r3').value;
  S.info.data=el('inf-data').value;
  save();
  updateHeaderChips();
}

function loadInfoForm(){
  el('inf-cmei').value=S.info.cmei||'';
  el('inf-mes').value=S.info.mes||'';
  el('inf-ano').value=S.info.ano||new Date().getFullYear();
  el('inf-dias').value=S.info.dias||23;
  el('inf-r1').value=S.info.r1||'';
  el('inf-r2').value=S.info.r2||'';
  el('inf-r3').value=S.info.r3||'';
  el('inf-data').value=S.info.data||'';
}

function updateHeaderChips(){
  el('chip-cmei').textContent=S.info.cmei||'CMEI não definido';
  el('chip-mes').textContent=(S.info.mes?S.info.mes+'/':'')+S.info.ano;
  // Count divergências
  const divs=getDivergencias();
  const dc=el('chip-div');
  if(divs.length===0){
    dc.textContent='✓ Sem Divergências';
    dc.className='hdr-chip ok';
  } else {
    dc.textContent=`⚠ ${divs.length} Divergência(s)`;
    dc.className='hdr-chip warn';
  }
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  F1 — RENDER                                                      ║
// ╚═══════════════════════════════════════════════════════════════════╝
function renderF1(){
  const dias=S.info.dias||23;
  const prods=V1B.filter(p=>!p.custom||nomeP(p,'b'));
  const tf=f1TotProd(),ta=f1TotAlunos();

  let h='<table id="tf1"><thead><tr>';
  h+=`<th class="sk" rowspan="2" style="min-width:40px">Dia</th>`;
  h+=`<th rowspan="2" style="min-width:62px">Café<br><small>(alunos)</small></th>`;
  h+=`<th rowspan="2" style="min-width:62px">Almoço<br><small>(alunos)</small></th>`;
  h+=`<th rowspan="2" style="min-width:62px">Lanche<br><small>(alunos)</small></th>`;
  h+=`<th rowspan="2" style="min-width:62px">Jantar<br><small>(alunos)</small></th>`;
  h+=`<th colspan="${prods.length}" style="background:var(--b1)">Consumo de Produtos Básicos (Kg/Un.)</th>`;
  h+='</tr><tr>';
  prods.forEach(p=>{
    const nm=nomeP(p,'b');
    h+=`<th class="vert" title="${nm}">${nm}</th>`;
  });
  h+='</tr></thead><tbody>';

  for(let d=0;d<dias;d++){
    const dia=S.f1[d]||{cafe:0,almoco:0,lanche:0,jantar:0,c:{}};
    h+=`<tr><td class="nc" style="font-weight:700;font-size:13px">${d+1}</td>`;
    h+=inp_n(`setFA(${d},'cafe',this.value)`,dia.cafe,62,1);
    h+=inp_n(`setFA(${d},'almoco',this.value)`,dia.almoco,62,1);
    h+=inp_n(`setFA(${d},'lanche',this.value)`,dia.lanche,62,1);
    h+=inp_n(`setFA(${d},'jantar',this.value)`,dia.jantar,62,1);
    prods.forEach(p=>{
      h+=inp_n(`setFC(${d},'${p.id}',this.value)`,(dia.c||{})[p.id]||0,68,0.001);
    });
    h+='</tr>';
  }

  h+=`<tr class="tr-tot"><td class="nc">TOTAL</td>`;
  h+=`<td class="total-row">${ta.cafe}</td><td>${ta.almoco}</td><td>${ta.lanche}</td><td>${ta.jantar}</td>`;
  prods.forEach(p=>{
    const v=round2(tf[p.id]||0);
    h+=`<td id="f1t_${p.id}">${v||''}</td>`;
  });
  h+='</tr></tbody></table>';
  el('f1-tbl').innerHTML=h;
  dotOn('f1',hasDados('f1'));
}

function inp_n(onchange,val,w,step){
  const v=(+val||0);
  return `<td><input class="inp" type="number" style="width:${w-6}px" min="0" step="${step}" value="${v||''}" placeholder="0" onchange="${onchange}"></td>`;
}

function setFA(d,ref,v){
  if(!S.f1[d]) S.f1[d]={cafe:0,almoco:0,lanche:0,jantar:0,c:{}};
  S.f1[d][ref]=+v||0;save();updF1Totals();
  if(telaCurrent==='v1') renderV1();
}
function setFC(d,id,v){
  if(!S.f1[d]) S.f1[d]={cafe:0,almoco:0,lanche:0,jantar:0,c:{}};
  if(!S.f1[d].c) S.f1[d].c={};
  S.f1[d].c[id]=+v||0;save();updF1Totals();
  if(telaCurrent==='v1') renderV1();
}
function updF1Totals(){
  const tf=f1TotProd(),ta=f1TotAlunos();
  const tbl=el('tf1'); if(!tbl) return;
  const lastRow=tbl.querySelector('tbody tr:last-child');
  if(!lastRow) return;
  const cells=lastRow.querySelectorAll('td');
  cells[1].textContent=ta.cafe;cells[2].textContent=ta.almoco;
  cells[3].textContent=ta.lanche;cells[4].textContent=ta.jantar;
  const prods=V1B.filter(p=>!p.custom||nomeP(p,'b'));
  prods.forEach((p,i)=>{
    const v=round2(tf[p.id]||0);
    if(cells[5+i]) cells[5+i].textContent=v||'';
  });
  updateHeaderChips();
}
function zerarF1(){if(!confirm('Zerar todos os dados da F1?'))return;
  S.f1=Array(31).fill(null).map(()=>({cafe:0,almoco:0,lanche:0,jantar:0,c:{}}));
  save();renderF1();}
function rebuildF1(){if(telaCurrent==='f1') renderF1();}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  V1 — RENDER                                                      ║
// ╚═══════════════════════════════════════════════════════════════════╝
function renderV1(){
  // Básicos
  const bCalc=v1bCalc();
  let h='<table><thead><tr>';
  h+='<th class="sk2" style="min-width:185px">Produto</th>';
  h+='<th style="min-width:50px">Unid.</th>';
  h+='<th style="min-width:85px">Saldo Anterior</th>';
  h+='<th style="min-width:85px">Entradas</th>';
  h+='<th style="min-width:85px;background:#7a2010">Saídas (F1)</th>';
  h+='<th style="min-width:85px;background:var(--b1)">Saldo Atual</th>';
  h+='</tr></thead><tbody>';
  V1B.forEach(p=>{
    const c=bCalc[p.id]||{};
    const nm=nomeP(p,'b');
    const nmCell=p.custom
      ?`<input class="inp inp-w" type="text" value="${escH(nm)}" placeholder="(produto livre)" onchange="setNm('${p.id}','b',this.value)" style="width:170px">`
      :escH(nm);
    const u=S.v1b[p.id]?.u||p.u;
    h+=`<tr>
      <td class="nc">${nmCell}</td><td>${u}</td>
      <td>${inpN(`setSA('${p.id}','b',v)`,c.sa,85)}</td>
      <td>${inpN(`setEnt('${p.id}','b',v)`,c.ent,85)}</td>
      <td class="said">${fmtN(c.said)}</td>
      <td class="${c.saldo<0?'neg':'entr'}">${fmtN(c.saldo)}</td>
    </tr>`;
  });
  h+='</tbody></table>';
  el('v1-bas').innerHTML=h;

  // Carnes
  const cCalc=v1cCalc();
  let h2='<table><thead><tr>';
  h2+='<th class="sk2" style="min-width:185px">Produto (Carne)</th>';
  h2+='<th style="min-width:50px">Unid.</th>';
  h2+='<th style="min-width:85px">Sobra Anterior</th>';
  h2+='<th style="min-width:85px;background:var(--g1)">Entradas (NF)</th>';
  h2+='<th style="min-width:85px">Saídas</th>';
  h2+='<th style="min-width:85px;background:var(--b1)">Saldo Atual</th>';
  h2+='</tr></thead><tbody>';
  V1C.forEach(p=>{
    const c=cCalc[p.id]||{};
    const nm=nomeP(p,'c');
    const nmCell=p.custom
      ?`<input class="inp inp-w" type="text" value="${escH(nm)}" placeholder="(produto livre)" onchange="setNm('${p.id}','c',this.value)" style="width:170px">`
      :escH(nm);
    const u=S.v1c[p.id]?.u||p.u;
    h2+=`<tr>
      <td class="nc">${nmCell}</td><td>${u}</td>
      <td>${inpN(`setSA('${p.id}','c',v)`,c.sa,85)}</td>
      <td class="entr">${fmtN(c.ent)}</td>
      <td>${inpN(`setSaid('${p.id}','c',v)`,c.said,85)}</td>
      <td class="${c.saldo<0?'neg':'entr'}">${fmtN(c.saldo)}</td>
    </tr>`;
  });
  h2+='</tbody></table>';
  el('v1-car').innerHTML=h2;
  dotOn('v1',hasDados('v1'));
}

function inpN(onchange_v,val,w){
  return `<input class="inp" type="number" style="width:${w-10}px" min="0" step="0.001" value="${+val||''}" placeholder="0" onchange="const v=+this.value||0;${onchange_v};this.closest('tr').querySelectorAll('td')[5].className=(this.value<0?'neg':'entr')">`;
}
function setSA(id,sec,v){
  if(sec==='b'){S.v1b[id].sa=+v||0}
  else if(sec==='c'){S.v1c[id].sa=+v||0}
  else{S.v2[id].sa=+v||0}
  save();renderV1();
}
function setEnt(id,sec,v){S.v1b[id].ent=+v||0;save();renderV1();}
function setSaid(id,sec,v){
  if(sec==='c'){S.v1c[id].said=+v||0}
  else{S.v2[id].said=+v||0}
  save();renderV2?renderV2():0;
}
function setNm(id,sec,v){
  if(sec==='b'){S.v1b[id].nome=v}
  else if(sec==='c'){S.v1c[id].nome=v}
  else{S.v2[id].nome=v}
  save();
  if(telaCurrent==='f1') renderF1();
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  F2 — RENDER                                                      ║
// ╚═══════════════════════════════════════════════════════════════════╝
function renderF2(){
  const dias=S.info.dias||23;
  let h='<table><thead><tr>';
  h+='<th class="sk" style="min-width:40px">Dia</th>';
  h+='<th style="min-width:190px">Café da Manhã</th>';
  h+='<th style="min-width:190px">Almoço</th>';
  h+='<th style="min-width:190px">Lanche da Tarde</th>';
  h+='<th style="min-width:190px">Jantar</th>';
  h+='</tr></thead><tbody>';
  for(let d=0;d<dias;d++){
    const f=S.f2[d]||{cafe:'',almoco:'',lanche:'',jantar:''};
    h+=`<tr>
      <td class="nc" style="font-weight:700;font-size:13px">${d+1}</td>
      <td><textarea class="inp-ta" onchange="setF2(${d},'cafe',this.value)">${escH(f.cafe||'')}</textarea></td>
      <td><textarea class="inp-ta" onchange="setF2(${d},'almoco',this.value)">${escH(f.almoco||'')}</textarea></td>
      <td><textarea class="inp-ta" onchange="setF2(${d},'lanche',this.value)">${escH(f.lanche||'')}</textarea></td>
      <td><textarea class="inp-ta" onchange="setF2(${d},'jantar',this.value)">${escH(f.jantar||'')}</textarea></td>
    </tr>`;
  }
  h+='</tbody></table>';
  el('f2-tbl').innerHTML=h;
  dotOn('f2',hasDados('f2'));
}
function setF2(d,ref,v){
  if(!S.f2[d]) S.f2[d]={cafe:'',almoco:'',lanche:'',jantar:''};
  S.f2[d][ref]=v;save();
}
function rebuildF2(){if(telaCurrent==='f2') renderF2();}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  V2 — RENDER                                                      ║
// ╚═══════════════════════════════════════════════════════════════════╝
function renderV2(){
  const vc=v2Calc();
  let h='<table><thead><tr>';
  h+='<th class="sk2" style="min-width:165px">Produto</th>';
  h+='<th style="min-width:50px">Unid.</th>';
  h+='<th style="min-width:85px">Sobra Anterior</th>';
  h+='<th style="min-width:85px;background:var(--g1)">Entradas (NF)</th>';
  h+='<th style="min-width:85px">Saídas</th>';
  h+='<th style="min-width:85px;background:var(--b1)">Saldo Atual</th>';
  h+='</tr></thead><tbody>';
  V2V.forEach(p=>{
    const c=vc[p.id]||{};
    const nm=nomeP(p,'v');
    const nmCell=p.custom
      ?`<input class="inp inp-w" type="text" value="${escH(nm)}" placeholder="(produto livre)" onchange="setNm('${p.id}','v',this.value)" style="width:148px">`
      :escH(nm);
    const u=S.v2[p.id]?.u||p.u;
    h+=`<tr>
      <td class="nc">${nmCell}</td><td>${u}</td>
      <td>${inpN(`setSA('${p.id}','v',v)`,c.sa,85)}</td>
      <td class="entr">${fmtN(c.ent)}</td>
      <td>${inpN(`setSaid('${p.id}','v',v)`,c.said,85)}</td>
      <td class="${c.saldo<0?'neg':'entr'}">${fmtN(c.saldo)}</td>
    </tr>`;
  });
  h+='</tbody></table>';
  el('v2-tbl').innerHTML=h;
  dotOn('v2',hasDados('v2'));
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  CÁLCULO DE NOTAS — RENDER                                        ║
// ╚═══════════════════════════════════════════════════════════════════╝
function renderCalc(){
  const ct=calcTot();
  let nfsData=new Set();
  CALC_ALL.forEach(p=>{
    for(let i=1;i<=50;i++) if(+(S.calc[p.id]?.[`N${i}`]||0)>0) nfsData.add(`N${i}`);
  });

  // NF selector
  let sel='';
  for(let i=1;i<=50;i++){
    const nf=`N${i}`;
    const has=nfsData.has(nf)?'has':'';
    const at=nfAtiva===nf?'ativo':'';
    sel+=`<button class="nf-btn ${has} ${at}" onclick="selNF('${nf}')">${nf}</button>`;
  }
  el('nf-sel').innerHTML=sel;
  el('nf-info').textContent=nfsData.size>0?`${nfsData.size} nota(s) com dados lançados`:'Nenhuma nota com dados';

  // Table
  let h='<table><thead><tr>';
  h+='<th class="sk2" style="min-width:175px">Produto</th>';
  h+=`<th style="background:var(--b1);min-width:95px">${nfAtiva} — Quantidade</th>`;
  h+='<th style="background:var(--g1);min-width:85px">TOTAIS (todas NFs)</th>';
  h+='</tr></thead><tbody>';

  // Vegetais section
  h+=`<tr class="tr-sep"><td colspan="3">🌿 VEGETAIS / FRUTAS — Entradas → V2</td></tr>`;
  V2V.forEach(p=>{
    const nm=nomeP(p,'v');if(!nm&&p.custom) return;
    const val=+(S.calc[p.id]?.[nfAtiva]||0);
    const tot=ct[p.id]||0;
    h+=`<tr>
      <td class="nc">${escH(nm)}</td>
      <td><input class="inp inp-lg" type="number" min="0" step="0.001" value="${val||''}" placeholder="0"
        onchange="setCalc('${p.id}','${nfAtiva}',this.value)"></td>
      <td class="entr" id="ct_${p.id}">${tot||''}</td>
    </tr>`;
  });

  // Carnes section
  h+=`<tr class="tr-sep"><td colspan="3">🥩 CARNES — Entradas → V1 Carnes</td></tr>`;
  V1C.forEach(p=>{
    const nm=nomeP(p,'c');if(!nm&&p.custom) return;
    const val=+(S.calc[p.id]?.[nfAtiva]||0);
    const tot=ct[p.id]||0;
    h+=`<tr>
      <td class="nc">${escH(nm)}</td>
      <td><input class="inp inp-lg" type="number" min="0" step="0.001" value="${val||''}" placeholder="0"
        onchange="setCalc('${p.id}','${nfAtiva}',this.value)"></td>
      <td class="entr" id="ct_${p.id}">${tot||''}</td>
    </tr>`;
  });

  h+='</tbody></table>';
  el('calc-tbl').innerHTML=h;
  dotOn('calc',nfsData.size>0);
}

function selNF(nf){nfAtiva=nf;renderCalc();}

function setCalc(id,nf,v){
  if(!S.calc[id]) S.calc[id]={};
  S.calc[id][nf]=+v||0;
  save();
  // Update total cell
  const ct=calcTot();
  const cell=document.getElementById('ct_'+id);
  if(cell) cell.textContent=ct[id]||'';
  // Update NF button style
  let has=false;
  CALC_ALL.forEach(p=>{if(+(S.calc[p.id]?.[nf]||0)>0) has=true});
  document.querySelectorAll('.nf-btn').forEach(b=>{
    if(b.textContent.trim()===nf){b.classList.toggle('has',has)}
  });
  if(telaCurrent==='v2') renderV2();
  if(telaCurrent==='v1') renderV1();
  updateHeaderChips();
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  RELATÓRIO                                                        ║
// ╚═══════════════════════════════════════════════════════════════════╝
function getDivergencias(){
  const divs=[];
  const bc=v1bCalc(),cc=v1cCalc(),vc=v2Calc();
  V1B.forEach(p=>{const c=bc[p.id];if(c&&c.saldo<0) divs.push({sec:'V1 Básicos',id:p.id,nome:nomeP(p,'b'),said:c.said,ent:c.ent,sa:c.sa,saldo:c.saldo})});
  V1C.forEach(p=>{const c=cc[p.id];if(c&&c.saldo<0) divs.push({sec:'V1 Carnes',id:p.id,nome:nomeP(p,'c'),said:c.said,ent:c.ent,sa:c.sa,saldo:c.saldo})});
  V2V.forEach(p=>{const c=vc[p.id];if(c&&c.saldo<0) divs.push({sec:'V2 Vegetais',id:p.id,nome:nomeP(p,'v'),said:c.said,ent:c.ent,sa:c.sa,saldo:c.saldo})});
  return divs;
}

function buildRel(){
  const bc=v1bCalc(),cc=v1cCalc(),vc=v2Calc();
  const ta=f1TotAlunos();
  const divs=getDivergencias();
  const dias=S.info.dias||23;
  let nfs=new Set();
  CALC_ALL.forEach(p=>{for(let i=1;i<=50;i++) if(+(S.calc[p.id]?.[`N${i}`]||0)>0) nfs.add(`N${i}`)});

  const v1bMov=V1B.filter(p=>{const c=bc[p.id];return c&&(c.sa>0||c.ent>0||c.said>0)});
  const v1cMov=V1C.filter(p=>{const c=cc[p.id];return c&&(c.sa>0||c.ent>0||c.said>0)});
  const v2Mov=V2V.filter(p=>{const c=vc[p.id];return c&&(c.sa>0||c.ent>0||c.said>0)});

  let h='';

  // Identificação
  h+=`<div class="card"><div class="ch ch-g">📋 Identificação do Período</div><div class="cb">
    <div class="rel-g">
      <div class="rel-item"><h4>CMEI</h4><p>${escH(S.info.cmei)||'—'}</p></div>
      <div class="rel-item"><h4>Período</h4><p>${S.info.mes||'—'} / ${S.info.ano||'—'}</p></div>
      <div class="rel-item"><h4>Dias Registrados</h4><p>${dias}</p></div>
      <div class="rel-item"><h4>Notas Fiscais</h4><p>${nfs.size}</p></div>
      <div class="rel-item ${divs.length>0?'alert':''}"><h4>Divergências</h4><p>${divs.length}</p></div>
    </div>
  </div></div>`;

  // F1
  h+=`<div class="card"><div class="ch ch-b">F1 — Resumo de Atendimento</div><div class="cb">
    <div class="rel-g">
      <div class="rel-item"><h4>Total Café</h4><p>${ta.cafe}</p></div>
      <div class="rel-item"><h4>Total Almoço</h4><p>${ta.almoco}</p></div>
      <div class="rel-item"><h4>Total Lanche</h4><p>${ta.lanche}</p></div>
      <div class="rel-item"><h4>Total Jantar</h4><p>${ta.jantar}</p></div>
    </div>
  </div></div>`;

  // V1 Básicos
  h+=relTabela('V1 — Estoque Básicos','ch-g',v1bMov,bc,'b',
    ['Produto','Unid.','Saldo Ant.','Entradas','Saídas (F1)','Saldo Atual'],false);

  // V1 Carnes
  h+=relTabela('V1 — Carnes','ch-b',v1cMov,cc,'c',
    ['Produto','Unid.','Sobra Ant.','Entradas (NF)','Saídas','Saldo Atual'],false);

  // V2
  h+=relTabela('V2 — Estoque Perecíveis/Vegetais','ch-g',v2Mov,vc,'v',
    ['Produto','Unid.','Sobra Ant.','Entradas (NF)','Saídas','Saldo Atual'],false);

  // Divergências
  h+=`<div class="card"><div class="ch ${divs.length>0?'ch-r':'ch-g'}">
    ${divs.length>0?`⚠ ${divs.length} Divergência(s) Encontrada(s)`:'✅ Nenhuma Divergência — Todos os Saldos Positivos'}
  </div><div class="cb">`;

  if(divs.length>0){
    // Correção
    const opts=divs.map(d=>`<option value="${d.id}|${d.sec}">${d.sec}: ${d.nome} (saldo: ${d.saldo})</option>`).join('');
    h+=`<div class="corr-box">
      <h4>🔧 Campo de Correção — Ajuste em um único campo</h4>
      <div class="corr-row">
        <select id="corr-p"><option value="">— Selecione o produto —</option>${opts}</select>
        <select id="corr-campo">
          <option value="sa">Corrigir Saldo/Sobra Anterior</option>
          <option value="ent">Corrigir Entradas (básicos)</option>
          <option value="said">Corrigir Saídas</option>
        </select>
        <input type="number" id="corr-v" placeholder="Novo valor" step="0.001">
        <button class="btn btn-am" onclick="aplicarCorr()">✔ Aplicar Correção</button>
      </div>
      <p style="font-size:11px;color:#7a5000;margin-top:6px">
        ⚠ Após aplicar, o relatório será atualizado automaticamente.
      </p>
    </div>`;

    h+='<ul class="div-lista">';
    divs.forEach(d=>{
      h+=`<li>
        <div class="esq">
          <span><strong>${escH(d.sec)}</strong> — ${escH(d.nome)}</span>
          <span style="font-size:10px;color:var(--txt3)">
            Saldo Ant.: ${d.sa} | Entradas: ${d.ent} | Saídas: ${d.said}
          </span>
        </div>
        <div class="dir">
          <span class="badge b-av">Saídas: ${d.said}</span>
          <span class="badge b-in">Entradas: ${d.ent}</span>
          <span class="badge b-er">Saldo: ${d.saldo}</span>
        </div>
      </li>`;
    });
    h+='</ul>';
  } else {
    h+='<p style="color:var(--g1);font-weight:600;padding:8px;font-size:13px">Todos os saldos estão positivos ou zerados.</p>';
  }
  h+='</div></div>';

  // Responsáveis
  h+=`<div class="card"><div class="ch ch-b">📝 Responsáveis e Assinaturas</div><div class="cb">
    <div class="resp-grid">
      <div class="rel-item"><h4>Responsável pelas Informações</h4><p style="font-size:14px">${escH(S.info.r1)||'—'}</p></div>
      <div class="rel-item"><h4>Responsável pelo Preenchimento</h4><p style="font-size:14px">${escH(S.info.r2)||'—'}</p></div>
      <div class="rel-item"><h4>Visto da Diretora</h4><p style="font-size:14px">${escH(S.info.r3)||'—'}</p></div>
      <div class="rel-item"><h4>Data</h4><p style="font-size:14px">${S.info.data||'—'}</p></div>
    </div>
  </div></div>`;

  el('rel').innerHTML=h;
  updateHeaderChips();
}

function relTabela(titulo,cls,prods,calcObj,sec,headers,showEmpty){
  if(!prods.length&&!showEmpty){
    return`<div class="card"><div class="ch ${cls}">${titulo} — <span style="font-weight:400;font-size:12px">Nenhum produto com movimento</span></div></div>`;
  }
  let h=`<div class="card"><div class="ch ${cls}">${titulo} (${prods.length} produto(s) com movimento)</div><div class="cb">`;
  h+='<div class="tw"><table><thead><tr>';
  headers.forEach((hd,i)=>h+=`<th${i===0?' style="text-align:left;min-width:180px"':''}>${hd}</th>`);
  h+='</tr></thead><tbody>';
  prods.forEach(p=>{
    const c=calcObj[p.id]||{};
    const nm=nomeP(p,sec);
    const u=(sec==='b'?S.v1b:sec==='c'?S.v1c:S.v2)[p.id]?.u||p.u;
    h+=`<tr>
      <td style="text-align:left">${escH(nm)}</td><td>${u}</td>
      <td>${fmtN(c.sa)}</td><td>${fmtN(c.ent)}</td>
      <td>${fmtN(c.said)}</td>
      <td class="${c.saldo<0?'neg':''}">${fmtN(c.saldo)}</td>
    </tr>`;
  });
  h+='</tbody></table></div></div></div>';
  return h;
}

function aplicarCorr(){
  const ps=el('corr-p').value;
  const campo=el('corr-campo').value;
  const val=parseFloat(el('corr-v').value);
  if(!ps||isNaN(val)){alert('Selecione um produto e informe o valor.');return;}
  const[id,sec]=ps.split('|');
  if(sec==='V1 Básicos'){S.v1b[id][campo]=val}
  else if(sec==='V1 Carnes'){S.v1c[id][campo]=val}
  else if(sec==='V2 Vegetais'){S.v2[id][campo]=val}
  save();buildRel();
  if(telaCurrent==='v1') renderV1();
  if(telaCurrent==='v2') renderV2();
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  EXPORTAR PDF                                                     ║
// ╚═══════════════════════════════════════════════════════════════════╝
function expPDF(){buildRel();window.print();}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  EXPORTAR XLSX — ESPELHO DO ORIGINAL                              ║
// ╚═══════════════════════════════════════════════════════════════════╝
function expXLSX(){
  if(typeof XLSX==='undefined'){alert('Biblioteca XLSX não disponível. Verifique a conexão com a internet.');return;}
  const wb=XLSX.utils.book_new();
  const dias=S.info.dias||23;

  // ── SHEET F1 ──
  (function(){
    const ws={};let maxR=0,maxC=0;
    function sc(r,c,v,t){
      if(v===null||v===undefined||v==='') return;
      ws[XLSX.utils.encode_cell({r,c})]={v,t:t||'s'};
      if(r>maxR)maxR=r;if(c>maxC)maxC=c;
    }
    function sn(r,c,v){sc(r,c,v||0,'n')}

    const prods=V1B;
    // Row 5: title
    sc(5,1,'MAPA DE CMEI');sc(5,2,S.info.cmei||'');
    sc(5,3,'Mês: '+(S.info.mes||'')+' / '+(S.info.ano||''));
    // Row 7: headers
    sc(7,1,'Dias do mês de referência');
    sc(7,2,'Nº de alunos no café');sc(7,3,'Nº de alunos no almoço');
    sc(7,4,'Nº de alunos no lanche');sc(7,5,'Nº de alunos no jantar');
    prods.forEach((p,i)=>sc(7,6+i,nomeP(p,'b')||''));
    // Data rows (row 8 = day 1)
    for(let d=0;d<dias;d++){
      const r=8+d;const dia=S.f1[d]||{};
      sn(r,1,d+1);sn(r,2,+dia.cafe||0);sn(r,3,+dia.almoco||0);
      sn(r,4,+dia.lanche||0);sn(r,5,+dia.jantar||0);
      prods.forEach((p,i)=>{const v=+((dia.c||{})[p.id]||0);if(v)sn(r,6+i,v)});
    }
    // Total row
    const totR=8+dias;
    const tf=f1TotProd(),ta=f1TotAlunos();
    sc(totR,1,'TOTAL');sn(totR,2,ta.cafe);sn(totR,3,ta.almoco);
    sn(totR,4,ta.lanche);sn(totR,5,ta.jantar);
    prods.forEach((p,i)=>{const v=round2(tf[p.id]||0);if(v)sn(totR,6+i,v)});
    ws['!ref']=XLSX.utils.encode_range({s:{r:0,c:0},e:{r:maxR,c:maxC}});
    // Col widths
    const cols=[{wch:6},{wch:8},{wch:10},{wch:10},{wch:10},{wch:10}];
    prods.forEach(()=>cols.push({wch:12}));
    ws['!cols']=cols;
    XLSX.utils.book_append_sheet(wb,ws,'f1');
  })();

  // ── SHEET V1 ──
  (function(){
    const bc=v1bCalc(),cc=v1cCalc();
    const rows=[];
    rows.push(['*MOVIMENTAÇÃO DO ESTOQUE CMEI','unidade','saldo Anterior','entradas','saídas','saldo atual','','']);
    rows.push([]);
    V1B.forEach(p=>{
      const c=bc[p.id]||{};const nm=nomeP(p,'b')||'';const u=S.v1b[p.id]?.u||p.u;
      rows.push([nm,u,c.sa||0,c.ent||0,c.said||0,c.saldo||0,'','']);
    });
    rows.push([]);rows.push(['1','1','1','1','1','1']);
    rows.push(['Perecíveis - Carne','unidade','sobra','entradas','saídas','saldo','','']);
    rows.push(['','','anterior','','','atual','','']);
    V1C.forEach(p=>{
      const c=cc[p.id]||{};const nm=nomeP(p,'c')||'';const u=S.v1c[p.id]?.u||p.u;
      rows.push([nm,u,c.sa||0,c.ent||0,c.said||0,c.saldo||0,'','']);
    });
    const ws=XLSX.utils.aoa_to_sheet(rows);
    ws['!cols']=[{wch:32},{wch:8},{wch:14},{wch:12},{wch:12},{wch:14}];
    XLSX.utils.book_append_sheet(wb,ws,'v1');
  })();

  // ── SHEET F2 ──
  (function(){
    const rows=[];
    rows.push(['DIA DO MÊS','','CARDÁPIO','','','','','']);
    rows.push(['','','Café','','Almoço','','Lanche','','Jantar']);
    for(let d=0;d<dias;d++){
      const f=S.f2[d]||{};
      rows.push([d+1,'',f.cafe||'Segue conforme o cardápio','',f.almoco||'Segue conforme o cardápio','',f.lanche||'Segue conforme o cardápio','',f.jantar||'Segue conforme o cardápio']);
    }
    rows.push([]);
    rows.push(['Responsável pelas informações:',S.info.r1||'']);
    rows.push(['Responsável pelo preenchimento:',S.info.r2||'']);
    rows.push(['Visto da diretora:',S.info.r3||'']);
    rows.push(['DATA:',S.info.data||'']);
    const ws=XLSX.utils.aoa_to_sheet(rows);
    ws['!cols']=[{wch:14},{wch:4},{wch:30},{wch:4},{wch:30},{wch:4},{wch:30},{wch:4},{wch:30}];
    XLSX.utils.book_append_sheet(wb,ws,'f2');
  })();

  // ── SHEET V2 ──
  (function(){
    const vc=v2Calc();
    const rows=[];
    rows.push(['MOVIMENTAÇÃO DO ESTOQUE                                                                   CMEI','unidade','Sobra Anterior','entradas','saídas','saldo atual']);
    rows.push(['perecíveis - vegetais']);
    V2V.forEach(p=>{
      const c=vc[p.id]||{};const nm=nomeP(p,'v')||'';const u=S.v2[p.id]?.u||p.u;
      rows.push([nm,u,c.sa||0,c.ent||0,c.said||0,c.saldo||0]);
    });
    rows.push([]);rows.push(['OBSERVAÇÕES:']);rows.push([]);
    rows.push(['Responsável pelas informações: '+S.info.r1||'fulana de Tal - Merendeira']);rows.push([]);
    rows.push(['Responsável pelo preenchimento: '+S.info.r2||'Fulano de Tal - Secretário']);rows.push([]);
    rows.push(['Visto da diretora: '+(S.info.r3||'Ciclana de Tal - Diretora')]);rows.push([]);
    rows.push(['DATA:',(S.info.data||'')]);
    const ws=XLSX.utils.aoa_to_sheet(rows);
    ws['!cols']=[{wch:32},{wch:8},{wch:14},{wch:12},{wch:12},{wch:14}];
    XLSX.utils.book_append_sheet(wb,ws,'v2');
  })();

  // ── SHEET CÁLCULO DE NOTAS ──
  (function(){
    const ct=calcTot();
    const hdr=['PRODUTO'];
    for(let i=1;i<=50;i++) hdr.push(`N${i}`);
    hdr.push('TOTAIS');
    const rows=[hdr];
    CALC_ALL.forEach(p=>{
      const nm=V2V.includes(p)?nomeP(p,'v'):nomeP(p,'c');
      const row=[nm||''];
      for(let i=1;i<=50;i++) row.push(+(S.calc[p.id]?.[`N${i}`]||0)||null);
      row.push(ct[p.id]||0);
      rows.push(row);
    });
    const ws=XLSX.utils.aoa_to_sheet(rows);
    const cols=[{wch:30}];
    for(let i=0;i<51;i++) cols.push({wch:8});
    ws['!cols']=cols;
    XLSX.utils.book_append_sheet(wb,ws,'Cálculo de notas');
  })();

  const fn=`MAPA_CMEI_${(S.info.cmei||'CMEI').replace(/\s+/g,'_')}_${S.info.mes||''}${S.info.ano||''}.xlsx`;
  XLSX.writeFile(wb,fn);
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  HELPERS                                                          ║
// ╚═══════════════════════════════════════════════════════════════════╝
function el(id){return document.getElementById(id)}
function escH(s){if(!s) return '';return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;')}
function fmtN(v){const n=+(v||0);return n===0?'0':String(n)}

function nomeP(p,sec){
  if(sec==='b') return (S.v1b[p.id]?.nome!==undefined&&S.v1b[p.id].nome!==null?S.v1b[p.id].nome:null)||p.n||'';
  if(sec==='c') return (S.v1c[p.id]?.nome!==undefined&&S.v1c[p.id].nome!==null?S.v1c[p.id].nome:null)||p.n||'';
  return (S.v2[p.id]?.nome!==undefined&&S.v2[p.id].nome!==null?S.v2[p.id].nome:null)||p.n||'';
}

function hasDados(tab){
  if(tab==='f1') return S.f1.some(d=>d&&(d.cafe||d.almoco||d.lanche||d.jantar||Object.values(d.c||{}).some(v=>v>0)));
  if(tab==='v1') return V1B.some(p=>S.v1b[p.id]&&(S.v1b[p.id].sa||S.v1b[p.id].ent));
  if(tab==='f2') return S.f2.some(d=>d&&(d.cafe&&d.cafe!=='Segue conforme o cardápio'));
  if(tab==='v2') return V2V.some(p=>S.v2[p.id]&&(S.v2[p.id].sa||S.v2[p.id].said));
  if(tab==='calc') return CALC_ALL.some(p=>Object.values(S.calc[p.id]||{}).some(v=>v>0));
  return false;
}

function dotOn(tab,on){
  const d=el('dot-'+tab);
  if(d) d.classList.toggle('on',on);
}

function resetAll(){
  if(!confirm('⚠ ATENÇÃO: Apagará TODOS os dados inseridos. Confirma?'))return;
  if(!confirm('Última confirmação — operação irreversível!'))return;
  localStorage.removeItem('cmei_s');
  initS();loadInfoForm();
  goto('info');alert('Dados resetados.');
}

// ╔═══════════════════════════════════════════════════════════════════╗
// ║  INIT                                                             ║
// ╚═══════════════════════════════════════════════════════════════════╝
initS();
load();
loadInfoForm();
updateHeaderChips();
// Pre-render all tabs so they're ready
renderF1();renderV1();renderF2();renderV2();
renderCalc();
buildRel();
</script>
</body>
</html>

