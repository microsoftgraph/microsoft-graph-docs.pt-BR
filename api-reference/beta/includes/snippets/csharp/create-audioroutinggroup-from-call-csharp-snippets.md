---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3521b5ff1645ee6140a65ee3407873f409b5daea
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933767"
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

await graphClient.App.Calls["{id}"].AudioRoutingGroups
    .Request()
    .AddAsync(audioRoutingGroup);

```