---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1761b92e39057777cc20975e842a35a65726689
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequestId}"]
    .Decline(message)
    .Request()
    .PostAsync();

```