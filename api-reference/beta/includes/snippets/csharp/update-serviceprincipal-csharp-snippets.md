---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c24ddb6cf7a3a15f35413ab6d06be6aa04b3b32
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    AppRoleAssignmentRequired = true
};

await graphClient.ServicePrincipals["{id}"]
    .Request()
    .UpdateAsync(servicePrincipal);

```