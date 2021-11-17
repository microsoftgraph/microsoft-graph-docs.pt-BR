---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9bc36180bafea392edfa34aac798b165f7538aa3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007237"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter%20: "%20principalId%20eq%20'f1847572-48aa-47aa-96a3-2ec61904f41f'",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignments().Get(options)


```