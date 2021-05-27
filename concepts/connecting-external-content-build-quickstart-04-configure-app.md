<!-- markdownlint-disable MD002 MD025 MD041 -->

1. Abra sua interface de linha de comando (CLI) no diretório onde PartsInventoryConnector.csproj está localizado.
2. Execute o seguinte comando para inicializar os segredos do usuário do projeto.

    ```dotnetcli
    dotnet user-secrets init
    ```

3. Execute os comandos a seguir para armazenar a ID do aplicativo, o segredo do aplicativo e a ID do locatário no armazenamento secreto do usuário.
  
    ```dotnetcli
      dotnet user-secrets set appId "YOUR_APP_ID_HERE"
      dotnet user-secrets set appSecret "YOUR_APP_SECRET_HERE" (#CertificatesAndsecrets))
      dotnet user-secrets set tenantId "YOUR_TENANT_ID_HERE" 
    ```
