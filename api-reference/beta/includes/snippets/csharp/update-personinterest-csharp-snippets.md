---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc13e83a1739a377356ab080415444bfdcc1259b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = new PersonInterest
{
    Categories = new List<String>()
    {
        "Sports"
    }
};

await graphClient.Me.Profile.Interests["{personInterest-id}"]
    .Request()
    .UpdateAsync(personInterest);

```