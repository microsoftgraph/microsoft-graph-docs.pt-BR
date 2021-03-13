---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7ca391cffb0158476006d1c85a86292e5025e51
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroup = new AudioRoutingGroup
{
    Id = "oneToOne",
    RoutingMode = RoutingMode.OneToOne,
    Sources = new List<String>()
    {
        "632899f8-2ea1-4604-8413-27bd2892079f"
    },
    Receivers = new List<String>()
    {
        "550fae72-d251-43ec-868c-373732c2704f"
    }
};

await graphClient.Communications.Calls["{call-id}"].AudioRoutingGroups
    .Request()
    .AddAsync(audioRoutingGroup);

```