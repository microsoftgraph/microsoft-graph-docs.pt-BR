---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4588dc6a6fa880043ef6e123edfcfd069aec8ae8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequests = await graphClient.Teams["{team-id}"].Schedule.SwapShiftsChangeRequests
    .Request()
    .GetAsync();

```