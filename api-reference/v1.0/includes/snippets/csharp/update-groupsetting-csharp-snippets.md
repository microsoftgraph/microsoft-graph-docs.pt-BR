---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca1d572b420d5810b49aca9e72402936bb6fc5e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    DisplayName = "GroupSettings",
    TemplateId = "08d542b9-071f-4e16-94b0-74abb372e3d9",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "AllowToAddGuests",
            Value = "false"
        }
    }
};

await graphClient.Groups["{group-id}"].Settings["{groupSetting-id}"]
    .Request()
    .UpdateAsync(groupSetting);

```