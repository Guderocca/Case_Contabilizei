🚀 Case Contabilizei: Business Intelligence & Data EngineeringEste repositório contém a solução técnica para o case de planejamento estratégico da Contabilizei. 

O projeto foca na transformação de dados brutos de mercado e performance interna em insights acionáveis, utilizando SQL para o processamento lógico e Excel para modelagem estatística.

🛠️ Stack TécnicaDatabase: Oracle Database (via SQL Developer).
Data Analysis: Microsoft Excel .
Versionamento: Git/GitHub para documentação de scripts .

sql.📐 Arquitetura da Solução
A análise foi dividida em três camadas para garantir a escalabilidade e a verificação cruzada (cross-check) dos resultados:

Ingestão: Importação de arquivos flat (.xlsx) para tabelas relacionais via assistente do SQL Developer, garantindo a tipagem correta de dados (DATE, NUMBER, FLOAT).
Processamento (SQL): Implementação de queries complexas para evitar erros manuais de células, utilizando Window Functions (LAG) para cálculos de série temporal.

Visualização (Excel): 

Criação de dashboards de funil de vendas para facilitar a interpretação gerencial.


Validação de Market Share e Projeção


A projeção de investimento (Exercício 5) foi parametrizada para refletir o cenário de Abril/2022, utilizando o CAC real como variável multiplicadora sobre a meta de 6% do Market Share:Query de Projeção: (MERCADO_TOTAL * 0.06) * (INVESTIMENTO / VENDAS).

📈 Insights Técnicos ExtraídosDesvio de CAC: Identificado um aumento de 217% no CAC em 13 meses ($R\$ 114,34 \rightarrow R\$ 362,51$), sinalizando uma possível saturação de canais ou necessidade de otimização de lances.

Eficiência de Funil: A conversão de Lead para Venda apresentou queda de 22,9%, sugerindo um gargalo no processo de qualificação ou fechamento comercial.

Elasticidade de Atração: O investimento cresceu 144,44%, enquanto o volume de leads cresceu apenas 59%, evidenciando um aumento no Custo por Lead (CPL).

🚀 Como ReplicarImporte o arquivo Case_contabilizei.xlsx para o seu ambiente SQL.

Execute o script case_contabilizei.sql para gerar as tabelas de variação e KPIs.
Compare os resultados com as abas de "pergunta 1 a 5" no Excel para validação final .

Gustavo Della  Estudante de Engenharia de Computação - FIAPInfraestrutura & Data Analysis
