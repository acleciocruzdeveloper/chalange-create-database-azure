# Como lançar uma instância de banco de dados na Azure (Nível Free)

## 1. Criando uma Conta no Azure
Se ainda não tiver uma conta, crie uma em [Azure Portal](https://portal.azure.com) e aproveite o **nível gratuito** para novos usuários.

## 2. Acessando o Azure Portal
Entre no portal do Azure e navegue até **"Banco de Dados SQL"**.

## 3. Criando um Banco de Dados no Nível Gratuito
1. Clique em **"Criar recurso"** e selecione **Banco de Dados SQL**.
2. Escolha um **Servidor SQL** existente ou crie um novo.
3. No plano de **Preço**, selecione **Serviço Computacional sem Servidor** (_serverless_) ou o **Plano gratuito** (_Free Tier_), se disponível.
4. Configure nome, região e autenticação conforme necessário.
5. Clique em **"Revisar e Criar"** e, em seguida, **"Criar"**.

## 4. Conectando-se ao Banco de Dados
Após a implantação:
1. Pegue a **string de conexão** disponível no portal.
2. Use ferramentas como **Azure Data Studio** ou **SQL Server Management Studio (SSMS)** para se conectar.

## 5. Testando a Conexão
Execute o seguinte comando SQL para garantir que o banco está funcional:
```sql
SELECT 'Azure SQL Database está pronto!' AS Status;
