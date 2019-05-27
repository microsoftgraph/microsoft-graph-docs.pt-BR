---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be9c99e5b77edda415f3bdf19561caf9e152e377
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Self help community for library",
    DisplayName = "Library Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "library",
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```