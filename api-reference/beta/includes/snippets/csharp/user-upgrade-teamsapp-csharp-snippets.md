---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 445f64a8218b3120acab968001133a868d57990c
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931195"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id}"].Teamwork.InstalledApps["{id}"]
    .Upgrade()
    .Request()
    .PostAsync();

```