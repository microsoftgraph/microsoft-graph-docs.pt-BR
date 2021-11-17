---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 970ed1bb84cd9c8af43385c4c4e0f9918ef3719b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974379"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

conditionalAccessPolicyId := "conditionalAccessPolicy-id"
graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Patch(options)


```