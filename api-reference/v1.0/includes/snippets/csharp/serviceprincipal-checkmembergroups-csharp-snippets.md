---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7be445d75c184904d45a4aa3bfde44be87e177e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```