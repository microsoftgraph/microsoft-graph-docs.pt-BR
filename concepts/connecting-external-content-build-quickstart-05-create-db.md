<!-- markdownlint-disable MD002 MD025 MD041 -->

1. <span data-ttu-id="345ff-101">Abra sua interface de linha de comando (CLI) no diretório onde PartsInventoryConnector.csproj está localizado.</span><span class="sxs-lookup"><span data-stu-id="345ff-101">Open your command line interface (CLI) in the directory where PartsInventoryConnector.csproj is located.</span></span>
2. <span data-ttu-id="345ff-102">Execute os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="345ff-102">Run the following commands:</span></span>

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> <span data-ttu-id="345ff-103">Execute os comandos a seguir se um esquema mudar no arquivo CSV e refletir essas alterações no banco de dados SQLite.</span><span class="sxs-lookup"><span data-stu-id="345ff-103">Run the following commands if a schema changes in the CSV file, and reflect those changes into the SQLite database.</span></span>

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
