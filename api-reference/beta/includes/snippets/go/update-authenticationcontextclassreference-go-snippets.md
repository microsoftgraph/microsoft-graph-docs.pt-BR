---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08f3e60fdf5c74917e496e1187fec4754ea3f268
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982341"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAuthenticationContextClassReference()
requestBody.SetAdditionalData(map[string]interface{}{
    "value":  []Object {
    }
}
options := &msgraphsdk.AuthenticationContextClassReferenceRequestBuilderPatchOptions{
    Body: requestBody,
}
authenticationContextClassReferenceId := "authenticationContextClassReference-id"
graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferencesById(&authenticationContextClassReferenceId).Patch(options)


```