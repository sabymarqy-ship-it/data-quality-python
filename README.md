## 📊 PROJETO: Validação de Data Quality em Datas (Python/Pandas)

**Autor:** [Saby_Marqui]

---

### 🎯 RESUMO EXECUTIVO (HABILIDADES ANALÍTICAS)

Este projeto demonstra a capacidade de um analista de dados em construir um **pipeline de Data Quality robusto**, focado na auditoria de datas.

A solução implementada utiliza técnicas avançadas do Pandas para **tratamento em lote (vetorial)** e **Indexação Booleana**, garantindo que o relatório de conformidade seja gerado de forma rápida e escalável.

O pipeline verifica três dimensões cruciais da qualidade de dados: **Consistência**, **Completude** e **Validade**.

---

### 🛠️ TECNOLOGIAS E FERRAMENTAS

| Ferramenta | Propósito no Projeto | Habilidade Demonstrada |
| :--- | :--- | :--- |
| **Python** | Linguagem central. | Proficiência em desenvolvimento de scripts e funções personalizadas (`def`). |
| **Pandas** | Manipulação de DataFrames. | Domínio de Programação Vetorial e alto desempenho na limpeza de grandes volumes de dados. |
| **Dateparser** | Tratamento de formatos de data híbridos. | Utilização de bibliotecas especializadas para resolver problemas complexos de parsing (conversão de strings). |
| **Datetime** | Definição de limite temporal. | Capacidade de integrar módulos nativos para estabelecer regras de negócio e limites de validade. |

---

### 🔎 PIPELINE DE VALIDAÇÃO (PASSO A PASSO)

O *notebook* `Validador_de_Data_Quality.ipynb` executa a seguinte sequência de auditoria:

1.  **Limpeza e Consistência:** Aplicação da função `parse_data_hibrido` (usando `dateparser`) via método `.apply()`. Converte a coluna de *strings* para o tipo `datetime64[ns]`.
2.  **Completude (Missing Values):** Contagem dos valores nulos após a limpeza usando a expressão `.isnull().sum()`. Quantifica a incompletude.
3.  **Validade (Regras de Negócio):** Criação de colunas booleanas de rastreamento de erros: `Erro_Data_Futura` (`Data > Hoje`) e `Erro_Data_Antiga` (`Data < 1900-01-01`).
4.  **Relatório Final:** Agrega a contagem de todos os erros e utiliza um **Operador Ternário** para gerar o **STATUS FINAL** (APROVADO ou REPROVADO).


---

### 🎯 RESUMO EXECUTIVO (HABILIDADES ANALÍTICAS)

Este projeto demonstra a capacidade de um analista de dados em construir um **pipeline de Data Quality robusto**, focado na auditoria de datas.

A solução implementada utiliza técnicas avançadas do Pandas para **tratamento em lote (vetorial)** e **Indexação Booleana**, garantindo que o relatório de conformidade seja gerado de forma rápida e escalável.

O pipeline verifica três dimensões cruciais da qualidade de dados: **Consistência**, **Completude** e **Validade**.

---

### 🛠️ TECNOLOGIAS E FERRAMENTAS

| Ferramenta | Propósito no Projeto | Habilidade Demonstrada |
| :--- | :--- | :--- |
| **Python** | Linguagem central. | Proficiência em desenvolvimento de scripts e funções personalizadas (`def`). |
| **Pandas** | Manipulação de DataFrames. | Domínio de Programação Vetorial e alto desempenho na limpeza de grandes volumes de dados. |
| **Dateparser** | Tratamento de formatos de data híbridos. | Utilização de bibliotecas especializadas para resolver problemas complexos de parsing (conversão de strings). |
| **Datetime** | Definição de limite temporal. | Capacidade de integrar módulos nativos para estabelecer regras de negócio e limites de validade. |

---

### 🔎 PIPELINE DE VALIDAÇÃO (PASSO A PASSO)

O *notebook* `Validador_de_Data_Quality.ipynb` executa a seguinte sequência de auditoria:

1.  **Limpeza e Consistência:** Aplicação da função `parse_data_hibrido` (usando `dateparser`) via método `.apply()`. Converte a coluna de *strings* para o tipo `datetime64[ns]`.
2.  **Completude (Missing Values):** Contagem dos valores nulos após a limpeza usando a expressão `.isnull().sum()`. Quantifica a incompletude.
3.  **Validade (Regras de Negócio):** Criação de colunas booleanas de rastreamento de erros: `Erro_Data_Futura` (`Data > Hoje`) e `Erro_Data_Antiga` (`Data < 1900-01-01`).
4.  **Relatório Final:** Agrega a contagem de todos os erros e utiliza um **Operador Ternário** para gerar o **STATUS FINAL** (APROVADO ou REPROVADO).

---

### 🚀 COMO RODAR O PROJETO

1.  **Clone o Repositório:**
    ```bash
    git clone [https://github.com/sabymarqy-ship-it/data-quality-python]
    ```
2.  **Abra o Notebook:** Abra o arquivo `Validador_de_Data_Quality.ipynb` no Jupyter ou Google Colab.
3.  **Execução:** Certifique-se de que o arquivo de dados (`arq.csv`) está na mesma pasta. Execute todas as células sequencialmente para ver o pipeline de limpeza e o relatório final.

4.  **Autor:** [saby_marqy]
