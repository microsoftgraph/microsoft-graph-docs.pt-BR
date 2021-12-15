---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 836e0e3bc750d60a97dd2cfa7b5559077c5b6aab
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var availability = "DoNotDisturb";

var activity = "DoNotDisturb";

var expirationDuration = new Duration("PT8H");

await graphClient.Users["{user-id}"].Presence
    .SetUserPreferredPresence(availability,activity,expirationDuration)
    .Request()
    .PostAsync();

```