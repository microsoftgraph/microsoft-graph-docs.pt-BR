---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84bbbf2618c1c02d81587ca95bef16647843aeea
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequests = await graphClient.Teams["{teamId}"].Schedule.SwapShiftsChangeRequests
    .Request()
    .GetAsync();

```