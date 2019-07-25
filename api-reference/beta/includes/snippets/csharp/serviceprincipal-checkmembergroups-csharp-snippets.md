---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43c63a9b10f7e1c08d25dd68241af07a30d20930
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.ServicePrincipals["{id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```