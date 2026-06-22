# SCTEC - Mini Projeto

## Sobre o projeto

O dataview.ipynb é um projeto de análise exploratória de dados (EDA) de vendas, desenvolvido em Python em um notebook. 
O notebook lê, limpa, transforma, analisa e visualiza um dataset de vendas gerado de forma fictícia, gerando insights relevantes e relatórios exportáveis.


### Importante

A versão 1 foi escolhida para data/final/. 

Pelas análises, verificou-se que os outliers correspondem a vendas reais de notebooks em grandes quantidades. Considerando que o dataset também apresenta compras em grandes quantidades para outros produtos e que o preço unitário dos notebooks é naturalmente mais alto, essas observações não caracterizam erros ou inconsistências nos dados. Dessa forma, os "outliers" serão mantidos, optando pela versão 1.


## O que o projeto analisa

- Receita total e volume de vendas por mês
- Top produtos e categorias por receita
- Desempenho por região
- Segmentação de clientes por nível de gasto (Bronze, Prata, Ouro)
- Comparação entre os dados com e sem tratamento de outliers (v1 e v2)
- Exportação de relatórios em CSV e JSON

## Objetivo

Praticar os principais conceitos:

- Lógica de programação com Python
- Variáveis, tipos de dados e operadores
- Condicionais (`if`, `elif`, `else`) e repetição (`for`, `while`)
- Funções com parâmetros, retorno e funções lambda
- Funções reutilizáveis
- Leitura e escrita de arquivos CSV e JSON
- Módulo `datetime` para manipulação de datas
- Expressões regulares com o módulo `re`
- Pandas: DataFrames, limpeza, `groupby`, filtros e transformações
- NumPy: arrays, operações vetorizadas, broadcasting
- Detecção e tratamento de outliers (IQR ou z-score)
- Matplotlib e Seaborn: gráficos, customização e exportação em PNG
- Uso básico do GitHub

## Como executar

Atualizado em 21 de jun. de 2026

Criado por: Jênifer Vieira Goedert

### No Google Colab (recomendado)

1. Faça upload do notebook `dataview.ipynb`
2. Abra o arquivo carregado no Colab
3. Execute as células na ordem, de cima para baixo

### Localmente com VS Code

1. Instale o Python 3.12+ e o VS Code.
2. Instale as dependências:

```bash
pip install pandas numpy matplotlib seaborn
```

## Estrutura do projeto

```text
projeto/
│
├── data/
│   ├── raw/                         # Dataset bruto gerado∕baixado
│   ├── processed/
│   │   ├── v1_com_outliers/         # Dados de limpeza geral, outliers mantidos
│   │   └── v2_outliers_tratado/     # Limpeza v1 + tratamento de outliers
│   └── final/                       # Dataset escolhido para uso futuro
│
├── notebooks/
│   └── dataview.ipynb               # Notebook principal de EDA
│
├── outputs/
│   ├── metricas_mensais.csv
│   ├── clientes_segmentados.csv
│   ├── estatisticas_receita_total.json
│   ├── estatisticas_quantidade.json
│   ├── estatisticas_preco.json
│   └── graficos/
│
└── README.md
└── .gitignore
└── requirements.txt
```

## Ferramentas utilizadas

- Python 3.12.3
- VS Code
- Bibliotecas: 
    - Pandas (`pandas`)
    - NumPy (`numpy`)
    - Matplotlib (`matplotlib.pyplot`)
    - Seaborn (`seaborn`)
    - Datetime (`datetime`)
    - Random (`random`)
    - JSON (`json`)
    - OS (`os`)
    - Expressões Regulares (`re`)
- GitHub para versionamento

## Vídeo de demonstração
https://drive.google.com/file/d/1a6SEoj03y9JbxqLMAAmi1FvISVjJxtKi/view?usp=sharing
