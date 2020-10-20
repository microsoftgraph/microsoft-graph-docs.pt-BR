---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88800dfee9e2391b13fd68604b167411e3430687
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySetting = new DirectorySetting
{
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "name-value",
            Value = "value-value"
        }
    }
};

await graphClient.Settings["{id}"]
    .Request()
    .UpdateAsync(directorySetting);

```