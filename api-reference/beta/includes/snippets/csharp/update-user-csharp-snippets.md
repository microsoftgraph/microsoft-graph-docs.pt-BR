---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9dd475e8ae8fed361a9cb3f4084fc28d88381ce9
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    BusinessPhones = new List<String>()
    {
        "+1 425 555 0109"
    },
    OfficeLocation = "18/2111"
};

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```