---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 195eeb9171c476fb20eeb354458c38efbb6a4566
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43127130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "My Day at the Beach",
    AdditionalData = new Dictionary<string, object>()
    {
        {"@microsoft.graph.conflictBehavior","rename"}
    },
    Bundle = new Bundle
    {
        Album = new Album
        {
        }
    },
    Children = new List<DriveItem>()
    {
        new DriveItem
        {
            Id = "1234asdf"
        }
    }
};

await graphClient.Drive.Bundles
    .Request()
    .AddAsync(driveItem);

```