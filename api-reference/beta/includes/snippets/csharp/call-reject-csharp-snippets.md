---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84fa460e4c37752bdaaacf1df648ee91f83e8c0600b932d7c8b2fb195f79da0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.Busy;

await graphClient.Communications.Calls["{call-id}"]
    .Reject(reason,null)
    .Request()
    .PostAsync();

```