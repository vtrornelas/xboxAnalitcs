# Xbox Game Pass Sales Analysis

## Descrição do Projeto

Este projeto realiza uma análise das vendas de assinaturas do Xbox Game Pass ao longo de 2024, utilizando uma base de dados fictícia. O objetivo é responder perguntas de negócio relevantes sobre receitas, perfil de assinantes e desempenho de produtos agregados (como passes de temporada EA Play e Minecraft), além de apresentar um dashboard consolidado para visualização dos principais indicadores.

---

## Estrutura do Projeto

```
/
├── Xbox.xlsx
├── README.md
```

---

## Dados

O arquivo principal é [`Xbox.xlsx`](Xbox.xlsx)[1], que contém as seguintes abas:

- **Assets:** Paleta de cores e logos para padronização visual.
- **Bases:** Base de assinantes com os campos:
  - `Subscriber ID`, `Name`, `Plan`, `Start Date`, `Auto Renewal`, `Subscription Price`, `Subscription Type`, `EA Play Season Pass`, `EA Play Season Pass Price`, `Minecraft Season Pass`, `Minecraft Season Pass Price`, `Coupon Value`, `Total Value`
- **Cálculos:** Resumos e tabelas dinâmicas que respondem perguntas como:
  - Faturamento total de planos anuais
  - Faturamento por renovação automática
  - Vendas de passes de temporada (EA Play e Minecraft)
  - Faturamento mensal agregado
- **Dashboard:** Painel visual consolidado, com período de cálculo e data de atualização.

---

## Como Reproduzir

### Pré-requisitos

- Microsoft Excel (ou Google Sheets/LibreOffice Calc)
- Opcional: Python (com pandas, openpyxl) para análises automatizadas

### Passos

1. **Clone o repositório**
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
   ```

2. **Abra o arquivo de dados**
   - Utilize o Excel ou editor de planilhas de sua preferência para abrir `Xbox.xlsx`.

3. **Explore as abas**
   - `Bases`: visualize os dados brutos.
   - `Cálculos`: veja os resumos e respostas às perguntas de negócio.
   - `Dashboard`: confira os principais resultados em formato visual.

4. **(Opcional) Análise em Python**
   ```python
   import pandas as pd
   df = pd.read_excel('Xbox.xlsx', sheet_name='Bases')
   print(df.head())
   ```

5. **Atualize os dados**
   - Para atualizar indicadores, adicione novos registros na aba `Bases` e atualize as tabelas dinâmicas e gráficos.

---

## Observações

- Os dados são fictícios e têm finalidade didática.
- O projeto pode ser expandido para novas métricas ou integração com ferramentas de BI.
- Paleta de cores e logos estão disponíveis na aba `Assets` para uso em relatórios.

---

**Autor:**  
Victor Ornelas

---

[1]: O arquivo `Xbox.xlsx` está incluído neste repositório.
