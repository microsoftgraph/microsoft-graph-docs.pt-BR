---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d54d3d2cef8ab1acb7933f18975d137a14eaf312
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    OfficeLocation = "city-value"
};

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```