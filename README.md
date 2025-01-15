# Integração do Power BI com um banco de dados MySQL hospedado na Azure
Repositório do projeto de integração do power bi com banco de dados MySQL usando Azure

## Passos

- Criar um banco MySQL na Azure. O nome padrão é _azure_company_, para usar outro nome é preciso modificar os scripts de criação e população.
- Configurar o acesso ao banco para permitir acessar usando o seu IP.
- Executar os scripts de criação e população pelo azure shell. É preciso adicionar o certificado para conexão usando TSL e configurar o shell para conectar com o banco.
- Conectar o Power BI com o banco MySQL.