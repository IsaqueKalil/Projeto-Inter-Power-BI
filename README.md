#  Retrospectiva S.C. Internacional no Brasileirão (2003 – 2025) | Power BI


Este repositório contém o projeto analítico desenvolvido no **Power BI** referente ao desempenho histórico do **Sport Club Internacional** no Campeonato Brasileiro, cobrindo toda a era dos pontos corridos (2003 até 2025 finalizado).

---

##  Visão Geral do Projeto

O objetivo do projeto foi transformar mais de duas décadas de estatísticas esportivas num dashboard interativo, dinâmico e de alta performance, permitindo analisar tanto o rendimento coletivo da equipe quanto as estatísticas individuais dos atletas.

### 📊 Funcionalidades e Painéis:
- **Visão Geral Coletiva:** Jogos, Vitórias, Empates, Derrotas, APROVEITAMENTO e Pontos ao longo dos anos.
- **Mando de Campo:** Desempenho detalhado em jogos como Mandante vs. Visitante.
- **Histórico por Técnico:** Desempenho e número de jogos sob o comando de cada treinador.
- **Desempenho Individual:** Análise de jogadores, cartões, minutos jogados e participação direta em gols.

---

##  Desenvolvimento & Desafios Técnicos

### 1. Fonte de Dados, ETL e Imagens
- **Fonte de Dados:** Dados extraídos e estruturados a partir do **Transfermarkt**, a principal referência global em estatísticas de futebol.
- **Power Query:** Limpeza, padronização de datas, nomes de adversários e cálculo de partidas por mando de campo.
- **Mídia Dinâmica:** Mapeamento de URLs para exibição das fotos dos jogadores nos visuais. Devido a limitações de bases históricas antigas, cerca de 80% dos atletas contam com fotos tratadas e integradas.
- **Modelagem de Dados:** Estrutura em **Star Schema** (Tabelas Fato e Dimensão), otimizando relacionamentos e performance de filtragem.

### 2. Lógicas DAX Destacadas
- **Tratamento de Nulos:** Utilização da função `COALESCE` para garantir que visuais e cartões exibam `0` em vez de valores em branco em cenários sem registros.
- **Métricas Condicionais:** Regras personalizadas para o cálculo de *Minutos por Participação em Gol*, aplicando filtros específicos por posição (como a exclusão de goleiros em métricas ofensivas).

### 3. Design & UX
- Layout customizado com paleta de cores institucional do clube.
- Otimização do canvas para apresentação em tela cheia e navegação por filtros dinâmicos (Ano, Posição, Técnico e Adversário).

---

##  Como Visualizar

1. Faça o download do arquivo `.pbix` localizado neste repositório.
2. Abra o arquivo no **Power BI Desktop**.
3. *(Opcional)* Se possuir o vídeo/GIF demonstrativo, insira o link aqui.

---

💬 *Feedbacks, sugestões e contribuições são muito bem-vindos!*
