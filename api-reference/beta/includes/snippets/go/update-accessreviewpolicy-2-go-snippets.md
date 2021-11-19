---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b623243270adec012b980fac956ec4a7dfc4fece
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089561"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewPolicy()
isGroupOwnerManagementEnabled := true
requestBody.SetIsGroupOwnerManagementEnabled(&isGroupOwnerManagementEnabled)
options := &msgraphsdk.PolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.IdentityGovernance().AccessReviews().Policy().Patch(options)


```