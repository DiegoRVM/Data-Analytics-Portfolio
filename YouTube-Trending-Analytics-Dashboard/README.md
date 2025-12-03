# 📺 YouTube Trending Analytics Dashboard

## 📌 Contexto do Projeto (Sterling & Draper)
Como analista de dados na agência de publicidade **Sterling & Draper**, fui encarregado de automatizar a análise de vídeos "Em Alta" (Trending) no YouTube.

O objetivo era criar uma ferramenta para os gerentes de planejamento de mídia (Melanie e Ashok) identificarem rapidamente qual tipo de conteúdo merece atenção de marketing, substituindo processos manuais por um **Dashboard Automatizado**.

## 🔗 Links do Projeto
* 📊 **Acesse o Dashboard Interativo (Tableau Public):** [Clique aqui para ver o Dashboard](https://public.tableau.com/views/AnlisedeTendnciasdoYouTubeHistricoeDistribuioRegional/Painel1)
* 📑 **Apresentação de Resultados (Google Slides):** [Ver Slides](https://docs.google.com/presentation/d/1XPldhHEWaKYU3uqiBKWQ6dYWqmZUDoTlyD7UMoLOkoM/edit?usp=sharing)

## ❓ Problemas de Negócio Resolvidos
O dashboard foi desenhado para responder, em tempo real, às seguintes perguntas recorrentes da diretoria:
1.  Quais categorias de vídeo ficam em alta com mais frequência?
2.  Como os vídeos populares estão distribuídos geograficamente?
3.  Existe alguma diferença de preferência de conteúdo nos Estados Unidos em relação ao resto do mundo?

## 🛠️ Ferramentas e Dados
* **Ferramenta de BI:** Tableau Public
* **Fonte de Dados:** Tabela agregada `trending_by_time` (CSV) contendo dados históricos de vídeos em alta, categorias e regiões.
* **Modelagem:** Relacionamento entre tabelas de fatos (vídeos) e dimensões (categorias e países).

## 💡 Principais Insights (Descobertas)
[cite_start]Com base na análise dos dados históricos, identificamos:

### 1. O Domínio do Entretenimento
As categorias **Entretenimento** e **Música** são, de longe, as mais dominantes, representando juntas cerca de **50% de todo o volume** de vídeos em alta. Para campanhas de massa, este é o canal ideal.

### 2. O Poder da Notícia e Política
A categoria **"News & Politics"** apresentou um volume surpreendente, competindo diretamente com categorias de lazer. Isso indica uma oportunidade para marcas que desejam se posicionar em tópicos atuais e discussões sociais.

### 3. Distribuição Regional
Os **Estados Unidos** lideram o volume de vídeos em tendência (23.7%), seguidos por Índia e Reino Unido. A estratégia de marketing deve priorizar criativos em inglês, mas considerar a localização cultural para o mercado indiano.

## 📂 Estrutura do Repositório
* `data/`: Contém o dataset bruto utilizado (`trending_by_time.csv`).
* `tableau_files/`: Arquivo de trabalho do Tableau (`.twb`) para quem quiser ver a construção técnica.
* `reports/`: Relatório executivo em PDF com a análise estática.

---
*Projeto desenvolvido por Diego Raniel Vaz Mendes durante o Bootcamp de Análise de Dados.*
