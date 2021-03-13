---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10f0b5fa46ac62c53afd8a1bec4697e602893644
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPatent = new ItemPatent
{
    Number = "USPTO-3954432633",
    WebUrl = "https://patents.gov/3954432633"
};

await graphClient.Users["{user-id}"].Profile.Patents["{itemPatent-id}"]
    .Request()
    .UpdateAsync(itemPatent);

```