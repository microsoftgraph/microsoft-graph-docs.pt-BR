<!-- markdownlint-disable MD002 MD025 MD041 -->

1. Abra sua interface de linha de comando (CLI) no diretório onde PartsInventoryConnector.csproj está localizado.
2. Execute os seguintes comandos:

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> Execute os comandos a seguir se um esquema mudar no arquivo CSV e refletir essas alterações no banco de dados SQLite.

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
