# Vinicola Data Exploration 🍷

Exploração de dados sobre a produção, exportação e importação de vinhos e derivados no Brasil. Este projeto busca identificar padrões, entender influências externas (como clima e economia) e apoiar decisões estratégicas no setor vinícola.

---

## 📋 Sumário

- [Contexto & Objetivo](#-contexto--objetivo)  
- [Fontes de Dados](#-fontes-de-dados)  
- [Pipeline & Metodologia](#-pipeline--metodologia)  
- [Limpeza & Pré‑processamento](#-limpeza--pré‑processamento)  
- [Análise Exploratória](#-análise-exploratória)  
- [Visualizações](#-visualizações)  
- [Insights e Conclusões](#-insights-e-conclusões)
- [Instalação & Execução](#-instalação-&-execução)
- [Autor](#-autor)

---

## 🧠 Contexto & Objetivo

Você foi responsável por analisar os relatórios iniciais do volume e valor da exportação/importação de vinhos para reunião com investidores e diretores. Além do comércio, foram considerados fatores externos como clima, indicadores econômicos e avaliações de vinhos com notas de juízes. O objetivo: entender padrões e direcionar estratégias.

---

## 🗄️ Fontes de Dados

1. **Produção e comércio**: dados da CNPUV/Embrapa (vinhos e derivados exportados/importados pelo Brasil).  
2. **Climáticos**: temperatura média e pluviosidade por região produtora.  
3. **Socioeconômicos**: PIB, renda per capita e população (APIs públicas).  
4. **Avaliações de vinho**: notas atribuídas por juízes.  
5. **Outros atributos**: ano de safra, tipo de uva, cor, faixa de preço.

---

## 🧭 Pipeline & Metodologia

1. Leitura dos dados com `pandas`.  
2. Identificação de valores ausentes ou inconsistentes (e.g., valores `-1`).  
3. Limpeza de dados: remoção de registros com preço, ano ou nota inválidos e outliers (ex: preço > 2000).  
4. Conversão de tipos: notas, preços e ano para numéricos; categóricos para cor/região.  
5. Análise estatística: contagem, distribuição e identificação de padrões.  
6. Visualizações: gráficos de frequência, distribuições, pairplot, heatmap de correlações e gráficos por tipo de uva/região/produtor.  
7. Extração de insights para guiar decisões (comércio, produção e marketing).

---

## 🧹 Limpeza & Pré‑processamento

- Valores `-1` em **preço mínimo, preço máximo, ano e nota** foram removidos.  
- Preços acima de **2000** foram considerados outliers e descartados.  
- Conversão de colunas para tipos adequados (`float`, `category`, ou `object`).  
- Extração de colunas de tipo de uva (Castes), separadas por vírgulas para análise individual.
  
---

## 🔍 Análise Exploratória

- **Faixa de preços**: identificação das faixas mais comuns (ex: 4, 7.5, 10, 12.5, 15).  
- **Ano de safra**: maioria das safras entre 2004–2013; safra “-1” foi descartada.  
- **Notas dos juízes**: maioria entre 15–17 (escala de 0–20); valores extremos e “-1” foram removidos.  
- **Correlação**: preço e teor alcoólico têm impacto significativo na nota; safra tem menor correlação.

---

## 📊 Visualizações  

- **Distribuição de notas** (“JudgeRating”): valores concentrados em 15–17.  
- **Kernel density por cor**: vinhos tintos tendem a notas ligeiramente maiores.  
- **Gráfico de pares (pairplot)**: correlação entre variáveis numéricas destacando a relação entre preço, álcool e nota.  
- **Heatmap**: correlações numéricas com destaque para álcool e preços sobre a nota.  
- **Top 30 tipos de uva**: gráficos de barras para frequência.  
- **Top regiões e produtores**: contagens das principais regiões e produtores na base.

---

## 🧩 Insights e Conclusões

- Juízes tendem a avaliar vinhos entre 15–17, com quase nenhuma nota abaixo de 11.5.  
- Vinhos tintos recebem notas ligeiramente superiores à média dos brancos.  
- O preço e teor alcoólico têm forte correlação positiva com as notas, mas o ano da safra impacta pouco.  
- Tipos de uva mais frequentes e regiões/produtores mais representativos foram identificados, auxiliando segmentação de mercado.

---

## ⚙️ Instalação & Execução

**Requisitos**: Python 3.8+

```bash
# Clone o repositório
git clone https://github.com/PedroSilva0z/Vinicola_data_exploration.git

# Acesse a pasta
cd Vinicola_data_exploration

# (Opcional) Crie um ambiente virtual
python -m venv venv
source venv/bin/activate  # ou venv\Scripts\activate no Windows

# Instale as dependências
pip install -r requirements.txt

# Execute o notebook
jupyter notebook Vinicola_data_exploration.ipynb
```


## 👤 Autor

**Pedro Silveira**  
📍 São Paulo, Brasil  
🔗 [LinkedIn](https://www.linkedin.com/in/silveirapedrosil)  

---

## 🤝 Contribuições

Contribuições, sugestões e melhorias são muito bem-vindas!  
Basta abrir uma *issue* ou enviar um *pull request*.

