---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed6ad941a791eebaf15154efa7602805c3b87f01
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740176"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Groups["{id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```