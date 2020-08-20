---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb172798e774a85dd3886b81351ff48c877763e9
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821364"
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

await graphClient.Me.Profile.Interests["{id}"]
    .Request()
    .UpdateAsync(personInterest);

```