Análise de Evasão de Clientes (Churn) na TelecomX
Descrição do Projeto
Este projeto realiza uma análise exploratória dos dados de clientes da TelecomX com o objetivo de identificar os principais fatores que levam à evasão de clientes (churn). Compreender esses fatores é essencial para a empresa desenvolver estratégias eficazes de retenção e melhorar a satisfação do cliente.

Fonte de Dados
Os dados utilizados nesta análise foram obtidos a partir de um arquivo JSON fornecido para este desafio.

Etapas da Análise
A análise seguiu as seguintes etapas principais:

Extração e Carregamento: Carregamento dos dados a partir da API fornecida e transformação em um DataFrame pandas.
Exploração Inicial: Análise das informações básicas do DataFrame, tipos de dados e verificação de valores nulos.
Transformação e Limpeza:
Renomeação das colunas para português.
Substituição de valores categóricos ('Yes', 'No', 'No phone service', 'No internet service') por valores numéricos (1 e 0).
Tratamento de inconsistências e valores nulos nas colunas 'evazao' e 'gasto_total'.
Verificação de consistência entre serviços de telefone/internet e serviços agregados.
Análise Exploratória de Dados:
Análise da distribuição geral da variável target (Evasão).
Exploração da relação entre a evasão e variáveis categóricas (gênero, parceiro, dependentes, idoso, tipo de contrato, método de pagamento, serviço de internet e serviços agregados).
Análise da relação entre a evasão e variáveis numéricas (meses de contrato, total mensal, gasto total), incluindo agrupamento por trimestres de meses de contrato.
Cálculo da matriz de correlação entre variáveis selecionadas, incluindo serviços de internet e evasão (considerando apenas clientes com serviço de internet).
Visualização de Dados: Criação de gráficos (histogramas, box plots, countplots) para visualizar a distribuição das variáveis e sua relação com a evasão.
Principais Descobertas
A análise exploratória revelou os seguintes insights importantes sobre a evasão de clientes na TelecomX:

A taxa geral de evasão na base de dados analisada é de aproximadamente 26.6%.
Clientes com contratos "Month-to-month" apresentam uma taxa de evasão significativamente maior.
O método de pagamento "Electronic check" está fortemente associado à evasão.
Clientes com serviço de internet "Fiber optic" têm uma alta taxa de evasão.
A evasão é mais alta nos primeiros meses de contrato, diminuindo com o tempo de permanência do cliente.
Clientes com contas mensais mais altas tendem a ter uma maior taxa de evasão.
A análise de correlação e visualizações sugerem que alguns serviços agregados de internet (como backup, proteção de dispositivo, streaming de TV e filmes) têm uma relação com a evasão, embora a direção e força da correlação variem.
Recomendações
Com base nestas descobertas, as seguintes ações são recomendadas para a TelecomX:

Implementar programas de integração e suporte aprimorado para novos clientes nos primeiros meses.
Oferecer incentivos para que os clientes optem por contratos de maior duração (um ou dois anos).
Investigar possíveis problemas ou atritos associados ao método de pagamento "Electronic check".
Analisar a experiência do cliente com o serviço de "Fibra óptica" para identificar causas de insatisfação.
Desenvolver estratégias de retenção direcionadas a clientes com contas mensais mais altas.
Este relatório e a análise realizada fornecem uma base sólida para a TelecomX desenvolver e implementar estratégias direcionadas para reduzir a evasão de clientes e melhorar a retenção.
