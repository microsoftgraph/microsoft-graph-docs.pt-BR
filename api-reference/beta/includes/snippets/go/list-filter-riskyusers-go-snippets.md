---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4e9991459ec2076846ba7d56bacaf20068e872a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979945"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RiskyUsersRequestBuilderGetQueryParameters{
    Filter: "riskLevel%20eq%20microsoft.graph.riskLevel'medium'",
}
options := &msgraphsdk.RiskyUsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityProtection().RiskyUsers().Get(options)


```