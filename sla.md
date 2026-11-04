INTERACTIVE DECK BUILDER CATALOG: O DUELO TÁTICO DE CARTAS (VERSÃO AVANÇADA)
1. CABEÇALHO DO PAINEL INTERATIVO (HUD DE MONTAGEM & ENGENHARIA DE DECK)
Título da Interface: CATÁLOGO MESTRE & DECK BUILDER TÁTICO

Subtítulo / Descrição Operacional: O laboratório definitivo de engenharia de baralhos. Explore o catálogo global de cartas, filtre por raças, arquétipos e custos de Mana, monte sua estratégia 1v1 em tempo real e importe/exporte instantaneamente via arquivos CSV estruturados para o motor de combate.

Ações Globais de Controle (Toolbar Superior):

[ NOVO DECK ] | [ SALVAR ALTERAÇÕES ] | [ 📂 IMPORTAR CSV ] | [ 💾 EXPORTAR CSV ] | [ 🔄 TESTAR MÃO INICIAL ] | [ 🗑️ LIMPAR BARALHO ]

2. LAYOUT DO PAINEL PRINCIPAL (DASHBOARD EM 3 COLUNAS EXPANDIDAS)
Coluna Esquerda: Catálogo Mestre, Filtros Avançados e Busca
Barra de Pesquisa Global Inteligente: Busca em tempo real por ID, Nome parcial, Efeitos descritivos ou trechos do texto de flavor/lore.

Filtros por Tipo de Carta (TipoCarta):

[ TODOS ] | [ MONSTER (Unidades) ] | [ SPELL (Magias) ] | [ TRAP (Armadilhas) ]

Filtros Avançados por Subtipo / Raça (SubCarta):

Seletor multicategorias dividido por facções/raças (Dragões, Guerreiros, Magos, Máquinas, Zumbis, Fadas, Demônios, Plantas, etc.), permitindo selecionar múltiplos subtipos simultaneamente para decks temáticos.

Filtros por Atributos de Combate e Recursos:

Custo de Mana (cost): Slider ou botões de seleção rápida (0 a 5+).

Atributo de Ataque (atk): Filtro por faixa de poder ofensivo.

Atributo de Vida (hp): Filtro por faixa de resistência defensiva.

Grid Dinâmico de Exibição do Catálogo (Cards Interativos):

Renderização visual simulando os campos da struct Carta (Miniatura de Textura, Nome, Custo de Mana no canto superior, ATK/HP nos cantos inferiores, e ícones indicativos de Tipo e Subtipo).

Interação de Clique: Clique simples exibe o card em alta resolução com o texto de efeito detalhado; duplo clique ou botão [ + ADICIONAR ] insere o card no deck ativo.

Coluna Central: O Deck Ativo e Gerenciamento de Cópia
Cabeçalho de Métricas do Deck:

Contador Numérico Estrito: X / 30 Cartas (Barra de progresso visual que muda de cor: vermelho se incompleto, verde ao atingir exatamente o teto de 30).

Contador de Tipos: Proporção em tempo real de Monstros vs. Magias vs. Armadilhas presentes no baralho.

Listagem Dinâmica do Deck Atual:

Organização estruturada em ordem de Custo de Mana ou por Tipo.

Cada linha exibe o ID, Nome, Tipo, Custo e o número de cópias incluídas.

Botões de Gestão Rápida por Linha: [ + ] (adicionar cópia extra, respeitando o limite máximo por carta) e [ - ] (remover cópia ou unidade da lista).

Painel de Validação e Avisos Críticos em Tempo Real:

Alertas instantâneos para inconsistências estruturais (ex: "Aviso: Deck abaixo do limite de 30 cartas", "Erro: O arquivo CSV importado possui IDs inválidos ou inexistentes no catálogo").

Coluna Direita: Análise Tática, Sinergia e Simulador de Mão Inicial
Histograma de Curva de Mana:

Gráfico de barras interativo exibindo a distribuição de custos de Mana (de 1 a 5+), permitindo ao duelista avaliar se o deck tem cartas suficientes para o Início de Turno (custo 1 e 2) sem sobrecarregar as rodadas finais.

Radar de Sinergia e Modificadores:

Indicadores de presença de cartas compatíveis com táticas de Shield (blindagem) e Charge (multiplicador de ataque), além da contagem de Armadilhas na zona dedicada.

Ferramenta de Simulação de Mão Inicial (Test Draw):

Botão [ 🎲 SIMULAR MÃO (4 CARTAS) ] que simula instantaneamente o puxão inicial do Jogador, exibindo quais cartas viriam na mão para testar a viabilidade do primeiro turno e evitar mãos travadas.

Painel de Importação e Exportação CSV Dedicado:

Área de Upload CSV: Caixa de arrastar e soltar (drag & drop) ou botão de seleção de arquivo para carregar planilhas contendo os dados do deck (mapeados diretamente para a struct do jogo).

Botão de Exportação CSV: Gera e baixa instantaneamente um arquivo .csv perfeitamente formatado para leitura direta pelo motor em C/Raylib da arena de combate.

3. FEEDBACK VISUAL, UX E INTERAÇÕES AVANÇADAS
Tooltips Flutuantes Detalhados: Ao passar o cursor do mouse sobre qualquer carta (no catálogo ou no deck), surge um painel lateral ampliado exibindo todas as propriedades lógicas da struct (id, hp, atk, cost, tipo, subTipo, nome) e uma descrição expandida do efeito.

Feedback de Importação de CSV (Relatório de Status): Após carregar um arquivo .csv, o sistema exibe um modal de resumo detalhando:

Número de cartas lidas com sucesso.

Alertas para linhas duplicadas ou cartas com custos incompatíveis.

Confirmação de integridade estrutural pronta para o duelo.

Estados Visuais de Bloqueio (Greyscale & Disabled): Cartas que atingem o limite máximo de cópias no deck ou que violam regras de restrição do sistema recebem uma sobreposição esmaecida com o distintivo visual de bloqueio.
