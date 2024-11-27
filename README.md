# Automação de Consultas de CPF

Automatização do processo de consulta de CPFs em uma página web, com leitura e registro de dados provenientes de uma planilha Excel. Este projeto foi desenvolvido para facilitar o acompanhamento da situação de CPFs (em dia ou pendente) e gerar relatórios atualizados automaticamente.


Principais Funcionalidades

Consulta Automatizada: Lê os dados de CPFs de uma planilha Excel e realiza consultas automáticas em uma página web.

Geração de Relatórios: Registra os resultados das consultas (situação do CPF, data e método de pagamento, se aplicável) em uma nova planilha.

Interação Precisa: Utiliza o Selenium para preencher campos, clicar em botões e extrair informações da página web com precisão.

Integração Excel: Manipulação das planilhas é realizada de forma direta e segura com a biblioteca openpyxl.


Tecnologias Utilizadas

Python: Linguagem de programação principal.
openpyxl: Para manipulação de planilhas Excel.
Selenium: Para automação de navegação e interação com páginas web.
Excel: Base para o input dos dados dos CPFs e para armazenar os relatórios gerados.


Como Funciona

O usuário insere os dados de clientes (nome, valor, CPF e vencimento) em uma planilha Excel.

O script utiliza Selenium para acessar a página de consulta de CPF e realiza as buscas automaticamente.

Dependendo do status retornado pela consulta:
  Se o CPF estiver "em dia", o script captura a data e o método de pagamento.
  Se o CPF estiver "pendente", apenas registra o status.

Os resultados são gravados em uma planilha Excel separada, contendo todas as informações processadas.

