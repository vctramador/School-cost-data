# School Cost Visualization Project

## Description

This project involves the analysis and visualization of costs associated with different schools. We use popular Python libraries such as `pandas` and `matplotlib` to process and visualize the data in a clear and intuitive manner. The goal is to identify and highlight the cost of each school without duplication, ensuring an accurate and comprehensible view.

## Motivation

Analyzing educational costs is essential to understand the differences between institutions and to make informed decisions. This project was developed to provide an easy-to-interpret visualization of costs per school, highlighting institutions without data duplication, which is common in large and complex datasets.

## Features

- **Duplicate Removal**: Ensures that each school appears only once in the visualization.
- **Data Sorting**: Costs are sorted to facilitate data interpretation.
- **Clear Visualization**: Horizontal bar charts are used for clear and readable visualization.

## Technologies Used

- **Python**: Main language of the project.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For creating charts and visualizations.

## How to Use

1. Clone this repository:

    ```sh
    git clone https://github.com/your-username/repository-name.git
    ```

2. Install the necessary dependencies:

    ```sh
    pip install pandas matplotlib
    ```

3. Run the main script:

    ```sh
    python main.py
    ```

## Usage Example

Here is a basic example of how the code is structured and used:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Example DataFrame
data = {
    'School': ['School A', 'School B', 'School A', 'School C', 'School B'],
    'Cost': [100, 200, 150, 300, 250]
}
df = pd.DataFrame(data)

# Removing duplicates, keeping the first occurrence
df_unique = df.drop_duplicates(subset='School', keep='first')

# Sorting the data for better visualization
df_unique = df_unique.sort_values(by='Cost')

# Data for the chart
y = df_unique['School']
x = df_unique['Cost']

# Creating the bar chart
plt.barh(y, x)
plt.title('Cost by School')
plt.xlabel('Cost')
plt.ylabel('School')
plt.show()
```

## Contributions

Contributions are welcome! If you have suggestions, improvements, or find any bugs, feel free to open an issue or submit a pull request.

#Português


# Projeto de Visualização de Custos por Escola

## Descrição

Este projeto é uma análise e visualização dos custos associados a diferentes escolas. Utilizamos bibliotecas populares de Python, como `pandas` e `matplotlib`, para processar e visualizar os dados de forma clara e intuitiva. O objetivo é identificar e destacar o custo de cada escola sem duplicações, garantindo uma visão precisa e compreensível.

## Motivação

A análise de custos educacionais é fundamental para entender as diferenças entre instituições e tomar decisões informadas. Este projeto foi desenvolvido para proporcionar uma visualização fácil de interpretar dos custos por escola, destacando as instituições sem duplicação de dados, o que é comum em datasets grandes e complexos.

## Funcionalidades

- **Remoção de duplicatas**: Garantimos que cada escola apareça apenas uma vez na visualização.
- **Ordenação de dados**: Os custos são ordenados para facilitar a interpretação dos dados.
- **Visualização clara**: Utilizamos gráficos de barras horizontais para uma visualização clara e legível.

## Tecnologias Utilizadas

- **Python**: Linguagem principal do projeto.
- **Pandas**: Para manipulação e análise de dados.
- **Matplotlib**: Para criação dos gráficos e visualizações.

## Como Usar

1. Clone este repositório:

    ```sh
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```

2. Instale as dependências necessárias:

    ```sh
    pip install pandas matplotlib
    ```

3. Execute o script principal:

    ```sh
    python main.py
    ```

## Exemplo de Uso

Aqui está um exemplo básico de como o código é estruturado e utilizado:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Exemplo de DataFrame
data = {
    'School': ['School A', 'School B', 'School A', 'School C', 'School B'],
    'Cost': [100, 200, 150, 300, 250]
}
df = pd.DataFrame(data)

# Removendo duplicatas, mantendo o primeiro registro encontrado
df_unique = df.drop_duplicates(subset='School', keep='first')

# Ordenando os dados para facilitar a visualização
df_unique = df_unique.sort_values(by='Cost')

# Dados para o gráfico
y = df_unique['School']
x = df_unique['Cost']

# Criando o gráfico de barras
plt.barh(y, x)
plt.title('Custo por Escola')
plt.xlabel('Custo')
plt.ylabel('Escola')
plt.show()
```

## Contribuições

Contribuições são bem-vindas! Se você tem sugestões, melhorias ou encontrou algum bug, sinta-se à vontade para abrir uma issue ou enviar um pull request.
