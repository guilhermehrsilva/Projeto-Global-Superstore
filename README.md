# 📊 Global Superstore - Análise de Eficiência Comercial e Lucratividade

[Dashboard Preview](dashboard/Dashboard.pdf)
*(Nota: Visualize o PDF acima para ver o layout final em alta resolução)*

## 🏢 Sobre o Projeto
Este projeto simula um cenário real de Business Intelligence onde uma rede varejista global precisava identificar gargalos de lucratividade. Apesar do alto volume de vendas, a margem líquida da empresa não acompanhava o crescimento.

O objetivo foi transformar dados brutos de transações em um dashboard estratégico para apoiar a tomada de decisão da diretoria, focando em responder: **"Onde estamos perdendo dinheiro?"**

## 📂 Estrutura do Repositório
* `/Dataset`: Contém os dados brutos (CSV) com histórico de transações globais.
* `/ETL`: Planilhas de apoio utilizadas para validação de qualidade de dados e auditoria inicial (Excel).
* `/Dashboard`: Arquivo fonte do Power BI (`.pbix`) e exportação em PDF.

## 🛠️ Tecnologias e Ferramentas
* **Microsoft Power BI:** Ferramenta principal para ingestão, modelagem e visualização.
* **Power Query:** Utilizado para limpeza de dados (ETL), padronização de nomes de países e correção de tipagem de datas.
* **DAX (Data Analysis Expressions):** Criação de medidas calculadas para *Margem de Lucro %*, *Variação YoY* e *Faturamento Total*.
* **Excel:** Utilizado para *Quick Audit* (auditoria rápida) e validação dos números antes da carga no BI.
* **Figma/Canva:** Design de background e identidade visual (Logo: Guilherme Risson Analytics).

## ⚙️ Etapas de Desenvolvimento
1.  **Coleta e ETL:** Importação do arquivo `superstore_sales.csv`. Tratamento de erros de locale (ponto vs vírgula) e verificação de nulos.
2.  **Modelagem de Dados:** Criação da Tabela Calendário (dCalendario) para análises temporais precisas.
3.  **Visualização (Data Viz):**
    * Implementação de **Dark Mode** para visualização executiva.
    * Uso de **Formatação Condicional Divergente**: Vermelho para valores negativos (Prejuízo) e Azul/Verde para positivos.
    * Mapa Geoespacial para identificação de mercados ineficientes.
4.  **UX/UI:** Criação de filtros laterais e cartões de KPI com alto contraste.

## 💡 Principais Insights
* **Produtos Ofensores:** As categorias "Tables" e "Bookcases" apresentam performance negativa consistente, exigindo revisão de preços ou custos.
* **Impacto dos Descontos:** Foi identificada uma correlação direta entre descontos acima de 20% e margem negativa.
* **Sazonalidade:** O final do ano apresenta picos de venda, mas o lucro não cresce na mesma proporção devido a promoções agressivas.

---
**Autor:** Guilherme Risson
*Projeto desenvolvido para portfólio de Análise de Dados.*
