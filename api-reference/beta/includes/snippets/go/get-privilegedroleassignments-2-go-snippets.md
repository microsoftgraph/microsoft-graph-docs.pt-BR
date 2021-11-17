---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbd92aecaa773f32673d97e2541e01b31b5c61df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019665"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "isElevated%20eq%20true",
}
options := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.PrivilegedRoleAssignments().Get(options)


```