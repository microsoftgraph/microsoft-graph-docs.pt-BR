---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5872b89989126a9de9aa6d2b91eda5c6a1c41e21
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873929"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var used = await graphClient.Me.Insights.Used
    .Request()
    .OrderBy("LastUsed/LastAccessedDateTime desc")
    .GetAsync();

```