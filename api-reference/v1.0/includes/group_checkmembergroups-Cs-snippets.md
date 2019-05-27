---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed6ad941a791eebaf15154efa7602805c3b87f01
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478122"
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