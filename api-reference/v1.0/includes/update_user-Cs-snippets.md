---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64f3465f2cca9a803587aec82f5a86b32e439e67
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AccountEnabled = true,
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    City = "city-value"
};

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```