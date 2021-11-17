---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac2a90687ed93574bccf221b5695fe6dc67a64e3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010622"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SwapShiftsChangeRequests().Get(options)


```