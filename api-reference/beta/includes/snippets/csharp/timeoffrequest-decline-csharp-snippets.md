---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1043278684a9ec675409ae588094b7b21eb33fe5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```