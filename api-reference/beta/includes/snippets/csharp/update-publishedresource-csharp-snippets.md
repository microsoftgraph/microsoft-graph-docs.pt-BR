---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c88fc1d2d77cc547a3ec75ad3807dce1473b1265
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = new PublishedResource
{
    DisplayName = "Demo provisioning (updated)"
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources["{publishedResource-id}"]
    .Request()
    .UpdateAsync(publishedResource);

```