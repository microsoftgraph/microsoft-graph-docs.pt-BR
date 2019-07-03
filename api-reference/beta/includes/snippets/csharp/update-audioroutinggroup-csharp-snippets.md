---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb54bdb6a6aab192139e409ac0bd18821c98a99b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var AudioRoutingGroup = new AudioRoutingGroup
{
    Id = "oneToOne",
    RoutingMode = RoutingMode.OneToOne,
    Sources = new List<String>()
    {
        "632899f8-2ea1-4604-8413-27bd2892079f"
    },
    Receivers = new List<String>()
    {
        "550fae72-d251-43ec-868c-373732c2704f",
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
    }
};

await graphClient.App.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .UpdateAsync(AudioRoutingGroup);

```