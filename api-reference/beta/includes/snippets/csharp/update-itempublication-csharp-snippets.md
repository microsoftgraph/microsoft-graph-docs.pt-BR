---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50aab1308f803f823b80642859dd24c957d04e3b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPublication = new ItemPublication
{
    Publisher = "International Association of Branding Management Publishing",
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
};

await graphClient.Users["{user-id}"].Profile.Publications["{itemPublication-id}"]
    .Request()
    .UpdateAsync(itemPublication);

```