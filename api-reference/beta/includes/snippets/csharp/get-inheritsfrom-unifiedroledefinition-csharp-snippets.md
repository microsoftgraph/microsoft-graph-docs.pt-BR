---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d5e8720fa038d5fe4d81abca7433d5a136ceda5
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.Directory.RoleDefinitions["fdd7a751-b60b-444a-984c-02652fe8fa1c"]
    .Request()
    .Expand("inheritsPermissionsFrom")
    .GetAsync();

```