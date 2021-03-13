---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 630b043046dc4cac61a919f5e6a564727b1ef0d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemInsightsSettings = new ItemInsightsSettings
{
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
};

await graphClient.Organization["{organization-id}"].Settings.ItemInsights
    .Request()
    .UpdateAsync(itemInsightsSettings);

```