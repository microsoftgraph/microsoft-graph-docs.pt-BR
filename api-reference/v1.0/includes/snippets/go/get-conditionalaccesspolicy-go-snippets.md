---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21e92308b6148724ff21cb449d3a266b464ac505
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979351"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

conditionalAccessPolicyId := "conditionalAccessPolicy-id"
result, err := graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Get(options)


```