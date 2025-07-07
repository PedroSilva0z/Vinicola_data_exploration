# Vinicola Data Exploration 🍷

Exploração de dados sobre a produção, exportação e importação de vinhos e derivados no Brasil. Este projeto busca identificar padrões, entender influências externas (como clima e economia) e apoiar decisões estratégicas no setor vinícola.

---

## 📋 Sumário

- [Sobre o Projeto](#-sobre-o-projeto)  
- [Motivação](#-motivação)  
- [Dados](#-dados)  
- [Metodologia](#-metodologia)  
- [Instalação & Execução](#-instalação--execução)  
- [Resultados & Insights](#-resultados--insights)  
- [Conclusões](#-conclusões)  
- [Próximos Passos](#-próximos-passos)  
- [Autor](#-autor)  

---

## 🧠 Sobre o Projeto  

Este notebook analisa dados da cadeia produtiva de vinhos no Brasil, incluindo produção, exportação, importação e variáveis externas como clima, economia e qualidade do produto. A intenção é transformar dados em insights úteis para negócios e políticas públicas.

---

## 🎯 Motivação  

- Compreender fluxos comerciais (origem/destino, volume, receita)  
- Identificar padrões sazonais, geográficos e econômicos  
- Avaliar influências externas (clima, PIB, avaliações)  
- Apoiar decisões com base em evidências e visualizações

---

## 🗄️ Dados Utilizados  

- **Produção, exportação e importação** de vinhos no Brasil  
- **Clima**: temperatura média e pluviosidade nas regiões produtoras  
- **Indicadores socioeconômicos**: PIB, renda per capita, população  
- **Avaliações de vinhos**: notas médias e faixa de preço  

**Fonte principal**: Embrapa CNPUV + APIs públicas para dados climáticos e socioeconômicos.

---

## 🧪 Metodologia  

- Leitura e limpeza de dados com `pandas`  
- Análise exploratória com foco em distribuição, outliers e sazonalidade  
- Visualizações com `matplotlib` e `seaborn`  
- Análise multivariada e correlação  
- Agrupamentos e segmentações por tipo de produto, faixa de valor e localidade  
- Criação de sumários e insights para apresentações

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
