---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1b0ac7b9b440c6ba18e8c9b68727d5418ba1936
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAward = new PersonAward
{
    IssuingAuthority = "International Association of Branding Management",
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
};

await graphClient.Users["{user-id}"].Profile.Awards["{personAward-id}"]
    .Request()
    .UpdateAsync(personAward);

```