---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a539dffa674d4670b9ca1725409b699bf5e49a1e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequest-id}"]
    .Approve(message)
    .Request()
    .PostAsync();

```