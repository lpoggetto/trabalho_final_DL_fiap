# trabalho_final_DL_fiap

A ideia é desenvolver um modelo que tenha como output a compra ou venda de um determinada ação baseado na movimentaçãodo mercado nos últimos 15 dias.

Inicialmente 4 ações foram selecionadas para análise:
* VALE3 – Vale do Rio Doce;
* PETR4 – Petrobras;
* BBAS3 – Banco do Brasil;
* CSNA3 - Companhia Siderúrgica Nacional.

Foco no modelo - "Perseguidor de tendência".

Obs: Suavização aplicada (método não informado).

### Dicionário dos dados:

* Date - Dia da operação (Compra/Venda);
* Close - Valor do preço da ação no fim do dia;
* Smoothed Close - Preço filtrado no fim do dia (Apenas critério de curiosidade);
* Label - (-1) = Venda / (+1) = Compra para ser operado naquele dia (antes do fechamento);
* Past_XYZ_Days_Close - Valor do preço das ações na faixa de dias descrita (D-1 à D-15).

### Testar o uso de:
* Redes neurais convolucionais 1D (CNN 1D);
* Redes neurais recorrentes (RNN).

link com os materiais: https://drive.google.com/drive/folders/1OTU650tmFmeyARV5-lYW7yNacVWPxvOJ?usp=sharing

### Entrega:

A solução implementada utilizando modelos de Deep Learning com Tensorflow para as 4 ações e outras soluções diferenciadas e inovadores (opcional) que possam ser aplicadas ao conjunto de dados proposto.
1 - Devem ser entregues em formato de Jupyter Notebook;

As quatro ações devem ter modelos treinados, e devem ser apresentados os seguintes indicadores:
* Acurácia no conjunto de teste de cada modelo;
* Matriz de confusão, precision e recall de cada modelo;
* Desempenho financeiro do modelo via ‘backtest’ com o objetivo de responder se o modelo gerado daria retorno financeiro (opcional pois é um assunto de finanças, se não fizer não há prejuízo na nota final);
