#Vinicola Data Exploration 🍷

Exploração de dados de produção, exportação e importação de vinhos e derivados no Brasil, com foco na compreensão de padrões, fatores externos e qualidade do produto.

📋 Sumário
Sobre o Projeto

Motivação

Dados

Metodologia

Instalação & Execução

Resultados & Insights

Conclusões

Próximos Passos

Autor

🧠 Sobre o Projeto
Este notebook analisa dados da cadeia produtiva de vinhos no Brasil, incluindo produção, exportação, importação e variáveis influentes (clima, economia, avaliações). A finalidade é gerar insights estratégicos para stakeholders do setor.

🎯 Motivação
Compreender os fluxos comerciais de vinho (origem/destino, volume, receita)

Identificar padrões sazonais, geográficos e econômicos

Avaliar influências externas como clima regional e tendências de avaliação de vinhos

Preparar dashboards e relatórios para suportar decisões em reuniões com investidores e acionistas

🗄️ Dados
Produção, exportação e importação: origem, destino, volume (L), valor (US$)

Clima: variáveis como temperatura e pluviosidade nas regiões produtoras

Econômicas e demográficas: PIB, população, renda per capita

Avaliações de vinho: notas de qualidade em bases públicas

Fontes: Embrapa (CNPUV) e APIs públicas de clima, economia e avaliações.

🧪 Metodologia
Importação e limpeza dos dados com pandas

Análise exploratória: estatísticas descritivas, identificação de valores ausentes e outliers

Visualizações: histogramas, séries temporais, mapas, boxplots e scatterplots

Correlação multivariada: uso de seaborn.pairplot e matrizes de correlação

Segmentação de mercados via clusters (ex: K-means)

Agrupamentos por geografia, tipo de produto e faixa de preço

⚙️ Instalação & Execução
Requisitos: Python 3.8+

bash
Copiar
Editar
git clone https://github.com/PedroSilva0z/Vinicola_data_exploration.git
cd Vinicola_data_exploration
pip install -r requirements.txt
jupyter notebook Vinicola_data_exploration.ipynb
Ou abra o Colab diretamente via link.

📊 Resultados & Insights
Tabelas resumo: volume e receita por país origem/destino

Sazonalidade: picos de exportação alinhados a eventos climáticos

Correlação: forte relação entre temperatura média e volume exportado

Segmentação: clusters identificam mercados emergentes vs consolidados

Avaliações: vinhos com maior preço tendem a ter notas superiores

(Detalhe visualizações e sumarização dos gráficos mais relevantes)

🧾 Conclusões
O volume exportado cresce em clima mais frio

Mercados emergentes (Ásia) estão crescendo, embora ainda com preços menores

Existem oportunidades de elevar margem através de vinhos premium altamente avaliados

🔭 Próximos Passos
Aplicar técnicas de forecasting (ex.: ARIMA, Prophet) para volume e receita

Desenvolver modelos preditivos de nota de qualidade

Construir dashboard interativo com Plotly Dash ou Power BI

Ampliar com dados de marketing, sazonalidade global e comportamento do consumidor

🧑‍🎓 Autor
Pedro Silveira – Analista de Dados em transição para Cientista de Dados

📌 LinkedIn: silveirapedrosil
📍 Área: São Paulo, Brasil

🤝 Contribuições
Contribuições são bem-vindas! Consulte o arquivo CONTRIBUTING.md para orientações ou abra uma issue.

📄 Licença
Este projeto está sob a licença MIT – veja o arquivo LICENSE para mais detalhes.
