---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67c8b972d6445f806a288d5e11042802287fb06a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49656994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["{id}"].Teamwork.InstalledApps["{id}"].Chat
    .Request()
    .GetAsync();

```