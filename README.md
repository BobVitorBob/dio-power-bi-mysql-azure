# Integração do Power BI com um banco de dados MySQL hospedado na Azure
Repositório do projeto de integração do power bi com banco de dados MySQL usando Azure

## Passos

- Criar um banco MySQL na Azure. O nome padrão é _azure_company_, para usar outro nome é preciso modificar os scripts de criação e população.
- Configurar o acesso ao banco para permitir acessar usando o seu IP.
- Executar os scripts de criação e população pelo azure shell. É preciso adicionar o certificado para conexão usando TSL e configurar o shell para conectar com o banco.
- Conectar o Power BI com o banco MySQL.

## Transformações feitas no Power BI
### employee
- Adição do campo Department com o departamento do colaborador.
- Adição do campo SuperFName com o nome completo do gerente do colaborador.
- Troca dos campos Fname, Minit e Lname pelo campo FName, contendo o nome completo do colaborador
- Troca do campo Address pelos campos AddrNumber, District, City e State, contendo as mesmas informações mas agora separadas.
### department
- Adição do campo "Location" com o local do departamento.
- Adição do campo DFullName com o nome do departamento e local separados por "-". Os campos originais foram mantidos para uso futuro.
### dependent
- Adição do campo EFullName com o nome do colaborador referente.
### dept_locations
- NA
### project
- Adição do campo Department com o departamento do projeto.
### works_on
- Adição do campo ProjectName com o nome do projeto.
- Adição do campo EName com o nome do colaborador.