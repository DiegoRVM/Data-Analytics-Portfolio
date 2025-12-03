# 📱 Análise de Comportamento e Teste A/A/B em App de Delivery

## 📌 Contexto do Projeto
Trabalho em uma startup de produtos alimentícios e a equipe de design propôs alterar as fontes de todo o aplicativo. A gerência, preocupada que o novo design pudesse ser "intimidador" e afetar as vendas, solicitou uma análise baseada em dados.

**Objetivo:** Analisar o funil de vendas atual e avaliar os resultados de um Teste A/A/B para decidir se a nova fonte deve ser implementada.

## 📂 Estrutura dos Dados
O dataset contém logs de eventos de usuários com as seguintes colunas:
* `EventName`: Tipo de ação (ex: visualizar tela principal, adicionar ao carrinho).
* `DeviceIDHash`: Identificador único do usuário.
* `EventTimestamp`: Data e hora do evento.
* `ExpId`: Grupo do experimento (246/247 = Controle, 248 = Teste).

## 📊 Metodologia
1.  **Pré-processamento:** Limpeza de dados, ajuste de tipos e filtragem de logs antigos (dados anteriores a 01/08/2019 foram descartados por incompletude).
2.  **Análise do Funil:** Mapeamento da jornada do usuário para identificar gargalos de conversão.
3.  **Teste A/A:** Validação da estabilidade entre os dois grupos de controle (246 e 247).
4.  **Teste A/B:** Comparação do grupo de teste (248 - Fontes Novas) contra os grupos de controle combinados e isolados.
5.  **Estatística:** Utilizado o **Teste Z para igualdade de proporções** com correção de Bonferroni para múltiplos testes.

## 🔍 Principais Resultados

### 1. Funil de Vendas
* Apenas **47.7%** dos usuários que abrem o app completam uma compra.
* A maior perda de usuários (**~38%**) ocorre logo no início, entre a `Tela Principal` e a `Tela de Ofertas`.

### 2. Resultado do Teste A/A/B
Realizamos 12 testes de hipóteses comparando as taxas de conversão em cada etapa do funil entre os grupos.

* **Controle vs Controle (A/A):** Não houve diferença estatisticamente significativa, validando a precisão do sistema de split.
* **Teste vs Controle (A/B):** Não houve diferença estatisticamente significativa em nenhuma das etapas do funil entre o grupo com novas fontes e os grupos de controle.

## 💡 Conclusão e Recomendação
A alteração das fontes **não afetou o comportamento de compra** dos usuários, nem positiva nem negativamente. O receio de que o design seria "intimidador" não se confirmou nos dados.

✅ **Recomendação:** A equipe de design pode prosseguir com a atualização das fontes, pois isso não trará prejuízos financeiros à conversão.

---
## 🛠️ Tecnologias
* Python (Pandas, Matplotlib, Seaborn, SciPy)
* Jupyter Notebook
* Estatística Inferencial

---
*Projeto desenvolvido por Diego Raniel Vaz Mendes.*
