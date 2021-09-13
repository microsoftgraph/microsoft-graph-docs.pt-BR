---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00c88ee961d7729bd0d23e674b5031ce3bcc66180e8cb098cbceaa1eb64beea1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.SwapShiftsChangeRequests["{swapShiftsChangeRequest-id}"]
    .Approve(message)
    .Request()
    .PostAsync();

```