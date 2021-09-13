---
ms.localizationpriority: medium
ms.openlocfilehash: e04c28e801be69487d83e5b5a3184c4702652aa3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289499"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

1. Abra sua interface de linha de comando (CLI) no diretório onde PartsInventoryConnector.csproj está localizado.
2. Execute o seguinte comando para inicializar os segredos do usuário do projeto.

    ```dotnetcli
    dotnet user-secrets init
    ```

3. Execute os comandos a seguir para armazenar a ID do aplicativo, o segredo do aplicativo e a ID do locatário no armazenamento secreto do usuário.

    ```dotnetcli
      dotnet user-secrets set appId "YOUR_APP_ID_HERE"
      dotnet user-secrets set appSecret "YOUR_APP_SECRET_HERE"
      dotnet user-secrets set tenantId "YOUR_TENANT_ID_HERE"
    ```
