---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 445af123b44e200a7cdb5049bc10c9d36a5344fd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007535"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewProfileCardProperty()
requestBody.SetAnnotations( []ProfileCardAnnotation {
    msgraphsdk.NewProfileCardAnnotation(),
    SetAdditionalData(map[string]interface{}{
        "localizations":  []Object {
        }
    }
}
options := &msgraphsdk.ProfileCardPropertyRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
profileCardPropertyId := "profileCardProperty-id"
graphClient.OrganizationById(&organizationId).Settings().ProfileCardPropertiesById(&profileCardPropertyId).Patch(options)


```