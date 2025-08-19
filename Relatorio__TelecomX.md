
# Relatório de Churn – TelecomX

## Contexto

Este documento apresenta uma avaliação detalhada sobre o cancelamento de clientes (churn) na TelecomX. O objetivo central é identificar fatores que aumentam a chance de evasão e sugerir caminhos práticos para retenção. A análise utilizou dados relacionados ao perfil do cliente, seus contratos, serviços contratados e aspectos financeiros.

## Preparação e Tratamento da Base

Os dados brutos passaram por uma etapa inicial de limpeza e padronização. Foram ajustados registros com informações faltantes, em especial na coluna `ChargesTotal`, que teve valores corrigidos com base na multiplicação entre `tenure` e `ChargesMonthly` nos casos de clientes recém-ingressos. Essa coluna foi convertida para tipo numérico, permitindo análises estatísticas consistentes. Nenhum caso duplicado foi encontrado, garantindo a integridade da amostra.

## Resultados da Análise

A taxa de churn geral é de **25,72%**. A seguir, os principais achados organizados por dimensão de análise:

### Perfil do Cliente

* **Gênero e Idade:** A evasão ocorre em proporção semelhante entre homens e mulheres. Clientes mais jovens (não seniores) são maioria entre os que cancelam, mostrando que a idade por si só não explica a decisão de saída.
* **Dependentes:** Usuários sem dependentes têm maior probabilidade de cancelar, o que indica menor vínculo ou compromisso com a continuidade do serviço.

### Tempo de Relacionamento (Tenure)

* O risco de cancelamento é mais elevado nos **primeiros dois anos**, especialmente nos quatro meses iniciais (responsáveis por **9,36% do churn**).
* Após os 36 meses, há um novo aumento de desligamentos, sugerindo um ciclo de vida do cliente com pontos críticos de atenção.

### Modalidade de Contrato

* O contrato de **“Month-to-month”** responde por **88,5% do churn** e é o principal fator de risco.
* Contratos de 1 e 2 anos têm taxas de churn muito menores, o que reforça a importância de vínculos de longo prazo.

### Serviços Adquiridos

* **Telefonia:** A maioria dos cancelamentos envolve clientes que utilizam serviço de telefonia (92%).
* **Internet:** Entre os usuários de internet, clientes de **fibra óptica** concentram os maiores índices de churn (17,85% do total), representando quase 70% dos cancelamentos nesse serviço.

### Forma de Pagamento

* O **“Electronic check”** é o método mais associado à evasão, concentrando 57% dos cancelamentos (14,72% do total). Isso sugere falhas ou insatisfação no processo de cobrança por esse canal.

### Cobranças Mensais e Totais

* Clientes que saem possuem, em média, **cobranças mensais cerca de 13 dólares maiores** do que os clientes retidos.
* Essa diferença persiste ao longo do tempo, reforçando que preços mais altos aumentam a propensão ao churn.

## Síntese e Recomendações

Os fatores mais relevantes identificados para explicar o churn são:

* Predomínio do contrato **mensal (Month-to-month)**, muito flexível.
* Maior vulnerabilidade nos **primeiros meses de relacionamento**.
* Alta taxa de cancelamento entre clientes de **fibra óptica**.
* Experiência problemática com o método de pagamento **Electronic check**.
* **Cobranças mensais elevadas** associadas à insatisfação.

**Sugestões de ação:**

1. **Onboarding estruturado:** Investir em suporte ativo nos primeiros 6–12 meses, especialmente para clientes em contratos mensais.
2. **Revisão da fibra óptica:** Pesquisar junto a clientes os motivos de insatisfação (qualidade, atendimento, expectativa vs. entrega).
3. **Aprimorar cobrança via Electronic check:** Revisar a jornada desse método e oferecer alternativas mais amigáveis.
4. **Gestão de clientes de alto valor:** Criar ofertas e benefícios diferenciados para usuários com maior gasto mensal.
5. **Incentivo à fidelização:** Ampliar vantagens para quem adere a contratos de 1 ou 2 anos, reduzindo a facilidade de saída imediata.
