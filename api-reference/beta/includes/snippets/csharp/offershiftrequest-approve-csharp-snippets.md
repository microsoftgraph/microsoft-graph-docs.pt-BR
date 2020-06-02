---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 274f5153a12c04dac412a06e867f58263748b2eb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "Approved!";

await graphClient.Teams["{teamId}"].Schedule.OfferShiftRequests["{offerShiftRequestId}"]
    .Approve(message)
    .Request()
    .PostAsync();

```