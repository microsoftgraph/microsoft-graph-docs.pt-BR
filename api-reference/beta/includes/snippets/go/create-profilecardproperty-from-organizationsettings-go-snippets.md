---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bafebbbd6aad3731372f1e60a875cd51f7c0b0bc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089263"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProfileCardProperty()
directoryPropertyName := "CustomAttribute1"
requestBody.SetDirectoryPropertyName(&directoryPropertyName)
requestBody.SetAnnotations( []ProfileCardAnnotation {
    msgraphsdk.NewProfileCardAnnotation(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Cost Center",
        "localizations":  []Object {
        }
    }
}
options := &msgraphsdk.ProfileCardPropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ProfileCardProperties().Post(options)


```