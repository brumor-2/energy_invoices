# Energy Invoices – Processamento de Faturas de Energia (Python)

[Read in English](https://github.com/brumor-2/energy_invoices/blob/main/README.md)

Este projeto automatiza o processamento de faturas de energia elétrica (formato PDF) da ENEL para 70 escolas.  
O script busca arquivos PDF em uma pasta específica, renomeia cada arquivo de acordo com o nome e número de instalação da escola, extrai os valores das faturas e gera uma planilha Excel com o resumo e o valor total.

---

## Tecnologias Utilizadas
- Python  
- Pandas (manipulação e exportação de planilhas Excel)  
- `os`, `re`, `openpyxl` ou bibliotecas equivalentes para manipulação de arquivos e leitura de PDFs  

---

## O que Aprendi
- **Renomeação de arquivos em lote** com mapeamento personalizado por escola e número de instalação  
- **Extração de dados de PDFs semi-estruturados**  
- **Consolidação de dados no Excel**, incluindo cálculo de totais  
- **Aplicação prática de Python** para automação de tarefas reais  
- **Documentação clara** para reprodução e adaptação do código  

---

## Como Usar
1. Coloque todos os PDFs na pasta `input_pdfs/`.
2. Ajuste o mapeamento no arquivo `energy_invoices_base.py` para corresponder aos dados da sua escola/instalação.
3. Execute:
   ```bash
   python energy_invoices_base.py
O arquivo output.xlsx será gerado com os arquivos renomeados e a planilha consolidada.

⚠️ Observações
É necessário adaptar o mapeamento das escolas para uso próprio — dados sensíveis não foram incluídos neste repositório.

O padrão dos PDFs deve corresponder ao formato das faturas da ENEL para que a extração funcione corretamente.
