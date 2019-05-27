---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b28631a00c285f8556e5cbe6a913672ed2cd600b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468665"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = new GroupSetting
{
    DisplayName = "displayName-value",
    TemplateId = "templateId-value",
    Values = new List<SettingValue>()
    {
        new SettingValue
        {
            Name = "name-value",
            Value = "value-value"
        }
    }
};

await graphClient.GroupSettings
    .Request()
    .AddAsync(groupSetting);

```