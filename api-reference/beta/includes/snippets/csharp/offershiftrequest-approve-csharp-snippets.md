---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12aabd71348b8bf7a94b25632d9c10818f7abb95
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "Approved!";

await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests["{offerShiftRequest-id}"]
    .Approve(message)
    .Request()
    .PostAsync();

```