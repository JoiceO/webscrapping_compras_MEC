
# Webscraping com dados públicos: compras de materiais didáticos pelo MEC (2025)

Fonte: Diário Oficial da União

Projeto elaborado com as **PyLadies SP no Open Data Day (07/03/2026)** que demonstra como automatizar a coleta de dados públicos, por meio de webscraping pelo Selenium, organizar os dados coletados e realizar uma análise exploratória inicial.


## 🔎 Contexto

O Diário Oficial da União publica diariamente atos administrativos, incluindo contratos firmados por órgãos do governo federal. Neste projeto, realizamos uma busca pela palavra-chave: **“materiais didáticos”** para identificar contratos firmados com o Ministério da Educação (MEC) ao longo de 2025.


## 🎯 Objetivos

Demonstrar, de forma prática, como automatizar tarefas de coleta de dados na web, incluindo:

* navegação automatizada em páginas web
* interação com elementos da página (botões, campos de busca, filtros)
* extração de informações estruturadas
* navegação entre páginas de resultados
* organização dos dados para análise

## 🔹 Tecnologias utilizadas

O projeto utiliza:

* **Python**
* **Google Colab**
* Bibliotecas: **Selenium**, **Pandas** e **Matplotlib**

## Processo de coleta de dados

A raspagem de dados consiste em:

1. acessar o site do Diário Oficial da União
2. realizar uma busca pela expressão “materiais didáticos”
3. aplicar filtros para identificar contratos do Ministério da Educação em 2025
4. percorrer as páginas de resultados
5. extrair informações relevantes de cada contrato

As principais informações coletadas são:

* número do processo
* órgão contratante
* empresa contratada
* objeto do contrato
* vigência
* valor total do contrato
* data de assinatura

Com isso, o conjunto de dados final possui as seguintes colunas:

* `processo`
* `contratante`
* `contratado`
* `objeto`
* `vigencia`
* `valor_total`
* `data_assinatura`
* `mes`

### Exportação dos dados

Ao final do processo, o dataset é exportado em formato CSV, permitindo que ele seja utilizado em outras ferramentas de visualização e análise.

### Análise exploratória dos dados

Após a coleta  e limpeza dos dados, para entender o comportamento das contratações, foi feita a seguinte análise:

1️⃣Estatísticas descritivas dos contratos <br>
2️⃣ Gasto total em materiais didáticos em 2025 <br>
3️⃣ Valor médio dos contratos <br>
4️⃣ Top 10 contratos mais caros <br>
5️⃣ Contrato mais barato <br>
6️⃣ Licitantes mais selecionados <br>
7️⃣ Concentração de fornecedores (HHI) <br>
8️⃣ Mês com mais contratos <br>
9️⃣ Mês com maior volume financeiro <br> 


## Possíveis extensões do projeto

Este projeto pode ser expandido de diversas formas, por exemplo:

* ampliar a coleta para outros anos
* analisar concentração de fornecedores
* construir dashboards interativos
* integrar a coleta com APIs ou automações periódicas




