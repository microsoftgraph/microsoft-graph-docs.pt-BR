---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75d73e2fb3c95f054118bb2e8299d9d0e6c485dd
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

var availability = "Available";

var activity = "Available";

var expirationDuration = new Duration("PT1H");

await graphClient.Users["{user-id}"].Presence
    .SetPresence(sessionId,availability,activity,expirationDuration)
    .Request()
    .PostAsync();

```