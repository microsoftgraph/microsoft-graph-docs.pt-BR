---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44b1251722a91b111942712857efd7de7eaa78d0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null",
}
options := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.PrivilegedRoleAssignments().Get(options)


```