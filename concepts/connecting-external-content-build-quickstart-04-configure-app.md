<!-- markdownlint-disable MD002 MD025 MD041 -->

1. <span data-ttu-id="23182-101">Abra sua interface de linha de comando (CLI) no diretório onde PartsInventoryConnector.csproj está localizado.</span><span class="sxs-lookup"><span data-stu-id="23182-101">Open your command line interface (CLI) in the directory where PartsInventoryConnector.csproj is located.</span></span>
2. <span data-ttu-id="23182-102">Execute o seguinte comando para inicializar os segredos do usuário do projeto.</span><span class="sxs-lookup"><span data-stu-id="23182-102">Run the following command to initialize the user secrets for the project.</span></span>

    ```dotnetcli
    dotnet user-secrets init
    ```

3. <span data-ttu-id="23182-103">Execute os comandos a seguir para armazenar a ID do aplicativo, o segredo do aplicativo e a ID do locatário no armazenamento secreto do usuário.</span><span class="sxs-lookup"><span data-stu-id="23182-103">Run the following commands to store your app ID, app secret, and tenant ID in the user secret store.</span></span>
  
    ```dotnetcli
      dotnet user-secrets set appId "YOUR_APP_ID_HERE"
      dotnet user-secrets set appSecret "YOUR_APP_SECRET_HERE" (#CertificatesAndsecrets))
      dotnet user-secrets set tenantId "YOUR_TENANT_ID_HERE" 
    ```
