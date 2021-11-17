---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9b65fc7c9062cd3c3167800dbc7c5353338bb66
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017208"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter%20: "%20principalIds/any(x:x%20eq%20'564ae70c-73d9-476b-820b-fb61eb7384b9')",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.RoleManagement().DeviceManagement().RoleAssignments().Get(options)


```