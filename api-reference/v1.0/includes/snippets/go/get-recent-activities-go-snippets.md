---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8058a07ece2feeb2238dfa5d86d48a1d2a2c7c87
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016193"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userActivityId := "userActivity-id"
result, err := graphClient.Me().ActivitiesById(&userActivityId).Get(options)


```