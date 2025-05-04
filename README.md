# Configurando uma instância de Banco de Dados na Azure

 > ℹ️ **NOTE:**  Este repositório é um desafio de projeto proposto no curso "Microsoft 50 Anos - Computação em Nuvem com Azure" na plataforma da [DIO](https://dio.me)

Projeto com o objetivo de praticar o processo de configuração de uma instância de Banco de Dados na Azure.

🗂️ O que é uma instância de banco de dados?
É um serviço em nuvem que permite criar e gerenciar um banco de dados (como MySQL, SQL Server, PostgreSQL etc.) sem precisar instalar nada no seu computador. O Azure cuida da infraestrutura, segurança e backups.

🛠️ Passo a passo: Criando uma instância de banco de dados no Azure (exemplo com Azure SQL)
1. Acesse o Portal do Azure
Vá para https://portal.azure.com e faça login com sua conta.

2. Crie um Grupo de Recursos (se ainda não tiver)
No menu à esquerda, clique em "Grupos de recursos" > "+ Criar".

Dê um nome e selecione a região mais próxima.

3. Crie um Banco de Dados SQL
Clique em "Criar um recurso" > "Banco de Dados" > "SQL Database".

4. Preencha os detalhes do banco
Nome do banco de dados: qualquer nome que desejar (ex: meubanco).

Assinatura: selecione sua assinatura (geralmente é a gratuita).

Grupo de recursos: selecione o grupo criado.

Servidor: clique em "Criar novo", e:

Dê um nome ao servidor.

Crie um login de administrador e senha.

Escolha a região.

5. Configuração de desempenho
Para testes, escolha a opção de camada gratuita ou a mais barata.

Você pode ajustar CPU e memória conforme necessário.

6. Configurações adicionais
Pode deixar as opções padrão (como backup, auditoria, etc.) ou personalizar depois.

7. Revisar e Criar
Clique em "Revisar + Criar", revise os dados e clique em "Criar".

Aguarde alguns minutos até a implantação ser concluída.

🔗 Como se conectar ao banco de dados
1. Permitir acesso ao seu IP
No painel do banco criado, vá até "Conexão" > "Regras de firewall".

Adicione seu IP público para poder se conectar.

2. Conectar com ferramentas
Use o SQL Server Management Studio (SSMS) ou Azure Data Studio.

Insira:
Servidor: nome_do_servidor.database.windows.net

Usuário: criado na etapa anterior

Senha: a mesma da criação


✅ Finalizado
Você agora tem uma instância de banco de dados funcional na nuvem. Pode criar tabelas, inserir dados e usar em aplicativos, sites, ou para estudos.


📚 Recursos Adicionais
Tutorial Oficial da Microsoft: Para um guia detalhado com imagens, acesse Início Rápido – Criar um banco de dados SQL no portal do Azure.
(https://learn.microsoft.com/pt-br/azure/azure-sql/database/single-database-create-quickstart?view=azuresql&tabs=azure-portal)
