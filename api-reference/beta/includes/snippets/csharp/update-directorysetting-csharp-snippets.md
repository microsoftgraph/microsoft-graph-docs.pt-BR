---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88800dfee9e2391b13fd68604b167411e3430687
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498410"
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