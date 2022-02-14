---
ms.localizationpriority: medium
ms.openlocfilehash: e8f13a3fe886db688d12a997f0cddc38547a30f6
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805219"
---
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
