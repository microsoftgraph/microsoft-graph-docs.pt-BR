---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21441decc41e0992d7f43e5cb93bcdbfd78cd61c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794980"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "Sorry, you can't offer this shift.";

await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests["{offerShiftRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```